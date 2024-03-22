## Padrão JSON

![[padrao-json.png]]
![[json.png]]
![[metodos-json.png]]

Examples:

```javascript
// Criando objeto pessoa

const pessoa = {

nome: 'Joao',

idade: 25,

profissao: 'Desenvolvedor'

}

  

// Convertendo objeto para JSON

const pessoaJson = JSON.stringify(pessoa);

console.log(pessoa);

console.log(pessoaJson);

  
  

// Convertendo JSON para objeto

const pessoaObj = JSON.parse(pessoaJson);

console.log(pessoaObj);
```

[[16 - LEITURA MANIPULACAO DE JSON]]