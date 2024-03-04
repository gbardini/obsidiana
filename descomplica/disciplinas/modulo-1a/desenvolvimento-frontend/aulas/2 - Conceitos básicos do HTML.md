Professora: Lívia Gouvêa

#html
HTML, que significa "Hypertext Markup Language" (Linguagem de Marcação de Hipertexto, em português), é a linguagem padrão utilizada para criar e projetar páginas web. Criada em 1991 pelo britânico Tim Berners-Lee e mantida pelo World Wide Web Consortium (W3C), o HTML permite a criação de documentos estruturados que incluem títulos, parágrafos, listas, links, imagens e outros elementos. Esses documentos podem ser interpretados por navegadores da web, que exibem o conteúdo conforme a estrutura definida no HTML.

O HTML utiliza uma sintaxe de marcação, onde os elementos são cercados por tags que indicam como o conteúdo deve ser estruturado. Por exemplo, para criar um parágrafo em HTML, você usaria a seguinte estrutura:

```html
<p>Este é um parágrafo de exemplo.</p>`
```
Além do HTML, o desenvolvimento web muitas vezes envolve o uso de outras tecnologias, como CSS (Cascading Style Sheets) para estilizar o conteúdo e JavaScript para adicionar interatividade. Juntos, essas tecnologias formam a base para a criação de páginas web modernas e dinâmicas.

![[elementos-essenciais-html.png]]
1. **`<!DOCTYPE html>`**: Esta é a declaração do tipo de documento HTML e deve ser o primeiro elemento no documento HTML. Ela informa ao navegador que a página está utilizando a versão mais recente do HTML.
2. **`<html>`**: O elemento `<html>` é o contêiner principal que envolve todo o conteúdo da página.
3. **`<head>`**: Este elemento contém informações sobre o documento, como metadados, links para folhas de estilo, scripts, e o título da página.
4. **`<body>`**: O elemento `<body>` contém o conteúdo principal da página, como texto, imagens, links, formulários, etc.
5. **`<h1>, <h2>, ..., <h6>`**: Essas tags são usadas para definir cabeçalhos de diferentes níveis. `<h1>` é o maior e `<h6>` é o menor.
6. **`<p>`**: Essa tag é usada para definir parágrafos de texto.
7. **`<a>`**: A tag `<a>` é usada para criar links.
8. **`<img>`**: Esta tag é usada para incorporar imagens na página.

#elementos-semanticos
Os elementos semânticos em HTML5 refere-se ao uso de tags HTML de maneira significativa e descritiva para estruturar e apresentar o conteúdo de uma página web. A introdução do HTML5 trouxe consigo uma série de novas tags e atributos que visam melhorar a clareza do código, facilitar a leitura por humanos e máquinas, e promover uma estrutura mais significativa para os motores de busca. Aqui estão algumas das principais tags semânticas em HTML5:

1. **`<header>`**: Utilizada para definir o cabeçalho da página ou de uma seção. Pode conter logotipos, títulos, links de navegação, etc.
```html
<header>
    <h1>Meu Site</h1>
    <nav>
        <ul>
            <li><a href="#">Página Inicial</a></li>
            <li><a href="#">Sobre</a></li>
            <li><a href="#">Contato</a></li>
        </ul>
    </nav>
</header>
```

2. **`<nav>`**: Define uma seção de navegação. Geralmente utilizado dentro do elemento `<header>`.
```html
<nav>
    <ul>
        <li><a href="#">Página Inicial</a></li>
        <li><a href="#">Sobre</a></li>
        <li><a href="#">Contato</a></li>
    </ul>
</nav>
```

3. **`<main>`**: Indica o conteúdo principal da página. Ajuda a separar o conteúdo principal de cabeçalhos, rodapés e barras laterais.
```html
<main>
    <h1>Artigo Principal</h1>
    <p>Conteúdo principal da página.</p>
</main>
```

4. **`<article>`**: Utilizada para representar um conteúdo independente e autossuficiente, como um artigo ou post de blog.
```html
<article>
    <h2>Meu Primeiro Artigo</h2>
    <p>Conteúdo do artigo...</p>
</article>
```

5. **`<section>`**: Define seções em um documento, geralmente agrupando conteúdos relacionados.
```html
<section>
    <h2>Seção 1</h2>
    <p>Conteúdo da Seção 1...</p>
</section>
<section>
    <h2>Seção 2</h2>
    <p>Conteúdo da Seção 2...</p>
</section>
```

6. **`<aside>`**: Representa conteúdo relacionado ao conteúdo ao redor, como barras laterais, anúncios ou informações adicionais.
```html
<aside>
    <h3>Barra Lateral</h3>
    <p>Conteúdo relacionado...</p>
</aside>
```

7. **`<footer>`**: Utilizado para definir o rodapé da página ou de uma seção. Pode conter informações de copyright, links de contato, etc.
```html
<footer>
    <p>&copy; 2024 Meu Site</p>
    <p>Contato: <a href="mailto:contato@meusite.com">contato@meusite.com</a></p>
</footer>
```

Ao utilizar essas tags semânticas, você não apenas melhora a estrutura e legibilidade do seu código, mas também fornece informações mais precisas sobre a hierarquia e o propósito dos diferentes elementos na página. Isso é valioso para a acessibilidade, SEO (Search Engine Optimization) e manutenção a longo prazo do seu site.
![[elementos-semanticos.png]]
[[2 - Leitura Conceitos básicos do HTML]]
[[3 - Midia com HTML]]