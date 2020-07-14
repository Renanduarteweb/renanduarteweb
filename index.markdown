---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Início
imgbg: ../assets/img/led_panel.png
---
<div id='coin-slider'>
	<a class="slider-item" href="#" target="_blank">
		<img src="../assets/img/executives.jpg"/>
		<span>
			<h1>Bem vindo!</h1>
			<p>Precisa de um site? Se sim, está no lugar certo!</p>
		</span>
	</a>
	<a class="slider-item" href="/portfolio/" target="_blank">
		<img src="../assets/img/pensativo.jpg"/>
		<span>
			<h1>Por que devo ter um site?</h1>
			<p>
				Quem não está na internet, não é visto.
			</p>
			<p>
				Para ganhar mais clientes, é necessário que seus serviços sejam vistos por muita gente. E a web é um dos meios (se não o melhor) para tal.
			</p>
			<p>
				Veja alguns exemplos no portifólio
			</p>
		</span>
	</a>
	<a class="slider-item" href="/orcamento.html" target="_blank">
		<img src="../assets/img/governanca-corporativa.png" width="900px" height="400px"/>
		<span>
			<h1>Interessante, mas.... como posso criar um site para meu negócio?</h1>
			<p>
			Não se preocupe, eu faço para você. Solicite um orçamento.
			</p>
		</span>
	</a>
	<!--
<div class="slider_item" id="slide3">
	<h1>Interessante, mas.... como posso criar um site para  meu negócio?</h1>
	<img src="../assets/img/duvida.png"/>
	<p>
		Não se preocupe, eu faço para você. Faça aqui <a href="/orcamento.html">seu orçamento</a>.
	</p>
</div>
-->
</div>
<script type="text/javascript">
	$(document).ready(function() {
		$('#coin-slider').coinslider(
			{height: 400, navigation: true, delay: 5000 });
	});
</script>