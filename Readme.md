<h1 align="center">Opera Blocklist</h1>

<p align="center">
  <img alt="License" src="https://img.shields.io/static/v1?label=license&message=MIT&color=49AA26&labelColor=000000">
</p>

Essa é uma lista de itens para o navegador [Opera GX](https://opera.com/pt-br/gx) usar no bloqueador de anuncios.

## Como usar

No Opera GX, acesse a guia de "Proteção de privacidade" abra o "Bloquear Anúncios - Gerenciar listas", no final da pagina em "Listas personalizadas", clique em adicionar e cole o seguinte link

```
https://raw.githubusercontent.com/Jonas-Portes/Opera-Blocklist/main/blockView.txt
```


<div class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="OPJqPKp" data-pen-title="Aula 1 - Conversor de moedas" data-user="Jonas-portes"  data-prefill='{"title":"Aula 1 - Conversor de moedas","tags":["imersaodev","alura"],"scripts":[],"stylesheets":[]}'>
  <pre data-lang="html">&lt;body>
	&lt;img src="https://i.postimg.cc/GpCxYmvc/title.png" alt="Logo" class="logo">

	&lt;div class="container">
		&lt;div class="content">
			&lt;h2>Grande conversão, de USD para BRL ou vice versa!&lt;/h2>
			&lt;p> Vamos ver a conversão?&lt;/p>
			&lt;button onclick="conversor()">Bora converter!&lt;/button>
		&lt;/div>
	&lt;/div>
	&lt;footer>Alura - Imersão DEV - 2025&lt;/footer>
&lt;/body></pre>
  <pre data-lang="css">/* Global Styles */
body {
	background-color: black;
	margin: 0;
	padding: 0;
	font-family: Arial, sans-serif;
	color: white;
	position: relative;
}

/* Logo Styles */
.logo {
	position: absolute;
	top: 20px;
	right: 20px;
	max-width: 150px;
	width: auto;
}

/* Container with the background image */
.container {
	background: url("https://i.postimg.cc/zXBWJgHm/a19e4e49a05d5f2385ec71be97c5f482.jpg") no-repeat center
		center/cover;
	min-height: 100vh;
	display: flex;
	justify-content: center;
	align-items: center;
}

/* Content div for text and button */
.content {
	text-align: center;
	background-color: rgba(0, 0, 0, 0.5);
	padding: 20px 40px;
	border-radius: 8px;
}

.content h2 {
	margin-bottom: 20px;
}

/* Button Styles */
button {
	background-color: #ff1b7b;
	border: none;
	padding: 10px 20px;
	font-size: 1.2em;
	color: white;
	cursor: pointer;
	transition: background-color 0.3s ease;
}

button:hover {
	background-color: #1abc9c;
}

/* Footer Styles */
footer {
	text-align: center;
	padding: 10px;
}
</pre>
  <pre data-lang="js">userValue = 0;

function conversor() {
	userChoice = prompt("Deseja converter BRL para USD (1) ou USD para BRL (2) ?");
	usdRate = 5.63;
	userValue = parseFloat(prompt("Ao invés de digitar um valor com vírgula, use ponto. Exemplo: 1.99"));
		
	while (typeof userValue === "string" || isNaN(userValue)){
		userValue = parseFloat(prompt("Ao invés de digitar um valor com vírgula, use ponto. Exemplo: 1.99"));
		}
	
	let result;
	if (userChoice == 1) {
		//brl para usd
		result = userValue / usdRate;
	
		alert(userValue + " reais é igual a: " + parseFloat(result.toFixed(2)) + " dolares");
	} else {
		//usd para brl
		result = userValue * usdRate;
		
		alert(userValue + " dolares é igual a: " + parseFloat(result.toFixed(2)) + " reais");
	}
}


</pre></div>
<script async src="https://public.codepenassets.com/embed/index.js"></script>
