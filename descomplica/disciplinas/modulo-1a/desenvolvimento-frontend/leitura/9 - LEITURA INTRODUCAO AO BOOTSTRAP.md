## Introdução ao Bootstrap

**Introdução**  

O Bootstrap foi desenvolvido com base em HTML5 e CSS3, e foi criado para ajudar os desenvolvedores a criar sites e aplicativos web responsivos e responsivos de maneira rápida e fácil, pois tem um conjunto de componentes reutilizáveis ​​que podem ser usados ​​para criar sites e aplicativos web. Esses componentes são projetados para fornecer um design consistente e uma experiência de usuário unificada para os usuários finais.  

O Bootstrap é uma estrutura de código aberto que pode ser usada livremente por qualquer pessoa. Ele é compatível com todos os navegadores modernos e é facilmente estendido para atender às suas necessidades específicas.

  

**Objetivos da aula**

● Definir o conceito de Bootstrap.

● Descrever a implementação do Bootstrap.

  

**Resumo**

Os desenvolvedores web hoje têm à sua disposição várias estruturas e ferramentas avançadas, que os diferenciam e os colocam à frente de seus colegas de alguns anos atrás. Uma dessas estruturas, que tornou o desenvolvimento web consideravelmente mais simplificado e expandiu a criação para incluir uma melhor experiência móvel, é conhecida como o maior e mais rápido framework de JS, HTML e CSS. Esse framework pode ser usado para construir projetos web interativos e envolventes. Conhecido como Bootstrap, trata-se de uma estrutura de front-end que permite que o desenvolvimento seja mais rápido e simplificado.

Um framework como o Bootstrap pode ser útil para qualquer desenvolvedor web, integrando-se ao seu arsenal técnico de maneira vantajosa.

Simplificando, o Bootstrap é uma enorme coleção de pedaços de código reutilizáveis ​​e versáteis que são escritos em CSS, HTML e JavaScript. Como um framework, ele já estabelece todas as bases para o desenvolvimento web responsivo, permitindo que os desenvolvedores simplesmente insiram o código no sistema de grade pré-definido.

O pacote inclui diversas ferramentas gratuitas que auxiliam os designers na construção dos componentes de interface mais comuns, tornando-os também altamente responsivos e, assim, aumentando a versatilidade do framework.

Normalmente, essa abordagem evita que você tenha que escrever longas strings especialmente de código CSS. Isso lhe dá mais tempo e capacidade para trabalhar no design das próprias páginas da web.

Apesar de você encontrar o Bootstrap no GitHub, você pode encontrá-lo em outros repositórios, como o Bower e o NPM. Além disso, é possível baixar o Bootstrap diretamente do site oficial do projeto.

Quer saber mais?!

