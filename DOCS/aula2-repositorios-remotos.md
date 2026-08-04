## 1. Onde os Repositórios Remotos Ficam?

Eles ficam armazenados em plataformas de hospedagem de código baseadas em Git. As mais famosas do mercado são:

*   **GitHub**: A plataforma mais popular do mundo, muito utilizada para projetos de código aberto.
*   **GitLab**: Muito focada em automação, integração contínua (CI/CD) e projetos empresariais.
*   **Bitbucket**: Bastante integrada às ferramentas da Atlassian (como o Jira) e muito usada por empresas.

---

## 2. Principais Comandos de Interação

Para que o seu computador converse com o repositório remoto, você utiliza quatro comandos essenciais no terminal:

### 🔗 git remote add
Conecta o seu repositório local a um repositório remoto criado na nuvem. Geralmente o nome padrão dado a essa conexão remota é `origin`.
```bash
git remote add origin https://github.com
```

### ⬆️ git push
Envia as alterações que você salvou localmente (seus *commits*) para o servidor remoto. É o ato de "subir" o código.
```bash
git push origin main
```

### ⬇️ git pull
Baixa as atualizações do repositório remoto e as mistura automaticamente com o código que está na sua máquina. É o ato de "atualizar" seu projeto local.
```bash
git pull origin main
```

### 👯 git clone
Cria uma cópia exata de um repositório remoto existente na nuvem para dentro do seu computador. Você usa isso quando vai começar a trabalhar em um projeto que já existe.
```bash
git clone https://github.com
```

---

## 3. O Fluxo de Trabalho Tradicional

1. Você altera os arquivos no seu computador (**Local**).
2. Você faz um `git commit` para salvar uma foto dessas alterações no seu histórico local.
3. Você faz um `git push` para enviar essa foto para o GitHub (**Remoto**).
4. Seu colega de equipe faz um `git pull` para receber essa foto no computador dele.
