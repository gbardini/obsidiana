## Avançando com BootStrap

**Introdução**  
```html
O Bootstrap possui uma biblioteca extensa de componentes disponíveis gratuitamente, contando com diferentes opções de ícones, painéis, caixas de texto e cores em links, para atender a inúmeros estilos.

Como não é necessário criar layouts do zero, o desenvolvimento de projetos web é realizado de maneira mais rápida, o que aumenta a produtividade.

Além disso, o Bootstrap é facilmente adaptável a diferentes tamanhos de tela, seja ela um celular, um tablet ou um computador, oferecendo ao usuário uma melhor experiência ao navegar no site.

  

**Objetivos da aula**

●      Descrever o container de Cards

●      Discutir a implementação com Modal

●      Explicar o componente Carousel

●      Aplicar Forms

●      Definir Layouts com base em outros

  

**Resumo**

**Carrossel**

O **_Carousel_** é um importante componente do Bootstrap que funciona como uma apresentação de slides, na qual os elementos são exibidos um de cada vez, como em um carrossel. O exemplo a seguir mostra como criar um carrossel básico com indicadores e controles:

<div id=“demo” class=“carousel slide” data-bs-ride=“carousel”>

   <div class=“carousel-indicators”>

        <button type=“button” data-bs-target=“#demo” data-bs-slide-to=“0” class=“active”></button>

        <button type=“button” data-bs-target=“#demo” data-bs-slide-to=“1”></button>

        <button type=“button” data-bs-target=“#demo” data-bs-slide-to=“2”></button>

   </div>

   <div class=“carousel-inner”>

        <div class=“carousel-item active”>

                 <img src=“la.jpg” alt=“Los Angeles” class=“d-block w-100”>

        </div>

        <div class=“carousel-item”>

                 <img src=“chicago.jpg” alt=“Chicago” class=“d-block w-100”>

        </div>

        <div class=“carousel-item”>

                 <img src=“ny.jpg” alt=“New York” class=“d-block w-100”>

        </div>

   </div>

   <button class=“carousel-control-prev” type=“button” data-bs-target=“#demo” data-bs-slide=“prev”>

        <span class=“carousel-control-prev-icon”></span>

   </button>

   <button class=“carousel-control-next” type=“button” data-bs-target=“#demo” data-bs-slide=“next”>

        <span class=“carousel-control-next-icon”></span>

   </button>

</div>

Cada classe é responsável por formatar um elemento

●       **._carousel_:** Cria um carrossel

●      **.c_arousel-indicators_:** Adiciona indicadores para o carrossel. Estes são os pequenos pontos na parte inferior de cada slide (que indicam quantos slides existem no carrossel e qual slide o usuário está visualizando no momento)

●       **._carousel-inner_:** Adiciona os slides ao carrossel

●      **._carousel-item_:** Especifica o conteúdo de cada slide

●      **._carousel-control-prev_:** Adiciona um botão esquerdo (anterior) ao carrossel, que permite ao usuário voltar entre os slides

●      **._carousel-control-next_:** Adiciona um botão direito (próximo) ao carrossel, que permite ao usuário avançar entre os slides

●      **._carousel-control-prev-icon_:** Usado junto com **_.carousel-control-prev_** para criar um botão “anterior”

●      **._carousel-control-next-icon_:** Usado junto com **_.carousel-control-next_** para criar um botão “próximo”

●      **._slide_:** Adiciona uma transição CSS e efeito de animação ao deslizar de um item para o próximo.

  

**Cartões (cards)**

Um cartão é um contêiner de conteúdo flexível e extensível que possui opções para cabeçalhos, rodapés e uma ampla variedade de conteúdo e cores de fundo.

●      Um cartão básico é criado com a classe **_.card_,** e o conteúdo dentro do cartão com uma classe **_.card-body_**:

<div class=“card”>

   <div class=“card-body”>Cartão básico</div>

</div>

●      Podemos adicionar a classe **_.card-header_** para criar um cabeçalho e a classe **_.card-footer_** para criar um rodapé no cartão:

<div class=“card”>

        <div class=“card-header”>Cabeçalho</div>

        <div class=“card-body”>Conteúdo</div>

        <div class=“card-footer”>Rodapé</div>

</div>

●      Podemos utilizar a classe **_.card-title_** para adicionar títulos ao cartão. E podemos usar a classe **_.card-text_** para remover as margens inferiores de um elemento **<p>** se este for o último filho (ou o único) dentro de **_.card-body_.** A classe **_.card-link_** adiciona uma cor azul a qualquer link e um efeito de foco.

<div class=“card”>

 <div class=“card-body”>

                 <h4 class=“card-title”>Título do cartão</h4>

                 <p class=“card-text”>Conteúdo do cartão.</p>

                 <a href=“#” class=“card-link”>Link</a>

        </div>

</div>

●      Adicione **_.card-img-top_** ou **_.card-img-bottom_** a um elemento <img> para colocar a imagem na parte superior ou inferior dentro do cartão. Observe que adicionamos a imagem fora do **_.card-body_** para abranger toda a largura:

<div class=“card” style=“width:400px”>

        <img class=“card-img-top” src=“Endereço da imagem” alt=“Card image”>

        <div class=“card-body”>

                 <h4 class=“card-title”>Título</h4>

                 <p class=“card-text”>Texto</p>

                 <a href=“#” class=“btn btn-primary”>Texto para o botão</a>

        </div>

</div>

  

**Modal**

Modal é um _plug-in_ em _JavaScript_ do _Bootstrap_ para adicionar caixas de diálogo flutuantes de notificações que são acionadas por clique.

<button type=“button” class=“btn btn-primary” data-bs-toggle=“modal” data-bs-target=“#myModal”>

 **Abrir Modal**

</button>

<div class=“modal” id=“myModal”>

         <div class=“modal-dialog”>

        <div class=“modal-content”>

                 <div class=“modal-header”>

                          <h4 class=“modal-title”>Cabeçalho da Modal</h4>

                          <button type=“button” class=“btn-close” data-bs-dismiss=“modal”></button>

                 </div>

                 <div class=“modal-body”>

                          Corpo da Modal

                 </div>

                 <div class=“modal-footer”>

                          <button type=“button” class=“btn btn-danger” data-bs-dismiss=“modal”>Fechar</button>

                 </div>

        </div>

         </div>

</div>

●      Podemos usar a classe **_.fade_** para adicionar um efeito de _fade_ ao abrir e fechar o modal:

<div class=“modal fade”></div>

●      Podemos alterar o tamanho da modal adicionando a classe _.modal-sm_ para modais pequenos (max-width 300px), a classe **_.modal-lg_** para modais grandes (max-width 800px) ou **_.modal-xl_** para modais extra grandes (max -largura 1140px). O padrão é 500px de largura máxima.

<div class=“modal-dialog modal-sm”>

<div class=“modal-dialog modal-lg”>

<div class=“modal-dialog modal-xl”>

  

**Dica quente para você não esquecer**

**Modelos**

O Bootstrap possui muitos modelos e exemplos que podemos utilizar como base para construir páginas web. A seguir alguns sites de onde encontrar:

●        [](https://getbootstrap.com/docs/5.1/examples/)[https://getbootstrap.com/docs/5.1/examples/](https://getbootstrap.com/docs/5.1/examples/)

●        [](https://www.w3schools.com/bootstrap5/bootstrap_templates.php)[https://www.w3schools.com/bootstrap5/bootstrap_templates.php](https://www.w3schools.com/bootstrap5/bootstrap_templates.php)

●         [](https://themes.getbootstrap.com/)[https://themes.getbootstrap.com/](https://themes.getbootstrap.com/)

●      _Bootstrap_ requer o uso do **_doctype_** HTML5. Sem ele, você verá um estilo incompleto. Por isso, certifique-se de ter suas páginas configuradas com os mais recentes padrões de design e desenvolvimento. Isso significa usar um **_doctype_** HTML5 e incluir uma **_meta tag_ _viewport_** para comportamentos responsivos adequados.

●      As imagens do carrossel e dos cards devem ter todas o mesmo tamanho para ficar harmônico.

  

**Conteúdo** **Bônus**

Para aprofundar seus conhecimentos em CSS e melhorar suas habilidades de programação, sugiro que você busque o curso gratuito “HTML, CSS, and Javascript for Web Developers” (HTML, CSS e Javascript para desenvolvedores web) no site Coursera. O curso é ministrado pelo Professor Yaakov Chaikin, da Universidade Johns Hopkins.

Nesse curso, você vai aprender como usar o Bootstrap, uma biblioteca de CSS e Javascript, para desenvolver sites responsivos. O curso também oferece exercícios de codificação para que você possa colocar em prática o que aprendeu. Além disso, aborda detalhadamente como usar o CSS e o JavaScript para adicionar funcionalidades interativas aos sites, como o carrossel e os cartões que foram mencionados no texto**.** A inscrição e a conclusão do curso são gratuitas, mas se você quiser obter um certificado de conclusão, pode haver um custo associado.

  

  

**Referência Bibliográfica**

BUILD fast, responsive sites with Bootstrap. [_S. l._], 20 set. 2022. Disponível em: [https://getbootstrap.com/](https://getbootstrap.com/). Acesso em: 20 set. 2022.

  

**Atividade Prática 13**

**- Avançando com BootStrap**  

**Título da Prática:** Explorando Recursos Avançados com Bootstrap

**Objetivos:** O objetivo dessa atividade prática é permitir que os alunos coloquem em prática os conceitos aprendidos na aula sobre HTML, CSS e Bootstrap, especificamente focando em componentes avançados do Bootstrap, como o Carousel, Cartões (cards) e Modais.

**Materiais, Métodos e Ferramentas:** Um editor de texto de sua escolha (ex: Visual Studio Code, Sublime Text, Atom, etc.), navegador web e Bootstrap (Você pode linkar o Bootstrap via CDN ou fazer o download da biblioteca para o seu projeto).

  

**Atividade Prática**

Você foi designado para desenvolver uma página web responsiva utilizando o Bootstrap, com foco nos componentes avançados mencionados na aula. Siga as instruções abaixo para completar a atividade.

Instruções:

a) Crie um novo arquivo HTML chamado “avancando-bootstrap.html”.

b) Importe o CSS do Bootstrap em seu documento HTML. Você pode usar o CDN ou baixar os arquivos CSS localmente.

c) Crie um layout básico utilizando a estrutura de container, row e col do Bootstrap.

d) Implemente os seguintes componentes do Bootstrap:

      1) Carousel:

●     Crie um Carousel com pelo menos 3 slides.

●     Adicione imagens e texto de sua escolha em cada slide.

●     Inclua indicadores e controles para navegar entre os slides.

      2) Cartões (cards):

●     Crie três cartões com diferentes conteúdos e estilos.

●     Utilize classes como .card, .card-header, .card-body, .card-footer, .card-title, .card-text, .card-link, .card-img-top, etc.

●     Explore diferentes opções de personalização, como cores de fundo e tamanhos.

      3) Modal:

●     Crie um botão que, ao ser clicado, abre um modal com um cabeçalho, corpo e rodapé.

●     Personalize o conteúdo do modal com informações de sua escolha.

●     Adicione um botão para fechar o modal.

e) Adicione seu próprio estilo CSS para personalizar os componentes, se desejar.

  

**Resolução**

Nesta atividade, exploramos três recursos avançados do Bootstrap: Carousel, Cards e Modal. O código fornecido contém a estrutura básica do HTML e as instruções para cada recurso. Basta seguir as instruções, copiando e colando o código no local adequado dentro do arquivo HTML.

O recurso Carousel cria um carrossel de slides, permitindo que você crie uma apresentação visual atraente. Você deve definir as imagens desejadas dentro do elemento div com a classe “carousel-item”. Utilize a classe “active” no primeiro elemento para definir o slide inicial.

O recurso Cards permite criar elementos de cartão flexíveis e estilizados. Você deve criar elementos div com a classe “card” e dentro deles adicionar o conteúdo desejado utilizando as classes apropriadas, como “card-header”, “card-body” e “card-footer”.

O recurso Modal adiciona caixas de diálogo flutuantes que podem ser acionadas por um botão. Você deve definir o botão com a classe “btn” e adicionar os atributos “data-bs-toggle” e “data-bs-target” para controlar a abertura do modal. Dentro do modal, você pode adicionar o cabeçalho, corpo e rodapé da janela de diálogo.

Ao concluir as etapas acima, você terá criado uma página web com os recursos de Carousel, Cards e Modal utilizando o Bootstrap. Utilize o navegador web para abrir o arquivo “atividade.html” e verifique o funcionamento dos recursos implementados.

Lembre-se de que esta é apenas uma sugestão de resolução e você pode personalizar sua página conforme desejado, adicionando mais slides ao Carousel, modificando o conteúdo dos Cards e ajustando o estilo do Modal.

Ir para exercício
```

[[12 - SITES COM BASE EM MODELO]]