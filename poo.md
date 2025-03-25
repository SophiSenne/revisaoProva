# Questões POO

1. **Questão 3 - Programação Orientada a Objetos (POO)**

Considere a seguinte definição de classes:

```javascript
class Animal {
  constructor(nome) {
    this.nome = nome;
  }

  falar() {
    return `${this.nome} faz um som.`;
  }
}

class Cachorro extends Animal {
  falar() {
    return `${this.nome} late.`;
  }
}
```

O que será impresso no console com o código abaixo?

```javascript
let rex = new Cachorro("Rex");
console.log(rex.falar());
```

A) `Rex faz um som.`  
B) `undefined late.`  
C) `Rex late.`  
D) `Cachorro late.`  
E) Erro de execução

**Resposta correta:** C  

--- 

2. **Questão 4 - POO com `super`**

Analise o seguinte código:

```javascript
class Pessoa {
  constructor(nome) {
    this.nome = nome;
  }

  saudacao() {
    return `Olá, meu nome é ${this.nome}`;
  }
}

class Aluno extends Pessoa {
  constructor(nome, curso) {
    super(nome);
    this.curso = curso;
  }

  saudacao() {
    return `${super.saudacao()} e estudo ${this.curso}`;
  }
}
```

Qual será a saída de `console.log(new Aluno("Lucas", "JS Avançado").saudacao());`?

A) `Olá, meu nome é Lucas`  
B) `Olá, meu nome é Lucas e estudo JS Avançado`  
C) `Lucas estuda JS Avançado`  
D) `Lucas`  
E) Erro, pois `super` não pode ser usado assim

**Resposta correta:** B  

---

3. **Questão 5 - POO: Métodos Estáticos e Instâncias**

Considere o seguinte código JavaScript:

```javascript
class Calculadora {
  constructor(num1, num2) {
    this.num1 = num1;
    this.num2 = num2;
  }

  somar() {
    return this.num1 + this.num2;
  }

  static multiplicar(a, b) {
    return a * b;
  }
}
```

Analise os seguintes trechos de código:

I.  
```javascript
let c = new Calculadora(10, 5);
console.log(c.somar());
```

II.  
```javascript
console.log(Calculadora.multiplicar(4, 3));
```

III.  
```javascript
let c = new Calculadora(2, 3);
console.log(c.multiplicar());
```

Assinale a alternativa correta:

A) Apenas o trecho I está correto.  
B) Apenas os trechos I e II estão corretos.  
C) Apenas os trechos II e III estão corretos.  
D) Todos os trechos estão corretos.  
E) O trecho III está correto, pois o método estático pode ser chamado pela instância.

**Resposta correta:** **B**
