Professora: Lívia Gouvêa
## Mídia com HTML
[[4 - Montando tabelas com HTML]]
**Introdução**  

Com o surgimento da web, o HTML se consolidou como a principal linguagem utilizada para a publicação de conteúdo na internet. Em termos gerais, o HTML é fundamentado no conceito de hipertexto, que consiste em conjuntos de elementos interligados por conexões, como palavras, imagens, vídeos, áudio, documentos, entre outros. Quando esses elementos são conectados, formam uma ampla rede de informações.

O HTML tem como objetivo primordial estruturar o conteúdo de uma página web, permitindo a criação de diversos tipos de links para outras páginas e arquivos, além de possibilitar a construção de formulários, tabelas, listas e mais. Quando visitamos um site e clicamos em uma página, estamos, essencialmente, acessando um documento HTML.

  

**Objetivos da aula**

●      Empregar Imagens em documentos HTML

●      Usar Vídeos em documentos HTML

●      Demonstrar Listas em documentos HTML

  

**Resumo**

**Como inserir imagens na página HTML**

A tag _<img>_ é usada para incorporar uma imagem em uma página da web. A sintaxe é <img src=”url” alt=”Texto alternativo”>. Este elemento não possui _tag_ de fechamento e possui dois atributos obrigatórios:

●     src: é o diminutivo de _source_ e deve receber o caminho para a imagem

●     alt é o diminutivo de _alternative_ e deve receber um texto alternativo para a imagem

  

**Como inserir vídeos na página HTML**

Para inserir um vídeo em uma página HTML utiliza-se a seguinte sintaxe:

<video width=“320”  height=“240” controls>  
    <source src=“movie.mp4”  type=“video/mp4”>  
    <source src=“movie.ogg”  type=“video/ogg”>  
    Seu navegador não suporta a exibição  deste vídeo  
  </video> 

Nessa estrutura, o elemento “source” é equipado com os atributos “src” e “type”, os quais especificam a localização e o formato do arquivo de vídeo, respectivamente. É viável definir múltiplos elementos “source” com diversos tipos de vídeo. O navegador dará preferência ao primeiro formato que seja reconhecido; caso nenhum seja suportado, será exibida a mensagem inserida ao final (Seu navegador não suporta a exibição deste vídeo).

O atributo “controls” desempenha a função de adicionar controles de vídeo, como play, pause e volume. Outros atributos podem ser empregados no controle do vídeo, tais como “muted” para iniciar o vídeo sem áudio e “autoplay” para fazê-lo iniciar automaticamente quando a página carrega. Também é possível estabelecer a altura (height) e a largura (width) da tag “video”; é aconselhável sempre realizar essas definições.

  

**Como apresentar conteúdo em listas**

Existem 3 formas de se exibirem listas em HTML:

1.   <ul>: Representa _unordered list_, ou seja, listas não ordenadas;

2.   <ol>: Representa _ordered list_, ou seja, listas ordenadas;

3.   <dl>: Representa _description list_, ou seja, listas de descrição

Para as listas ordenadas e não ordenadas, os itens são definidos pela tag <li> e a sintaxe final fica desta forma:

<ul>  
           <li>Primeiro  item</li>  
           <li>Segundo  item</li>  
           <li>Terceiro  item</li>  
  </ul>  
   
<ol>  
           <li>Primeiro  item</li>  
           <li>Segundo item</li>  
           <li>Terceiro  item</li>  
  </ol>

Para a lista de descrição utiliza-se as _tags_ <dt> para definição de termo e <dd> para descrição de termo e a sintaxe fica como a seguir:

<dl>  
           <dt>Primeiro  item</dt>  
           <dd>-  Descrição do primeiro item</dd>  
           <dt>Segundo  item</dt>  
           <dd>-  Descrição do segundo item</dd>  
  </dl>

  

**Conteúdo Bônus**

Recomendo o tutorial chamado “HTML Tutorial”, que pode ser encontrado no site W3Schools. Ele oferece um guia completo sobre HTML, abrangendo desde os conceitos básicos até tópicos mais avançados. O tutorial é gratuito e pode ser encontrado pesquisando diretamente no navegador utilizando os termos “HTML Tutorial W3Schools”.

  

