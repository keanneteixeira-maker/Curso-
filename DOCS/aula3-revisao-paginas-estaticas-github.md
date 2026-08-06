## 1. O que são Páginas Estáticas?
Ao contrário de sites dinâmicos (como WordPress ou sistemas que usam PHP e bancos de dados SQL), as páginas estáticas:
* Entregam o conteúdo exatamente do jeito que ele está armazenado no servidor.
* Não processam dados no lado do servidor (no-backend).
* São extremamente rápidas, seguras e leves.
* Podem rodar scripts no navegador do usuário (JavaScript), permitindo interatividade e consumo de APIs externas.

---

## 2. Como Funciona a Criação (Passo a Passo)

A publicação de um site estático no GitHub segue três etapas lógicas principais:

### Passo 1: Preparação dos Arquivos
Você precisa criar um repositório no GitHub e enviar os arquivos do seu site para lá. 
* O arquivo principal do seu site **obrigatoriamente** deve se chamar `index.html`.
* O GitHub procura por esse arquivo na raiz do repositório para usar como a página inicial do site.

### Passo 2: Ativação do Recurso
A ativação é feita diretamente na interface web do GitHub:
1. Acesse o seu repositório no GitHub.
2. Clique na aba **Settings** (Configurações).
3. No menu lateral esquerdo, clique em **Pages**.
4. Na seção *Build and deployment*, mude a origem (*Source*) para **Deploy from a branch**.
5. Escolha a branch (geralmente `main` ou `master`) e a pasta raiz (`/root`).
6. Clique em **Save**.

### Passo 3: Publicação e Acesso
O GitHub iniciará um processo automatizado (via GitHub Actions) para compilar e publicar seu site. Em menos de um minuto, o link público estará pronto.
* **Formato padrão da URL**: `https://github.io`

---

## 3. Principais Vantagens
* **Gratuito**: Sem custos de hospedagem ou servidores para projetos pessoais ou de código aberto.
* **HTTPS Automático**: O GitHub fornece um certificado de segurança SSL gratuito para o seu site.
* **Domínio Personalizado**: Permite configurar um domínio próprio (ex: `://meusite.com`) em vez de usar o link padrão do GitHub.
* **Integração com Jekyll**: Suporte nativo para geradores de sites estáticos, permitindo criar blogs inteiros usando apenas arquivos Markdown.
