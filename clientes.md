---
layout: page
title: Clientes
permalink: /clientes/
imgbg: ../assets/img/thumbs-up.jpg
---
<h1>{{page.title}}</h1>
{%assign count = 0 %}
{%for cliente in site.data.clientes%}
{%if count == 0%}
<div class="rd-card-container">
{%endif%}
	<div class="rd-card-item">
		{%if cliente.img%}
		<img class="rd-card-item-img" src="{{cliente.img}}" alt="img do  cliente"/>
		{%else%}
		<img class="rd-card-item-img" src="../assets/img/pessoa_flat.png" alt="img do port"/>
		{%endif%}
		<a class="rd-card-item-desc" href="{{cliente.link | relative_url}}">
			<h3>{{cliente.name}}</h3>
		<p>
			{{cliente.desc}}
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