**Dica quente para você não esquecer**

Nem todos os navegadores suportam os mesmos formatos de vídeo; por isso, você pode fornecer várias fontes em elementos _<source>_ dentro do elemento _<video>_, e o navegador usará a primeira que achar compatível.

  

  

**Referência Bibliográfica**

RESOURCES for Developers, by Developers. [_S. l._], 20 set. 2022. Disponível em: [https://developer.mozilla.org/pt-BR](https://developer.mozilla.org/pt-BR)/. Acesso em: 20 set. 2022.

  

**Atividade Prática 3**: Mídia com HTML  

**Título da Prática:** Criação de Página Web com Mídia Integrada

**Objetivo:** O objetivo desta atividade é permitir que os alunos apliquem os conceitos aprendidos na aula “Mídia com HTML”, criando uma página web que incorpora imagens, vídeos e listas.

  

**Materiais, Métodos e Ferramentas:**

1.   Computador com acesso à internet

2.   Editor de texto (como o Sublime Text, Atom, Visual Studio Code, etc.)

3.   Navegador web para visualização do resultado (como Google Chrome, Firefox, etc.)

  

**Atividade Prática**

**1º passo:** Crie uma nova página HTML chamada “media.html”.

**2º passo:** Na página, você deve incorporar uma imagem de sua escolha usando a tag <img>. Lembre-se de adicionar o atributo src com o caminho para a imagem e o atributo alt com uma descrição adequada da imagem.

**3º passo:** Adicione um vídeo à página usando a tag <video>. Use os atributos width, height e controls para definir as dimensões do vídeo e adicionar controles de reprodução. Use a tag <source> para especificar o caminho para o arquivo de vídeo e seu tipo. Lembre-se de adicionar uma mensagem para navegadores que não suportam a tag <video>.

**4º passo:** Crie três tipos de listas na página: uma lista não ordenada (<ul>), uma lista ordenada (<ol>) e uma lista de descrição (<dl>). Cada lista deve conter pelo menos três itens.

**5º passo:** Salve seu trabalho e visualize a página no navegador.

  

**Gabarito Atividade Prática**

Aqui está um exemplo de como a página HTML pode ser estruturada:

​  

<!DOCTYPE  html>  
   
<html>  
   
<head>  
   
    <title>Minha Página com  Mídia</title>  
   
</head>  
   
<body>  
   
    <h1>Bem-vindo à minha página com  mídia!</h1>  
   
   
    <h2>Imagem</h2>  
   
    <img  src=“caminho_para_sua_imagem.jpg” alt=“Descrição da  imagem”>  
   
   
    <h2>Vídeo</h2>  
   
    <video width=“320”  height=“240” controls>  
   
        <source  src=“caminho_para_seu_video.mp4” type=“video/mp4”>  
   
        Seu navegador não suporta a exibição  deste vídeo.  
   
    </video>  
   
   
    <h2>Listas</h2>  
   
   
    <h3>Lista não ordenada</h3>  
   
    <ul>  
   
        <li>Item 1</li>  
   
        <li>Item 2</li>  
   
        <li>Item 3</li>  
   
    </ul>  
   
   
    <h3>Lista ordenada</h3>  
   
    <ol>  
   
        <li>Item 1</li>  
   
        <li>Item 2</li>  
   
        <li>Item 3</li>  
   
    </ol>  
   
   
    <h3>Lista de descrição</h3>  
   
    <dl>  
   
        <dt>Termo 1</dt>  
   
        <dd>Descrição do Termo  1</dd>  
   
        <dt>Termo 2</dt>  
   
        <dd>Descrição do Termo  2</dd>  
   
        <dt>Termo 3</dt>  
   
        <dd>Descrição do Termo 3</dd>  
   
    </dl>  
   
</body>  
   
</html>

Lembre-se de substituir “caminho_para_sua_imagem.jpg” e “caminho_para_seu_video.mp4” pelos caminhos corretos para seus arquivos de imagem e vídeo. Além disso, substitua “Descrição da imagem”, “Item 1”, “Item 2”, “Item 3”, “Termo 1”, “Descrição do Termo 1”, etc., com o conteúdo apropriado para sua página.