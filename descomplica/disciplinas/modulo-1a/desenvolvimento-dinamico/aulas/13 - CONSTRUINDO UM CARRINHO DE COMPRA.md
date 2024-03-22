## Construindo um carrinho de compra

**Resumo**  

Nesta aula, vamos construir um carrinho de compras com um layout que pode ser adaptado e ajustado conforme as nossas necessidades. No final desta aula, você terá construído um carrinho de compras que pode servir de base para outros carrinhos de compras que você possa construir futuramente.

**Construindo o carrinho de compras**

A primeira etapa que precisamos fazer é pegar um template gratuito do Bootstrap que tenha um carrinho de compras interessante para trabalharmos. Para isso, podemos acessar o link [https://bbbootstrap.com/snippets/bootstrap-ecommerce-cart-page-template-91851305](https://bbbootstrap.com/snippets/bootstrap-ecommerce-cart-page-template-91851305) **(acesso em 27/06/2023)**, onde teremos um bom exemplo de carrinho de compras.

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698258088289-wotiB1rJqj.png)

  

Fonte: [https://bbbootstrap.com/snippets/bootstrap-ecommerce-cart-page-template-91851305](https://bbbootstrap.com/snippets/bootstrap-ecommerce-cart-page-template-91851305) **(acesso em 27/06/2023)**

Em seguida, teremos que fazer as devidas alterações no nosso código para contemplar a implementação do carrinho de compras com Javascript.

O próximo passo é pegar o código html disponível, colocar em uma pasta e começarmos a trabalhar nele.

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698258109351-AqsDfm3Jgp.png)

  

Fonte: [https://bbbootstrap.com/snippets/bootstrap-ecommerce-cart-page-template-91851305](https://bbbootstrap.com/snippets/bootstrap-ecommerce-cart-page-template-91851305) **(acesso em 27/06/2023)**

Faça o mesmo para o arquivo css do exemplo e crie também um arquivo Javascript para contemplar nosso código que iremos implementar.

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698258145751-rpPoVHvFyl.png)

  

Fonte: Autoral

Em seguida, temos que fazer as definições de alguns ids conforme as imagens a seguir:

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698258176514-ufmbzsv2sG.png)

  

Fonte: Autoral

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698258190730-ilWoq1hUNj.png)

  

Fonte: Autoral

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698258208985-ArL7YS1HNV.png)

  

Fonte: Autoral

**Conteúdo Bônus**

Nosso carrinho de compras precisa de interação para fazê-lo funcionar. Sendo assim, vamos implementar nosso primeiro código, que consiste em adicionar um item. Veja o código abaixo:

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698258225339-6yEjxsVAQf.png)

  

Fonte: Autoral

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698258241197-rZjU669Y2e.png)

  

Fonte: Autoral

Para removermos um item, podemos fazer da seguinte forma:

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698258260534-Tfvy7JFHmS.png)

  

Agora vamos aplicar as funções criadas no html:

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698258284273-4kVCYzR637.png)

  

Fonte: Autoral

Para fazer o valor total da compra, implemente o código abaixo:

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698258307444-idAbR6efuv.png)

  

Fonte: Autoral

Os códigos acima são os exemplos que estamos utilizando nas aulas para criar nosso carrinho de compras. Implemente os códigos demonstrados e depois execute seu carrinho de compras para ter sucesso nesse aprendizado.

  

**Referência Bibliográfica**

FLANAGAN, David. **JavaScript: O Guia Definitivo**. 6ª Ed. Porto Alegre: Bookman, 2013.

FREEMAN, Eric. **Use a cabeça!: programação JavaScript**. 1ª Ed. São Paulo: Alta Books, 2016.

  

**ATIVIDADE PRÁTICA  
**

**Título da Prática:**  Adicionar itens

**Objetivos:** Implementar itens em uma lista

**Materiais, Métodos e Ferramentas:** Para realizar esta prática vamos utilizar o Visual Studio Code.

  

**Prática**

Essa prática consiste em criar um código em JavaScript que permita ao usuário adicionar itens a uma lista por meio de um campo de texto no HTML. O programa deve capturar o valor inserido no campo de texto e, ao clicar no botão ‘Adicionar’, adicionar o item à lista exibida na página. Caso o campo de texto esteja vazio, nenhum item deve ser adicionado. O objetivo é criar uma interface interativa e intuitiva, facilitando o registro e a exibição dos itens adicionados pelo usuário. O código deve garantir que a lista seja atualizada em tempo real, possibilitando o registro eficiente dos itens inseridos.

Boa sorte e divirta-se resolvendo o exercício!

  

**Resolução**

<!DOCTYPE html>

<html>

<head>

  <title>Lista de Itens</title>

  <script>

    function adicionarItem() {

      var item = document.getElementById(‘item’).value; // Obtém o valor do campo de texto

      var lista = document.getElementById(‘lista’); // Obtém a lista de itens

      // Verifica se o campo de texto não está vazio

      if (item !== ‘’) {

        var novoItem = document.createElement(‘li’); // Cria um novo elemento <li>

        novoItem.appendChild(document.createTextNode(item)); // Adiciona o texto do campo de texto ao novo elemento <li>

        lista.appendChild(novoItem); // Adiciona o novo elemento à lista

        document.getElementById(‘item’).value = ‘’; // Limpa o campo de texto

      }

    }

  </script>

</head>

<body>

  <h1>Lista de Itens</h1>

  <input type=“text” id=“item” placeholder=“Digite um item”>

  <button onclick=“adicionarItem()”>Adicionar</button>

  <ul id=“lista”></ul>

</body>

</html>

[[14 - EXCEPTION]]