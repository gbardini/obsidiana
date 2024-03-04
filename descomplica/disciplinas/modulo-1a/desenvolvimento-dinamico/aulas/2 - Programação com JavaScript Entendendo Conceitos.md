Professor: Marcelo Estruc

**Conhecendo o JavaScript e Suas Características:**

JavaScript é uma linguagem de programação amplamente utilizada para o desenvolvimento web, permitindo a criação de interfaces interativas e dinâmicas. Aqui estão algumas características essenciais do JavaScript:

1. **Linguagem Interpretada:**
    
    - JavaScript é uma linguagem interpretada, executada diretamente pelos navegadores sem a necessidade de compilação prévia. Isso proporciona rapidez no ciclo de desenvolvimento.
2. **Linguagem Baseada em Protótipos:**
    
    - Ao contrário das linguagens baseadas em classes, JavaScript utiliza protótipos para herança. Objetos podem herdar propriedades diretamente de outros objetos, permitindo uma flexibilidade única.
3. **Tipagem Dinâmica:**
    
    - JavaScript é uma linguagem de tipagem dinâmica, o que significa que o tipo de uma variável é determinado em tempo de execução. Isso oferece mais flexibilidade, mas também exige atenção ao lidar com diferentes tipos de dados.
4. **Gerenciamento de Memória Automático:**
    
    - JavaScript possui um coletor de lixo (garbage collector) que gerencia automaticamente a alocação e liberação de memória. Isso simplifica a vida do desenvolvedor, mas é importante compreender seus princípios para evitar vazamentos de memória.
5. **Sincronia e Assincronia:**
    
    - JavaScript é projetado para ser não bloqueante e assíncrono. A utilização de callbacks, Promises e, mais recentemente, async/await, permite a execução de operações assíncronas de forma eficiente.
6. **Manipulação do DOM:**
    
    - JavaScript é frequentemente usado para manipular o DOM, representando a estrutura da página HTML. Essa manipulação dinâmica permite a criação de interfaces interativas e atualizações em tempo real.
7. **Funções de Ordem Superior:**
    
    - Funções em JavaScript são cidadãs de primeira classe e podem ser atribuídas a variáveis, passadas como argumentos e retornadas por outras funções. Isso facilita a implementação de funções de ordem superior.
8. **Expressividade e Flexibilidade:**
    
    - JavaScript oferece uma sintaxe expressiva e flexível, permitindo diferentes estilos de programação. Suporta programação orientada a objetos, funcional e procedural.
9. **Ecossistema Vibrante:**
    
    - JavaScript possui um ecossistema robusto de bibliotecas e frameworks, como React, Angular e Vue.js, que simplificam o desenvolvimento de aplicações web complexas.
10. **Multiplataforma:**
    
    - JavaScript não está restrito a navegadores; com o Node.js, é possível desenvolver aplicações server-side, estendendo o uso da linguagem para o desenvolvimento em larga escala.

Compreender essas características é fundamental para se tornar proficientemente em JavaScript. A natureza versátil da linguagem a torna essencial no mundo do desenvolvimento web moderno.
![[conceitos-gerais.png]]![[nucleo-js.png]]![[js-nao-eh-java.png]]![[js-vs-java.png]]![[ecmascript.png]]
Ecmascript são formas de escrever javascript.

JavaScript, como linguagem de programação, possui uma estrutura que inclui diversos elementos e conceitos essenciais. Vamos destrinchar a estrutura da linguagem para um entendimento mais abrangente:

1. **Variáveis e Tipos de Dados:**
	* JavaScript é de tipagem dinâmica, permitindo declarar variáveis sem especificar seu tipo. Os principais tipos de dados incluem Number, String, Boolean, Object, Array e Null.
	- Exemplo:
	javascript
```javascript
let nome = "John";
let idade = 25;
let ativo = true;
```

2. **Operadores:**
	- JavaScript suporta uma variedade de operadores, como aritméticos (+, -, *, /), de comparação `(==, ===, !=, !==), lógicos (&&, ||, !) e de atribuição (=).`
	- Exemplo:
	javascript
```javascript
let resultado = (idade > 18) ? "Maior de idade" : "Menor de idade";
```

3. **Estruturas de Controle:**
	- Incluem estruturas condicionais (if, else if, else), loops (for, while, do-while), e switch-case para controle de fluxo em programas JavaScript.
	* Exemplo:
	javascript
```javascript
if (idade >= 18) {
    console.log("Pode votar");
} else {
    console.log("Não pode votar");
}
```

4. **Funções:**
	- Funções são blocos de código reutilizáveis. Podem ser declaradas usando a palavra-chave `function` e podem ou não retornar valores.
	* Exemplo:
	javascript
```javascript
function saudacao(nome) {
    return "Olá, " + nome + "!";
}

let mensagem = saudacao("Alice");
```

