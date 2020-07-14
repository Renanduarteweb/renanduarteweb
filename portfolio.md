---
layout: page
title: Portfólio
permalink: /portfolio/
imgbg: ../assets/img/mesa-de-trabalho.jpg
---
<h1>{{page.title}}</h1>
{%assign count = 0 %}
{%for port in site.data.portfolio%}
{%if count == 0%}
<div class="rd-card-container">
{%endif%}
	<div class="rd-card-item">
		{%if port.screenshot %}
		<img class="rd-card-item-img" src="{{port.screenshot}}" alt="img do port"/>
		{%else%}
		<img class="rd-card-item-img" src="../assets/img/notebook_flat.png" alt="img do port"/>
		{%endif%}
		<a class="rd-card-item-desc" href="{{port.link | relative_url}}">
			<h3>{{port.title}}</h3>
			<p>
				{{port.desc}}
			</p>
		</a>
	</div>
	{%assign count = count | plus: 1 %}
	{%if count == 3%}
	{%assign count = 0 %}
	{%endif%}
{%if count == 0 %}
</div>
{%endif%}
{%endfor%}