CTRL + / para comentar um bloco
*Seletor * (all)*
Com o seletor all, todos os atributos sao atribuidos a todos os elementos. Normalmente utilizamos para zerar o margin e o padding do box model dos elementos para estilizarmos conforme nossa vontade pois quase todos os elementos precisamos definir esses atributos.
```css
* {
	margin: 0;
	padding: 0;
}
```

*Seletor por tag
p {}*
Com esse seletor todas as tags 'p' serao atribuidos os valores do css.
```css
p {
	color: red;
}
```

*Seletores com especificidade (selecao de descendente)
body div section p {}*
Dessa forma especificamos um pouco para o css aplicar nas tags que sao irmaos (lemos: toda tag p que esta dentro da section dentro de uma div que esta dentro do body)
```css
body div section p {
	color: blue;
}
```

Podemos fazer mais de uma selecao com uma virgula:
*body div section p,
body div section h1 {}*
```css
body div section p,
body div section h1 {
	color: yellow;
}
```

Mais exemplos:
*h1,p {}*
```css
h1, p {
	color: green;
}
```

**OBS: Conforme maior especificidade, mais dificil fica de mudar o atributo daquele elemento**

*Seletor de classe
.bg-blue*
O seletor de classe, utilizamos para selecionar os elementos que contenham o atributo classe correspondente.
```css
.bg-blue {
	background: blue;
}
```

Muito melhor usar classe para estilizar do que tags.

Tem como selecionarmos um grupo de tags dentro de uma tag que tem classe, exemplo:
Abaixo selecionamos os h2 que estejam dentro de uma tag que contenha a classe main-content.
```css
.main-content h2 {
	color: blue;
}
```

Conseguimos selecionar com mais de uma classe:
```css
.main-content .heading .outra-coisa {
	font-style: italic;
	color: red;
}
```

Se quisermos selecionar uma tag com classe especifica:
```css
.main-content h2.heading {
	color: yellow;
}
```
Acima selecionamos um h2 que tenha a classe heading definida e que esteja dentro de um elemento que tenha a classe main-content.