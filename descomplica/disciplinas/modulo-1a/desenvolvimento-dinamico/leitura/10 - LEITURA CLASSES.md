## Classes

**Resumo**  

Nesta aula, iremos aprender como utilizar as classes para organizar melhor o nosso desenvolvimento. O uso de classe tem se tornado mais comum no desenvolvimento com JavaScript devido ao crescimento do uso do Node.js. O que você aprenderá aqui será possível utilizar em aplicações, inclusive no Angular. A base que está sendo ensinada permite ser utilizada em outras tecnologias. Portanto, vamos compreender agora o uso de classes.

**Classes**

Quando definimos uma classe, um ponto importante é utilizar o construtor. Com ele, é possível manipular os parâmetros que foram passados ao instanciar uma classe.

Ele é definido em um bloco de classe, como se você estivesse definindo um método chamado construtor, embora ele seja realmente manipulado como um caso especial.

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698256938901-DX95PjdLoT.png)

Fonte: Autor

Como podemos usar essa classe?

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698256985185-4Nsle4hc3c.png)

  

Fonte: Autor

Outra forma de usar classe é através de herança. A herança funciona exatamente como em outras linguagens orientadas a objetos: os métodos definidos na superclasse são acessíveis na subclasse de extensão. Se a subclasse declara seu próprio construtor, então ele deve invocar o construtor pai via super() antes que ele possa acessar this.

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698257010896-AzICzAZEYJ.png)

  

Fonte: Autor

Getters e setters permitem que você defina um comportamento personalizado para ler e escrever uma determinada propriedade em sua classe. Para o usuário, eles aparecem como uma propriedade normal. No entanto, internamente, uma função personalizada é fornecida e usada para determinar o valor quando a propriedade é acessada (o getter) e para executar as alterações necessárias quando é atribuída (o setter). Em uma definição de classe, um getter é escrito como um método sem argumento prefixado pela palavra-chave get. Um setter é semelhante, exceto que ele aceita um argumento (o novo valor que está sendo atribuído). Aqui está uma classe de exemplo que fornece um getter e setter para sua propriedade .nome.

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698257036186-LhgVFw3AlD.png)

  

Fonte: Autoral

**Composição**

Composição é um padrão de design em que um objeto é composto por outros objetos menores, cada um responsável por uma parte específica da funcionalidade geral. Em JavaScript, a composição é uma técnica que permite criar objetos complexos a partir de outros objetos mais simples, combinando suas funcionalidades.

A composição em JavaScript geralmente é realizada por meio de objetos aninhados ou funções que retornam objetos. Um objeto pode ser composto por outros objetos que fornecem comportamentos específicos. Por exemplo, suponha que você tenha uma classe “Carro” que precisa ter recursos de “Motor”, “Transmissão” e “Rodas”. Em vez de criar uma classe grande que implemente tudo isso, você pode criar objetos separados para cada recurso e combiná-los usando a composição.

Veja um exemplo básico de como usar a composição em JavaScript:

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698257063322-DCr8TwSKgU.png)

  

Fonte: Autoral

Neste exemplo, a classe “Carro” recebe um objeto “Motor” como argumento do construtor e o armazena em uma propriedade. O método “acelerar” do objeto “Carro” usa o objeto “Motor” para obter informações sobre a cilindrada e imprimir uma mensagem. Isso permite que a classe “Carro” tenha acesso a funcionalidade específica do objeto “Motor” sem precisar implementá-la diretamente.

**Conteúdo Bônus**

Para utilizar da melhor forma as classes em JavaScript, devemos separar cada classe em um arquivo e transformar em um módulo que será importado onde desejamos usar. Vejamos o exemplo abaixo:

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698257081856-TtErT6kpWB.png)

  

Fonte: Autoral

Para utilizar essa classe em outra classe, temos que fazer o require. Dessa forma, conseguimos usar de uma forma mais organizada o javascript orientado a objetos.

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698257107938-tGT8sjZg21.png)

  

Fonte: Autoral

Agora podemos chamar o programa e teremos o seguinte resultado:

![](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1698257126076-zpAjoA0XlH.png)

  

Fonte: Autoral

**Referência Bibliográfica**

FLANAGAN, David. **JavaScript: O Guia Definitivo**. 6ª Ed. Porto Alegre: Bookman, 2013.

FREEMAN, Eric. **Use a cabeça!: programação JavaScript**. 1ª Ed. São Paulo: Alta Books, 2016.

Ir para exercício

[[11 - MANIPULANDO ELEMENTOS DO DOM]]