5. **Objetos e Arrays:**
	- Objetos e arrays são estruturas de dados fundamentais. Objetos contêm propriedades e métodos, enquanto arrays são coleções ordenadas de valores.
	* Exemplo:
	javascript
```javascript
let pessoa = {
    nome: "Carlos",
    idade: 30,
    saudacao: function() {
        return "Olá, eu sou " + this.nome + ".";
    }
};

let frutas = ["Maçã", "Banana", "Laranja"];
```

6. **Escopo de Variáveis:**
	- O JavaScript tem escopo de variáveis global e local. A palavra-chave `let` é usada para declarar variáveis com escopo de bloco.
	* Exemplo:
	javascript
```javascript
function exemploEscopo() {
    let local = "Esta variável é local";
    if (true) {
        let outraLocal = "Esta também é local";
    }
    // 'outraLocal' não está acessível aqui.
}
```

7. **Eventos e Callbacks:**
	- JavaScript é frequentemente usado para manipular eventos do usuário, como cliques e teclas pressionadas. Isso é feito utilizando callbacks.
	* Exemplo:
	javascript
```javascript
document.getElementById("botao").addEventListener("click", function() {
    alert("Botão clicado!");
});
```

8. **Promises e Async/Await:**
	- JavaScript introduziu Promises para lidar com operações assíncronas. O ES2017 introduziu o Async/Await, simplificando ainda mais o código assíncrono.
	* Exemplo:
	javascript
```javascript
function fetchData() {
    return new Promise((resolve, reject) => {
        // Lógica assíncrona
        if (sucesso) {
            resolve(dados);
        } else {
            reject(erro);
        }
    });
}

async function processaDados() {
    try {
        let dados = await fetchData();
        console.log(dados);
    } catch (erro) {
        console.error(erro);
    }
}
```


#estrutura-da-linguagem-javascript
![[sintaxe-de-comandos.png]]![[comentario-js.png]]
![[variaveis-js.png]]![[sintaxe-js.png]]![[sintaxe-js-2.png]]![[sintaxe-js-const.png]]

Ao trabalhar com JavaScript, há várias abordagens e ambientes nos quais você pode desenvolver e executar código. Vamos explorar algumas formas comuns de trabalhar com JavaScript:

1. **Navegador (Client-Side):**
	- **Desenvolvimento Local:** Escrever código JavaScript diretamente em arquivos HTML e executá-los em um navegador local. É útil para prototipagem e desenvolvimento rápido.
	- **Ferramentas de Desenvolvedor:** Utilizar as ferramentas de desenvolvedor do navegador (por exemplo, Chrome DevTools) para depurar, analisar e otimizar código JavaScript em tempo real.
2. **Node.js (Server-Side):**
	- **Desenvolvimento Server-Side:** Utilizar o Node.js para desenvolver aplicativos server-side com JavaScript. Isso inclui a construção de servidores web, APIs e outras aplicações.
3. **Frameworks e Bibliotecas:**
	- **Utilizar Frameworks Front-End:** Frameworks como React, Angular e Vue.js facilitam a construção de interfaces de usuário dinâmicas, simplificando o gerenciamento do DOM e o estado da aplicação.
4. **Ferramentas de Build e Gerenciadores de Pacotes:**
    - **Webpack e Babel:** Utilizar ferramentas de build como Webpack e transpiladores como Babel para otimizar e empacotar código JavaScript, bem como oferecer suporte a funcionalidades mais recentes do ECMAScript.
    - **npm e Yarn:** Utilizar gerenciadores de pacotes como npm (Node Package Manager) ou Yarn para instalar, gerenciar e compartilhar bibliotecas e dependências em projetos JavaScript.
5. **Integração com APIs e Serviços Externos:**
    - **Consumir APIs:** Usar JavaScript para fazer requisições a APIs externas e integrar dados em aplicativos web.
6. **Desenvolvimento em Nuvem (Serverless):**
	- **Serviços Serverless:** Utilizar plataformas serverless, como AWS Lambda ou Azure Functions, para hospedar e executar funções JavaScript sem a necessidade de gerenciar infraestrutura.
7. **Testes e Automação:**
    - **Jest e Mocha:** Utilizar frameworks de teste como Jest ou Mocha para escrever e automatizar testes unitários e de integração.
    - **Ferramentas de Automação:** Incorporar ferramentas como Gulp ou Grunt para automatizar tarefas de desenvolvimento, como compilação, minificação e otimização de código.

Essas são algumas das formas comuns de trabalhar com JavaScript, abrangendo desde o desenvolvimento local até a construção de aplicações server-side, integração com frameworks e serviços, e a automação de processos de desenvolvimento. A escolha da abordagem dependerá dos requisitos específicos do projeto e das preferências da equipe de desenvolvimento.

[[2 - Leitura Programação com JavaScript Entendendo Conceitos]]
[[3 - Programando com javascript primeiros comandos]]