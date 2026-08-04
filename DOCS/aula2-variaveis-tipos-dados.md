## 1. Declaração de Variáveis

Uma variável é um espaço na memória do computador com um nome (etiqueta) associado. Em JavaScript moderno, utilizamos três palavras-chave principais para criar variáveis:

*   **`let`**: Cria uma variável cujo valor **por ser alterado** (mutável) ao longo da execução do programa.
*   **`const`**: Cria uma constante cujo valor **não pode ser alterado** (imutável) após a primeira atribuição.
*   **`var`**: Forma antiga de declarar variáveis. Evite utilizá-la, pois possui problemas de escopo que podem gerar comportamentos inesperados no código.

### Exemplos Práticos:

```javascript
// Criando variáveis mutáveis
let idade = 25;
idade = 26; // Permitido: o valor foi atualizado de 25 para 26

// Criando constantes imutáveis
const pixChave = "usuario@email.com";
// pixChave = "outro@email.com"; // Erro! O JavaScript impede a reatribuição de uma const
```

---

## 2. Tipos de Dados Primitivos

Mesmo que o JavaScript identifique os tipos de forma automática, cada valor pertence a uma categoria específica. Os principais tipos primitivos são:

### 🔢 Number
Representa qualquer tipo de número, seja ele inteiro, negativo ou decimal (chamado de ponto flutuante). Ao contrário de outras linguagens, o JavaScript não separa inteiros de decimais em tipos diferentes.

```javascript
let quantidadeItens = 12; // Número inteiro
let precoProduto = 49.99;  // Número decimal (usa-se ponto como separador)
let temperatura = -5;      // Número negativo
```

### 🔤 String
Representa sequências de caracteres (textos). Podem ser delimitadas por aspas duplas (`""`), aspas simples (`''`) ou crases (`` ``). Textos envolvidos em crases são chamados de *Template Strings* e permitem interpolar (injetar) variáveis diretamente no texto usando a sintaxe `${}`.

```javascript
let nome = "Ana";
let profissao = 'Desenvolvedora';
let saudacao = `Olá, meu nome é ${nome} e eu sou ${profissao}.`; 
// Resultado de saudacao: "Olá, meu nome é Ana e eu sou Desenvolvedora."
```

### ⚖️ Boolean
Representa um valor lógico que pode assumir apenas dois estados: verdadeiro (`true`) ou falso (`false`). É a engrenagem principal para estruturas de tomada de decisão (condicionais).

```javascript
let usuarioLogado = true;
let possuiDesconto = false;
```

### 🫙 Undefined e Null
São dois tipos distintos utilizados para indicar a ausência de valor:

*   **`undefined`**: Significa que a variável foi declarada, mas nenhum valor foi atribuído a ela ainda. O próprio sistema define este estado.
*   **`null`**: É uma atribuição intencional feita pelo programador para indicar que a variável está vazia ou não possui valor nenhum.

```javascript
let respostaDoServidor; // Valor atual: undefined
let carrinhoDeCompras = null; // Valor atual: null (limpo intencionalmente)
```

---

## Summary (Resumo de Atribuição Dinâmica)

A tipagem dinâmica permite que uma mesma variável declarada com `let` mude de tipo caso receba um novo valor, embora mudar o tipo radicalmente de uma mesma variável não seja considerado uma boa prática de escrita:

```javascript
let dados = 100;      // O tipo atual é Number
dados = "Cem reais";  // Agora o tipo mudou para String
```
