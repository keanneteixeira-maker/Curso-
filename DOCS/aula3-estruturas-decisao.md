## 1. O Conceito Base: A Tomada de Decisão

Imagine que você está saindo de casa. A sua lógica mental funciona assim:
> **Se** estiver chovendo, **então** eu pego o guarda-chuva. **Senão**, eu não levo nada.

Na programação, essa análise é feita por meio de testes lógicos cujo resultado é sempre um valor booleano: **Verdadeiro** (`true`) ou **Falso** (`false`).

---

## 2. Tipos de Estruturas de Decisão

As linguagens de programação (como JavaScript, Python, Java, etc.) implementam essas tomadas de decisão por meio de três estruturas principais:

### 🟩 Condicional Simples (`if`)
Executa um bloco de código **apenas se** a condição testada for verdadeira. Se for falsa, o programa ignora o bloco e segue em frente.

```javascript
let velocidade = 90;

if (velocidade > 80) {
    console.log("Você foi multado por excesso de velocidade!");
}
```

### 🟨 Condicional Composta (`if / else`)
Define um caminho alternativo. Executa um bloco de código se a condição for verdadeira e **outro** bloco diferente se a condição for falsa.

```javascript
let idade = 16;

if (idade >= 18) {
    console.log("Acesso permitido. Maior de idade.");
} else {
    console.log("Acesso negado. Menor de idade.");
}
```

### 🟧 Condicional Encadeada (`if / else if / else`)
Utilizada quando existem mais de duas possibilidades de escolha. O programa testa as condições em sequência até encontrar a primeira verdadeira.

```javascript
let nota = 6.5;

if (nota >= 7.0) {
    console.log("Aprovado direto!");
} else if (nota >= 5.0) {
    console.log("Recuperação.");
} else {
    console.log("Reprovado.");
}
```

---

## 3. Seleção Múltipla (`switch / case`)

Quando temos uma única variável que precisa ser comparada com vários valores exatos e específicos, a estrutura `switch` deixa o código mais limpo do que vários `if / else if` seguidos.

```javascript
let opcaoMenu = 2;

switch (opcaoMenu) {
    case 1:
        console.log("Iniciando o jogo...");
        break;
    case 2:
        console.log("Abrindo configurações...");
        break;
    case 3:
        console.log("Saindo do aplicativo...");
        break;
    default:
        console.log("Opção inválida.");
}
```
*Nota: O comando `break` serve para parar a execução e sair do bloco assim que o caso correto for encontrado.*

---

## 4. O Papel dos Operadores Lógicos e de Comparação

Para criar as condições dentro dos parênteses, utilizamos operadores:

*   **Comparação:** `>`, `<`, `>=`, `<=`, `==` (igual), `!=` (diferente).
*   **Lógicos (União de condições):** 
    *   `&&` (E / AND) - Exige que **todas** as condições sejam verdadeiras.
    *   `||` (OU / OR) - Exige que **pelo menos uma** condição seja verdadeira.
    *   `!` (NÃO / NOT) - Inverte o valor lógico.