● **No GitHub:** O repositório oficial do Bootstrap no GitHub pode ser encontrado em [https://github.com/twbs/bootstrap](https://github.com/twbs/bootstrap). Este é o lugar onde as alterações e atualizações mais recentes do Bootstrap são feitas.

● **No Bower:** O Bootstrap também está disponível no Bower, um gerenciador de pacotes para front-end. Para instalar o Bootstrap com o Bower, execute o seguinte comando: bower install bootstrap

● **No NPM:** O Bootstrap também está disponível no NPM, um gerenciador de pacotes para JavaScript. Para instalar o Bootstrap com o NPM, execute o seguinte comando: npm install bootstrap

●**No site oficial do Bootstrap:** O site oficial do Bootstrap oferece um download do Bootstrap em um arquivo ZIP. Para baixar o Bootstrap do site oficial, acesse [https://getbootstrap.com/](https://getbootstrap.com/) e clique no botão “Download”.

  

**Dica quente para você não esquecer**

As principais diferenças entre o Bootstrap 5 e o Bootstrap 3 e 4 é que o Bootstrap 5 mudou para JavaScript em vez de jQuery" é uma boa maneira de lembrar que o Bootstrap 5 é diferente das versões anteriores, pois não depende do jQuery.

O jQuery é uma biblioteca JavaScript que foi muito popular nos últimos anos. No entanto, o jQuery não é mais necessário para usar o Bootstrap 5. O Bootstrap 5 foi reescrito para usar JavaScript nativo, o que significa que ele é mais leve e mais rápido.

Se você está acostumado a usar o Bootstrap 3 ou 4, é importante estar ciente dessa mudança. Se você estiver desenvolvendo um novo projeto com o Bootstrap 5, precisará aprender a usar o JavaScript nativo para interagir com os componentes do Bootstrap.

  

**Conteúdo Bônus**

Para um aprofundamento nesse tópico, sugiro a leitura da documentação sobre Bootstrap 5. Você pode encontrar a documentação procurando por Bootstrap 5 em seu buscador de preferência ou pelo termo “getbootstrap” que é o nome do site oficial.

  

  

**Referência Bibliográfica**

Build fast, responsive sites with Bootstrap. [_S. l._], 20 set. 2022. Disponível em: [https://getbootstrap.com/](https://getbootstrap.com/). Acesso em: 20 set. 2022.

  

  

**Atividade Prática 09** **- Introdução ao Bootstrap**

**Título da Prática:** Construindo uma Página Responsiva com Bootstrap

**Objetivos:** O objetivo desta atividade prática é reforçar o entendimento dos alunos sobre o uso do framework Bootstrap para criar uma página web responsiva.

**Materiais, Métodos e Ferramentas:** Você precisará de um editor de texto (como Sublime Text, Atom, Visual Studio Code, etc.), um navegador web para visualização e acesso à internet para obter os links necessários para o Bootstrap.

  

**Atividade Prática**

Você deve criar uma página web responsiva usando o Bootstrap. Sua página web deve conter os seguintes componentes:

1. Uma barra de navegação no topo da página com links para diferentes seções da página.

2. Um cabeçalho de página principal que ocupa toda a largura e altura da tela.

3. Uma seção de conteúdo com três colunas de texto.

4. Uma galeria de imagens com pelo menos seis imagens.

5. Um rodapé com informações de contato.

Cada um desses componentes deve ser responsivo e se adaptar a diferentes tamanhos de tela.

Para adicionar o Bootstrap ao seu projeto, você pode usar o link para a versão CSS do Bootstrap em seu arquivo HTML no <head>. Além disso, certifique-se de adicionar os links para o jQuery e o JavaScript do Bootstrap antes do fechamento da tag </body>. Você pode encontrar esses links na página de inicialização rápida do Bootstrap.

  

**Resolução:**

1. Criação do arquivo HTML básico:

```html  
  
<!DOCTYPE html>  
  
<html>  
  
<head>  
  
    <title>Página Responsiva com Bootstrap</title>  
  
    <link rel=“stylesheet” href=“[https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css](https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css)”>  
  
</head>  
  
<body>  
  
    <!-- Aqui vão os componentes da página -->  
  
    <script src=“[https://code.jquery.com/jquery-3.3.1.slim.min.js](https://code.jquery.com/jquery-3.3.1.slim.min.js)”></script>  
  
    <script src=“[https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js](https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js)”></script>  
  
</body>  
  
</html>  
  
```
  
  
2. Adição dos componentes:  
  
    * Barra de Navegação:  
  
    ```html  
  
    <nav class=“navbar navbar-expand-lg navbar-light bg-light”>  
  
        <a class=“navbar-brand” href=“#”>Meu Site</a>  
  
        <button class=“navbar-toggler” type=“button” data-toggle=“collapse” data-target=“#navbarNav” aria-controls=“navbarNav” aria-expanded=“false” aria-label=“Toggle navigation”>  
  
            <span class=“navbar-toggler-icon”></span>  
  
        </button>  
  
        <div class=“collapse navbar-collapse” id=“navbarNav”>  
  
            <ul class=“navbar-nav”>  
  
                <li class=“nav-item”>  
  
                    <a class=“nav-link” href=“#header”>Cabeçalho</a>  
  
                </li>  
  
                <li class=“nav-item”>  
  
                    <a class=“nav-link” href=“#conteudo”>Conteúdo</a>  
  
                </li>  
  
                <li class=“nav-item”>  
  
                    <a class=“nav-link” href=“#galeria”>Galeria</a>  
  
                </li>  
  
            </ul>  
  
        </div>  
  
    </nav>  
  
    ``` 
  
    * Cabeçalho:  
  
    ```html  
  
    <header id=“header” class=“jumbotron jumbotron-fluid”>  
  
        <div class=“container”>  
  
            <h1 class=“display-4”>Bem-vindo ao meu site!</h1>  
  
  
  
            <p class=“lead”>Este é um simples exemplo de um cabeçalho.</p>  
  
        </div>  
  
    </header>  
  
    ```  
  
    * Seção de Conteúdo:  
  
    ```html  
  
    <section id=“conteudo” class=“container”>  
  
        <div class=“row”>  
  
            <div class=“col”>  
  
                <h3>Coluna 1</h3>  
  
                <p>Este é um exemplo de texto para a primeira coluna.</p>  
  
            </div>  
  
            <div class=“col”>  
  
                <h3>Coluna 2</h3>  
  
                <p>Este é um exemplo de texto para a segunda coluna.</p>  
  
            </div>  
  
            <div class=“col”>  
  
                <h3>Coluna 3</h3>  
  
                <p>Este é um exemplo de texto para a terceira coluna.</p>  
  
            </div>  
  
        </div>  
  
    </section>  
  
    ```  
  
    * Galeria de imagens:  
  
    ```html  
  
    <section id=“galeria” class=“container”>  
  
        <div class=“row”>  
  
            <div class=“col-md-4”>  
  
                <img src=“imagem1.jpg” class=“img-fluid” alt=“Imagem 1”>  
  
            </div>  
  
            <!-- repita o bloco acima para cada imagem -->  
  
        </div>  
  
    </section>  
  
    ```  
  
    * Rodapé:  
  
    ```html  
  
    <footer class=“footer bg-light”>  
  
        <div class=“container”>  
  
            <span class=“text-muted”>Entre em contato: [email@example.com](mailto:email@example.com)</span>  
  
        </div>  
  
    </footer>  
  
    ```

3. **Resultado:** Ao abrir o arquivo “index.html” em um navegador, a página HTML criada com Bootstrap será exibida, sendo responsiva a diferentes tamanhos de tela.

**Nota:** Substitua “imagem1.jpg” pelo caminho da imagem desejada no bloco da galeria de imagens. Certifique-se de que as imagens estejam na mesma pasta que o arquivo HTML ou que o caminho esteja correto. Adicione quantos blocos de imagem forem necessários para atingir um mínimo de seis imagens.

Ir para exercício

[[10 - CONTAINERS COM BOOTSTRAP]]