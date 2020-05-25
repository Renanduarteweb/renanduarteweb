---
layout: page
title: Portfólio
permalink: /portfolio/
imgbg: ../assets/img/portfolio.png
---
<h1>{{page.title}}</h1>
{%assign count = 0 %}
{%for port in site.data.portfolio%}
{%if count == 0%}
<div class="rd-card-container">
{%endif%}
	<div class="rd-card-item">
		<h3>{{port.title}}</h3>
		<a href="{{port.link | relative_url}}">Ir para o projeto</a>
		<p>
			{{port.desc}}
		</p>
	</div>
	{%assign count = count | plus: 1 %}
	{%if count == 3%}
	{%assign count = 0 %}
	{%endif%}
{%if count == 0 %}
</div>
{%endif%}
{%endfor%}