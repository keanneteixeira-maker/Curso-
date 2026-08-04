## 1. O Fluxo de Trabalho Tradicional (GitHub Flow)

Para trabalhar em equipe de forma organizada e sem apagar o código dos colegas, o mercado adota um padrão conhecido como **GitHub Flow**. Ele consiste nos seguintes passos:

1.  **Criar uma Branch (Ramificação)**: Nunca faça alterações direto na linha principal (`main` ou `master`). Crie uma ramificação paralela chamada *branch* para desenvolver sua nova funcionalidade ou corrigir um bug.
    ```bash
    git checkout -b feature/nova-tela-login
    ```
2.  **Fazer Commits Localmente**: Faça as alterações nos arquivos e salve pequenos históricos explicativos (commits) na sua máquina.
3.  **Enviar para o GitHub (Push)**: Suba a sua branch com os commits para o servidor do GitHub.
    ```bash
    git push origin feature/nova-tela-login
    ```
4.  **Abrir um Pull Request (PR)**: No GitHub, você abre um pedido para que a sua branch seja misturada com a branch principal (`main`). É o momento em que você avisa a equipe: *"Terminei meu trabalho, alguém pode revisar?"*.
5.  **Revisão e Discussão (Code Review)**: Outros desenvolvedores analisam suas linhas de código, deixam comentários, sugerem melhorias ou aprovam a alteração.
6.  **Fazer o Merge (Fusão)**: Após a aprovação e a certeza de que o código funciona, o Pull Request é fechado e suas alterações são unidas à branch principal (`main`).

---

## 2. Formas de Colaboração no GitHub

Existem duas maneiras principais de colaborar em um projeto dentro da plataforma:

### A. Modelo de Repositório Compartilhado (Colaboradores Diretos)
Muito comum em empresas e equipes fechadas. O dono do repositório adiciona o seu usuário do GitHub como um "colaborador". Você ganha permissão direta para clonar o projeto na sua máquina, criar branches e enviar commits (`git push`) diretamente para aquele repositório.

### B. Modelo Fork & Pull (Projetos de Código Aberto / Open Source)
Utilizado quando você quer sugerir uma melhoria em um projeto público do qual você não faz parte da equipe oficial.
1.  Você clica no botão **Fork** no topo da página do projeto para gerar uma cópia idêntica dele dentro da *sua própria conta* do GitHub.
2.  Você clona o *seu fork*, faz as alterações e dá o `push` para a sua conta.
3.  Pela interface do GitHub, você envia um **Pull Request** do seu repositório para o repositório do criador original do projeto, sugerindo a alteração.

---

## 3. Boas Práticas de Trabalho no GitHub

Seguir boas práticas evita dores de cabeça como conflitos de código difíceis de resolver ou perda de histórico de trabalho.

*   **Escreva Commits Descritivos**: Evite mensagens genéricas como `git commit -m "ajustes"`. Use o padrão de Commits Semânticos ou mensagens claras no imperativo (ex: `git commit -m "Adiciona validação de e-mail no formulário de login"`).
*   **Mantenha as Branches Focadas**: Uma branch deve resolver apenas uma coisa. Não tente consertar um bug de banco de dados na mesma branch que altera o estilo visual de um botão.
*   **Faça Pulls Frequentemente**: Antes de começar a trabalhar no dia, atualize seu repositório local com o comando `git pull origin main`. Isso garante que você está programando em cima da versão mais recente do projeto.
*   **Automatize com Issues e Quadros**: Use as **Issues** do GitHub para relatar bugs e planejar novas tarefas. Você pode vinculá-las a um **Project** (quadro estilo Kanban) para que toda a equipe saiba quem está fazendo o que em tempo real.
*   **Use um arquivo `.gitignore`**: Nunca envie para o GitHub arquivos temporários do sistema operacional, pastas de dependências pesadas (como a `node_modules` no JavaScript) ou arquivos com senhas e chaves de segurança. Liste-os no arquivo `.gitignore` para o Git ignorá-los.
