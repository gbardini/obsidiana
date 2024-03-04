## CSS: Entendendo sobre estilos

[[8 - CSS Criando Estilos]]

**​Introdução**  

CSS, ou Cascading Style Sheets, é uma linguagem de marcação usada para definir a aparência e o layout de páginas da web. Ela é composta por regras que especificam como os elementos HTML devem ser exibidos no navegador.

CSS é uma linguagem poderosa que permite aos desenvolvedores web criar páginas da web personalizadas e responsivas. Com CSS, é possível controlar a cor, o tamanho, a fonte, a borda, a margem e outros aspectos da apresentação dos elementos HTML. O CSS também pode ser usado para criar efeitos visuais, como animações e transições.

O CSS é uma parte essencial do desenvolvimento web. É uma ferramenta fundamental para criar páginas da web bonitas e funcionais.

  

**Objetivos da aula**

●      Definir o conceito de CSS.

●      Discutir a estrutura básica do CSS.

●      Identificar forma de implementar CSS.

  

**Resumo**

**O que é o CSS e como é sua sintaxe**

O CCS, é o acrônimo de _Cascading Style Sheets,_ cuja tradução para português significa Folhas de estilo em cascata. É uma linguagem usada para formatar a apresentação de uma página em HTML no navegador. Os padrões desta linguagem são definidos pelo W3C, mesmo consórcio que define os padrões para a linguagem HTML.

O CSS foi criado em 1996 para remover da página HTML o estilo, que antes era atribuído por tags como _<font>_ que eram um pesadelo para desenvolvedores pois se aplicavam a cada elemento HTML. Para resolver esse problema, o _World Wide Web Consortium_ (W3C) criou o CSS, que economiza muito trabalho controlando o layout de várias páginas da web de uma só vez. O CSS atualmente está em sua terceira versão.

A linguagem CSS é utilizada para definir propriedades de elementos HTML, como cores, fontes, tamanhos de texto, espaçamento entre elementos, posicionamento dos elementos, definição de imagens de fundo ou cores de fundo e variações de exibição para diferentes dispositivos e tamanhos de tela. A palavra “cascata” significa que um estilo aplicado a um elemento pai também se aplicará a todos os elementos filhos dentro do pai.

A sintaxe do CSS compõe-se de um seletor, abertura de chaves, declaração de propriedade e valor para esta, como no exemplo a seguir, onde atribui-se ao seletor p a fonte verdana e o tamanho de 20px.

p {    font-family: verdana;    font-size: 20px;  
}

▪         O seletor aponta para o elemento HTML que se deseja estilizar.

▪         O bloco de declaração contém uma ou mais declarações separadas por ponto e vírgula.

▪         Cada declaração inclui um nome de propriedade CSS e um valor, separados por dois pontos.

▪         Os blocos de declaração são cercados por chaves.

**Formas de adicionar CSS ao documento HTML**

●      Existem três formas de adicionar CSS a uma página HTML:

◦         Inline (em linha): Um estilo embutido usado para aplicar um estilo único para um único elemento. Deve se adicionar o atributo style ao elemento que ser quer alterar e dentro dele, definir as propriedades, como no exemplo a seguir

<h1 style=“color:blue;text-align:center;”>Título</h1>  
<p style=“color:red;”>Parágrafo</p>

◦         Internal (interno): O código CSS é definido na própria página HTML, dentro do elemento <style>, dentro da seção <head>. Exemplo:

<!DOCTYPE html>  
<html>  
<head>      <style>         body {                 background-color: linen;         }         h1 {                 color: maroon;                 margin-left: 40px;         }      </style>  
</head>  
<body>      Corpo da página  
</body>

◦         External (externo): Um arquivo externo à página HTML que deve ser incluído via elemento <link>, dentro da seção <head>. no cabeçalho da página. Com uma folha de estilo externa, você pode alterar a aparência de um site inteiro alterando apenas um arquivo!  Exemplo:

<!DOCTYPE html>  
<html>  
<head>      <link rel=“stylesheet” href=“mystyle.css”>  
</head>  
<body>

                        Corpo da página                  </body>                  </html>

  

**Conteúdo Bônus**

Para descobrir o que é possível fazer com expertise em CSS, uma ótima maneira é procurar por prêmios de design web. Existem vários sites que organizam concursos e premiações para sites que se destacam pela beleza, usabilidade e inovação.

