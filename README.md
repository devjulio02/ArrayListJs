# 📘 ArrayListJs

Bem-vindo(a) ao **ArrayListJs**!   
Este projeto foi criado como parte de uma atividade prática para demonstrar o uso dos métodos **map()**, **filter()** e **reduce()** em **JavaScript** — três ferramentas fundamentais para manipulação de listas (arrays).

---

## Objetivo do projeto

O objetivo deste tutorial é ajudar você a compreender **como manipular coleções de dados** em JavaScript de forma moderna e eficiente.  
Vamos entender **o que cada método faz**, **quando usar**, e **ver exemplos práticos**.

---

## O que é um Array?

Um **array** é uma estrutura de dados usada para armazenar vários valores dentro de uma única variável.  
Ele pode conter números, strings, objetos e até outros arrays!

### Exemplo simples:

```js
const numeros = [1, 2, 3, 4, 5];
console.log(numeros); 

//Saída esperada
[1, 2, 3, 4, 5]
```
### O que é o map?

O **método map()** cria um novo array com base no original, aplicando uma função a cada elemento. Pense no map como uma “fábrica”: ele pega cada item, transforma e te entrega um novo array transformado.

### Exemplo:

```js
const numeros = [1, 2, 3, 4, 5];

//Dobra cada número do array
const dobrados = numeros.map(num => num * 2);

console.log("Array original:", numeros);
console.log("Array dobrado:", dobrados);

//Saída esperada
Array original: [1, 2, 3, 4, 5]
Array dobrado: [2, 4, 6, 8, 10]
```
### O que é o filter?
O **método filter()** cria um novo array com apenas os elementos que passam em um determinado teste. Pense no filter como um “porteiro”: ele deixa passar apenas os elementos que atendem à condição.

### Exemplo:

```js
const numeros = [1, 2, 3, 4, 5, 6];

//Filtra apenas os números pares
const pares = numeros.filter(num => num % 2 === 0);

console.log("Números pares:", pares);

//Saída Esperada
Números pares: [2, 4, 6]
```
### O que é o reduce?

O **método reduce()** percorre o array e reduz todos os valores a um único resultado,
ele recebe uma função que acumula valores, somando, multiplicando ou juntando-os conforme necessário. Pense no reduce como um “coletor”: ele pega tudo e transforma em uma coisa só.

### Exemplo:

```js
const numeros = [10, 20, 30, 40];

// Soma todos os números do array
const soma = numeros.reduce((acumulador, valorAtual) => acumulador + valorAtual, 0);

console.log("Soma total:", soma);

//Saída Esperada
Soma total: 100
```
### Exemplo combinado:

```js
const numeros = [5, 10, 15, 20, 25];

// Passo 1: dobrar os números
const dobrados = numeros.map(num => num * 2);

// Passo 2: filtrar os maiores que 20
const filtrados = dobrados.filter(num => num > 20);

// Passo 3: somar todos os filtrados
const somaFinal = filtrados.reduce((acc, val) => acc + val, 0);

console.log("Dobrado:", dobrados);
console.log("Filtrado (>20):", filtrados);
console.log("Soma final:", somaFinal);

//Saída esperada
Dobrado: [10, 20, 30, 40, 50]
Filtrado (>20): [30, 40, 50]
Soma final: 120
```
### Comparando os três métodos

| Método | Retorno | Modifica o original? | Uso principal |
|:-------:|:--------:|:------------------:|:---------------|
| `map()` | Novo array | ❌ Não | Transformar elementos |
| `filter()` | Novo array | ❌ Não | Filtrar elementos |
| `reduce()` | Valor único | ❌ Não | Somar ou combinar valores |

## Autor

**Feito por:** __**Júlio Soares da Silva**__\
**Contato:** __**soares.julio@academico.ifpb.edu.br**__

## Licença

Este projeto está sob a licença **MIT**.