# Questões Condicionais

Perfeito! Com base nas suas questões anteriores (que abordam **orientação a objetos** e **estrutura condicional/controle de fluxo**) e nos exemplos visuais, aqui vão sugestões de **novas questões para revisão**, todas em **JavaScript**, com foco nos temas solicitados:

---

1. **Questão 1 - Estrutura Condicional (If-Else)**
Você está criando uma função que analisa a temperatura para indicar o estado da água:

```javascript
function estadoDaAgua(temperatura) {
  // implemente aqui
}
```

A função deve retornar:

- `"sólido"` se a temperatura for menor que 0,
- `"líquido"` se a temperatura estiver entre 0 (inclusive) e 100 (exclusive),
- `"gasoso"` se a temperatura for igual ou maior que 100.

Assinale a alternativa que representa corretamente essa função:

A)
```javascript
function estadoDaAgua(temperatura) {
  if (temperatura < 0) return "sólido";
  if (temperatura >= 0 && temperatura < 100) return "líquido";
  return "gasoso";
}
```

B)
```javascript
function estadoDaAgua(temperatura) {
  if (temperatura > 100) return "gasoso";
  else if (temperatura > 0) return "líquido";
  else return "sólido";
}
```

C)
```javascript
function estadoDaAgua(temperatura) {
  switch(temperatura) {
    case temperatura < 0: return "sólido";
    case temperatura < 100: return "líquido";
    default: return "gasoso";
  }
}
```

D)
```javascript
function estadoDaAgua(temperatura) {
  if (temperatura == 0) return "sólido";
  if (temperatura == 100) return "gasoso";
  return "líquido";
}
```

**Resposta correta:** A  

---

2. **Questão 2 - Estrutura Condicional (Switch-Case)**
Implemente uma função que recebe o nome de um dia da semana e retorna se é um **dia útil** ou **fim de semana**.

```javascript
function tipoDeDia(dia) {
  // implementar usando switch
}
```

Exemplo:
```js
tipoDeDia("segunda") ➞ "Dia útil"
tipoDeDia("domingo") ➞ "Fim de semana"
```

Qual das opções implementa corretamente a função `tipoDeDia`?

A)
```javascript
function tipoDeDia(dia) {
  switch(dia) {
    case "sábado":
    case "domingo":
      return "Fim de semana";
    default:
      return "Dia útil";
  }
}
```

B)
```javascript
function tipoDeDia(dia) {
  if (dia === "sábado" || dia === "domingo") {
    return "Fim de semana";
  } else {
    return "Dia útil";
  }
}
```

C)
```javascript
function tipoDeDia(dia) {
  switch(dia) {
    case "segunda": return "Dia útil";
    case "terça": return "Dia útil";
    case "quarta": return "Dia útil";
    case "quinta": return "Dia útil";
    case "sexta": return "Dia útil";
    case "sábado": return "Fim de semana";
    case "domingo": return "Fim de semana";
  }
}
```

D)
```javascript
function tipoDeDia(dia) {
  switch(dia) {
    case "sábado":
    case "domingo":
      return "Fim de semana";
    case "segunda":
    case "terça":
    case "quarta":
    case "quinta":
    case "sexta":
      return "Dia útil";
    default:
      return "Dia inválido";
  }
}
```

**Resposta correta:** D  

