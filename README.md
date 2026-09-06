# 🛡️ Servidor de Arquivos Criptografados

> Plataforma web para armazenamento e compartilhamento seguro de arquivos com criptografia ponta a ponta, comunicação em tempo real via WebSockets e interface estilizada com Tailwind CSS.

---

## 📌 Visão Geral

O **Servidor de Arquivos Criptografados** é uma aplicação cliente-servidor voltada à segurança de dados e confidencialidade no upload, armazenamento e tráfego de arquivos sensíveis. 

Construído sobre o ecossistema **Node.js** com **Express 5**, o projeto integra rotinas criptográficas com **node-forge** e **crypto**, proteção e hash de credenciais com **bcrypt**, suporte a transferências multipart via **Multer** e sincronização de eventos de upload em tempo real com **Socket.io**[cite: 31].

---

## ✨ Funcionalidades

- 🔒 **Criptografia de Arquivos e Dados**:
  - Manipulação e cifragem criptográfica robusta utilizando primitivas do `crypto` nativo e suíte `node-forge`[cite: 31].
  - Armazenamento não legível no disco para prevenir vazamentos de dados não autorizados[cite: 31].
- 👤 **Autenticação & Segurança de Usuários**:
  - Hashing e verificação de senhas via `bcrypt` / `bcryptjs` com salt rounds configuráveis[cite: 31].
  - Controle de requisições cross-origin com suporte a `cors`[cite: 31].
- 📂 **Gerenciamento de Uploads**:
  - Processamento multipart/form-data através de `multer`[cite: 31].
  - Operações assíncronas no sistema de arquivos estruturadas com `fs-extra`[cite: 31].
- ⚡ **Atualizações em Tempo Real**:
  - Notificações de upload, progresso e status de arquivos via WebSockets com `socket.io`[cite: 31].
- 🎨 **Interface Moderna**:
  - Estilização com a nova versão de alta performance do `Tailwind CSS v4`[cite: 31].

---

## 🛠️ Tecnologias Utilizadas

- **Ambiente de Execução:** [Node.js](https://nodejs.org/) (v18+)
- **Framework Web:** [Express 5](https://expressjs.com/)[cite: 31]
- **WebSockets:** [Socket.io](https://socket.io/)[cite: 31]
- **Criptografia & Segurança:** `crypto`, `node-forge`, `bcrypt` e `bcryptjs`[cite: 31]
- **Upload & Sistema de Arquivos:** `multer` e `fs-extra`[cite: 31]
- **Front-end & Estilização:** [Tailwind CSS v4](https://tailwindcss.com/) (`@tailwindcss/vite`, `@tailwindcss/cli`)[cite: 31]
- **Ferramentas de Desenvolvimento:** `nodemon` (hot reload)[cite: 31]

---

## 📁 Estrutura do Projeto

```text
servidor-arquivos-criptografados/
│
├── backend/
│   └── server.js            # Ponto de entrada do servidor Express e Socket.io[cite: 31]
├── uploads/                 # Diretório de armazenamento dos arquivos cifrados[cite: 31]
├── package.json             # Dependências e scripts de automação[cite: 31]
├── package-lock.json        # Árvore de dependências resolvidas[cite: 32]
├── LICENSE                  # Licença de código aberto MIT
└── README.md                # Documentação da aplicação

🚀 Como Executar o Projeto Localmente
Pré-requisitos
Node.js (versão 18 ou superior)[cite: 32].

Gerenciador de pacotes npm.

Passo a passo
Clone o repositório:

Bash


git clone [https://github.com/SEU-USUARIO/servidor-arquivos-criptografados.git](https://github.com/SEU-USUARIO/servidor-arquivos-criptografados.git)
cd servidor-arquivos-criptografados
Instale as dependências do projeto:

Bash


npm install
Inicie o servidor em modo de desenvolvimento (com auto-reload):

Bash


npm run dev
Este comando utiliza o nodemon apontando diretamente para backend/server.js[cite: 31].

Ou inicie em modo de produção:

Bash


npm start
Executa a aplicação diretamente com node backend/server.js[cite: 31].
