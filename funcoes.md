# Questões Funções

Fiz 4 questões pra gente decidir qual/quais colocar no kahoot

## 1

Essa questão acho que é um pouco mais difícil, mas foi inspirada em uma que causou muita dificuldade ano passado na nossa prova.

1. Qual será a saída desse código?

```javascript
let convidadas = [
    { nome: "Giovanna", idade: 19, confirmado: true },
    { nome: "Kethelen", idade: 20, confirmado: true },
    { nome: "Gabi", idade: 18, confirmado: true },
    { nome: "Anna", idade: 20, confirmado: false }
];


function encontrarConvidadaEspecial (convidados){
    return convidados
        .filter (convidado => convidado.confirmado && convidado.idade >= 20)
        .map(convidado => convidado.nome)[0] || null;
}

console.log(encontrarConvidadaEspecial(convidadas));

```

a) null

b) Kethelen ✅

c) Anna

d) Giovanna

## 2

também peguei essa questão da nossa prova

2. Qual a saída desse trecho de código?

```javascript

function calcularTrajetoria(origem, destino) {
    return destino.subtract(origem);
}

const origem = new Phaser.Math.Vector2(100, 100);
const destino = new Phaser.Math.Vector2(200, 200);
const trajetoria = calcularTrajetoria(origem, destino);

console.log(trajetoria);

```

a) `Vector2 { x: 100, y: 100 }` ✅

b) `{ x: 100, y: 100 }`

c) `Vector2 { x: 300, y: 300 }`

d) `{ x: 300, y: 300 }`


## 3

3. Qual será a saída do código abaixo?  

```javascript
const conta = (x) => x * 2;
console.log(conta(5));
```  

a) `5`  

b) `10` ✅

c) `x * 2`  

d) `Erro`  


## 4

4. O que acontece se uma função não tiver um `return`?  
a) Retorna `undefined` ✅  
b) Retorna `null`  
c) Retorna `0`  
d) Causa um erro  




