## 1. Elementos Fundamentais
* **Inicialização**: Estado inicial antes de o laço começar.
* **Condição de parada**: Expressão lógica testada a cada repetição.
* **Incremento/Atualização**: Alteração do valor para que a condição se torne falsa em algum momento.

## 2. Tipos Principais

### Para / For (Repetição Contada)
* Utilizada quando se sabe o número exato de repetições.
* *Exemplo*: Contar de 1 até 10.

### Enquanto / While (Repetição Condicional Pré-testada)
* Utilizada quando o número de repetições é desconhecido.
* Avalia a condição **antes** de executar o bloco.
* *Exemplo*: Continuar lendo um arquivo até chegar ao fim.

### Faça... Enquanto / Do-While (Repetição Condicional Pós-testada)
* Garante que o código rode **pelo menos uma vez**.
* Avalia a condição apenas **no final** do bloco.
* *Exemplo*: Exibir um menu de opções ao usuário.

## 3. O Perigo do Loop Infinito
Ocorre quando a condição de parada nunca é atingida (ex: esquecer de incrementar a variável de controle). Isso consome memória e trava a execução do sistema.
