---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Início
---
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
<script type="text/javascript">
	$(document).ready(function() {
		$('#coin-slider').coinslider(
			{height: 400, navigation: true, delay: 5000, opacity: 0.7}
		);
	});
</script>