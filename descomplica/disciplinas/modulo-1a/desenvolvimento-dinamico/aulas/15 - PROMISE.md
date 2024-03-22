Promise is used to consume an external API.

```javascript
const minhaPromise = new Promise((resolve,reject)) => {
	const success = true;

	if (success) {
		resolve("Deu bom!");
	} else {
		reject("Ocorreu um problema!");
	}
})

minhaPromise
.then((resultado) => {
	console.log("Foi sucesso: " + resultado);
})
.catch((erro) => {
console.log("Deu ruim: " + erro);
})
```

More examples:

```javascript
function somarArray(array) {
	return new Promise((resolve, reject) => {
		if (!Array.isArray(array)) {
			reject("O argumento passado nao eh um array");
		}
		const soma = array.reduce((total, num) => total + num,0);
		resolve(soma);
	})
}

const myArray = [1,2,3,4,5]
somarArray(myArray)
.then((resutado) => {
	console.log("A soma dos elementos eh: " + resultado);
})
.catch((erro) => {
	console.log(erro);
})
```

More examples Promises with Classes:

```javascript
class MinhaClasse{

	constructor(valor) {
		this.valor = valor;
	}

	operacaoAssincrona() {
		return new Promise((resolve, reject) => {

			const resultado = this.valor * 2;

			if (resultado >= 0) {
				resolve(resultado);
			} else {
				reject("O resultado eh negativo");
			}
			
		})
	}
}

const primeiraClasse = new MinhaClasse(5)

primeiraClasse.operacaoAssincrona()
.then((resultado) => {
	console.log(resultado);
})
.catch((erro) => {
	console.log(erro);
})
```

More examples:

```javascript
function obterValor(valor) {
	return new Promise((resolve, reject) => {
		if (!valor > 10) {
			reject("O valor informado nao eh maior que 10");
		}
		valor += 1;
		resolve(valor);
	})
}

function dobrarValor(valor) {
	return valor * 2;
}

function adicionar10(valor) {
	return valor += 10;
}
```

[[15 - LEITURA PROMISE]]