Alguns dos sites mais populares são o CSS Design Awards, o Awwwards e o Webby Awards. Esses sites recebem milhares de inscrições todos os anos, e os vencedores são escolhidos por um júri de especialistas.

Além de conferir os sites premiados, você também pode visitar os portfólios de designers e desenvolvedores que trabalham com CSS. Isso lhe dará uma boa ideia de como eles aplicam a linguagem para criar sites bonitos e funcionais.

  

**Dica quente para você não esquecer**

Você pode usar o **_W3C_** [**_CSS Validation Service_**](https://jigsaw.w3.org/css-validator/) para verificar se o seu CSS é válido. Essa é uma ferramenta indispensável para depuração: [https://jigsaw.w3.org/css-validator/](https://jigsaw.w3.org/css-validator/)

  

  

**Referência Bibliográfica**

DEVELOPER. **CSS**. Disponível em: [https://developer.mozilla.org/pt-BR/docs/Web/CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS) Acesso em: 20 set. 2022.

W3Schools is Powered by W3. **CSS Tutorial**. Disponível em: [https://www.w3schools.com/css/default.asp](https://www.w3schools.com/css/default.asp) Acesso em: 20 set. 2022.

  

  

**Atividade Prática 7**: CSS: Entendendo sobre estilos

**Título da Prática:** Estilizando uma Página Web com CSS

**Materiais e Ferramentas**:

●     Editor de texto (recomendado: Visual Studio Code, Sublime Text ou Atom)

●     Navegador web (recomendado: Google Chrome, Mozilla Firefox ou Microsoft Edge)

●     Conhecimento básico em HTML

**Objetivo**:

O aluno deverá aplicar os conceitos aprendidos sobre CSS para estilizar uma página web, utilizando diferentes métodos de implementação de estilos.

  

**Enunciado**:

1. Crie uma página HTML básica com os seguintes elementos: um título (<h1>), dois parágrafos (<p>) e uma lista não ordenada (<ul>) com três itens (<li>).

2. Aplique estilos **inline** ao título, alterando sua cor para azul e alinhando-o ao centro.

3. Utilize estilos internos para:

   - Alterar a cor de fundo da página para cinza claro.

   - Estilizar os parágrafos com fonte “Arial”, tamanho de 16px e cor verde.

4. Crie um arquivo externo chamado “styles.css”. Neste arquivo:

   - Defina a cor dos itens da lista para roxo.

   - Aplique um espaçamento de 15px entre os itens da lista.

5. Vincule o arquivo “styles.css” à sua página HTML e verifique se os estilos foram aplicados corretamente.

  

**Resolução Comentada**:

1. A estrutura básica da página HTML:

html  
  
<!DOCTYPE html>  
  
<html>  
  
<head>  
  
    <title>Atividade Prática - CSS</title>  
  
</head>  
  
<body>  
  
    <h1>Meu Título</h1>  
  
    <p>Este é o primeiro parágrafo.</p>  
  
    <p>Este é o segundo parágrafo.</p>  
  
    <ul>  
  
        <li>Item 1</li>  
  
        <li>Item 2</li>  
  
        <li>Item 3</li>  
  
    </ul>  
  
</body>  
  
</html>  
  
  
2. Estilo inline aplicado ao título:  
  
html  
  
<h1 style=“color:blue;text-align:center;”>Meu Título</h1>  
  
  
3. Estilos internos aplicados:  
  
html  
  
<head>  
  
    <title>Atividade Prática - CSS</title>  
  
    <style>  
  
        body {  
  
            background-color: lightgray;  
  
        }  
  
        p {  
  
            font-family: Arial;  
  
            font-size: 16px;  
  
            color: green;  
  
        }  
  
    </style>  
  
</head>  
  
  
4. No arquivo “styles.css”:  
  
css  
  
li {  
  
    color: purple;  
  
    margin: 15px 0;  
  
}  
  
  
  
5. Vinculando o arquivo “styles.css” à página HTML:  
  
html  
  
<head>  
  
    <title>Atividade Prática - CSS</title>  
  
    <link rel=“stylesheet” href=“styles.css”>  
  
    <style>  
  
        body {  
  
            background-color: lightgray;  
  
        }  
  
        p {  
  
            font-family: Arial;  
  
            font-size: 16px;  
  
            color: green;  
  
        }  
  
    </style>  
  
</head>  
  

Ao abrir a página no navegador, os alunos deverão ver os estilos aplicados conforme as instruções.

