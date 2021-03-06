---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Início
---
<!--
<div id='coin-slider'>
	{% for s in site.data.slide_data%}
	<a class="slider-item" href="{{s.link}}" target="_blank">
		<img src="{{s.img}}"/>
		<span>
			{{s.desc}}
		</span>
	</a>
	{% endfor %}
</div>
-->
<div class="rd-slide">
	{%for s in site.data.slide_data %}
	<div>
		<a href="{{s.link}}">
			<img src="{{s.img}}"/>
			<span>
				{{s.desc}}
			</span>
		</a>
	</div>
	{% endfor %}
</div>