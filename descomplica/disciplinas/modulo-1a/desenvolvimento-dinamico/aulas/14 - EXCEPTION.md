![[exception.png]]

Exemplo de código:

```javascript
function divisao(a, b) {

if (b === 0) {

throw new Error("Divisao por zero nao eh permitido!");

}

return a / b;

}

  

try{

const resultado = divisao(10,0)

console.log("Resultado: " + resultado)

} catch(error) {

console.log("Ocorreu uma excecao: " + error.message)

}
```

Exemplo de código com callback:
```javascript
function processName(nome,callback) {

if (typeof nome !== "string") {

callback(new Error("O nome tem que ser uma string."));

}

if (nome.length === 0) {

callback(new Error("O nome nao pode ser vazio."));

}

  

callback(null, "O nome foi processado com sucesso");

}

  

processName("Gabriel",(error,result) => {

if (error) {

console.log("Ocorreu um erro na operacao: ", error.message)

} else {

console.log(result);

}

})
```

[[14 - LEITURA EXCEPTION]]