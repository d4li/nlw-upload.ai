<p align="center">
  <img width="200px" alt="Project NLW IA Mastery" title="Project NLW IA Mastery Logo" src="./.gihub/logo-nlw-ia-mastery.svg" />
  
  <h1 align="center">NLW Upload.AI</h1>

O NLW Upload.AI é um projeto desenvolvido durante a trilha Mastery do Next Level Week IA da Rocketseat. A aplicação utiliza a Inteligência Artificial da OpenAI para aprimorar a transcrição de vídeos e gerar títulos e descrições para conteúdo do YouTube.

</p>

## 🚀 Funcionalidades

- Transcrição de vídeos de forma precisa e eficiente.
- Geração automática de títulos e descrições atraentes para vídeos.
- Integração fácil com o YouTube para carregar conteúdo automaticamente.

## 💡 Tecnologias Utilizadas

### Back-end

- [x] Node.js
- [x] [Fastify](https://fastify.dev/)
- [x] [Prisma](https://www.prisma.io/client)
- [x] [TypeScript](https://www.typescriptlang.org/)
- [x] [fastify-multipart](https://github.com/fastify/fastify-multipart)
- [x] [Zod](https://zod.dev/)
- [x] [Openai](https://platform.openai.com/docs/api-reference)

### Front-end Web

- [x] [React](https://reactjs.org/)
- [x] [Vite](https://vitejs.dev/)
- [x] [TypeScript](https://www.typescriptlang.org/)
- [x] [Tawilndcss](https://tailwindcss.com/)
- [x] [RadixUi](https://www.radix-ui.com/primitives/docs/overview/introduction)
- [x] [Shadcn/ui](https://ui.shadcn.com/docs)
- [x] [Lucide React](https://lucide.dev/guide/packages/lucide-react)
- [x] [ffmpeg.wasm](https://ffmpegwasm.netlify.app/)
- [x] [Axios](https://axios-http.com/ptbr/)

## 📂 Estrutura de Pastas

```plainText
app
.
.
├── upload-ai-api               # Projeto Back-end
│   ├── src                       # Arquivos de origem
│         ├── lib                   # Contém as conexões
│         ├── routes                # Contém as rotas
│         . server.ts               # Entrada da aplicação
│   ├── tmp                       # Arquivos MP3 salvos para transcrição
│   . .env                        # Variáveis de ambiente
│   . routes.http                 # Executando rotas com Rest Client
.
├── upload-ai-web               # Projeto Front-end Web
│   ├── src                       # Arquivos de origem
│         ├── components            # Contém todos os componentes React globais
│         ├── ffmpeg                # Contém arquivos do ffmpeg
│         ├── lib                   # Contém as conexões
│         . main.tsx                # Entrada da aplicação React
│   . index.html                  # Entrada da aplicação
│
.
└── README.md
```

## 📋 Pré-requisitos

Antes de começar, certifique-se de ter os seguintes requisitos instalados:

- Node.js (versão 18 ou superior)
- NPM (gerenciador de pacotes do Node.js)

## 🚀 Executando o Projeto

Clone o projeto

```bash
  git clone https://github.com/d4li/nlw-upload.ai.git
```

### Back-end

Acesse o diretório do projeto

```bash
  cd nlw-upload.ai/upload-ai-api
```

Instale as dependências

```bash
  npm install
```

Crie o arquivo '.env' seguindo o exemplo no arquivo '.env.example'.

Para criar e obter a chave da OpenAI, visite https://platform.openai.com/account/api-keys."

Crie o banco de dados

```bash
  npx prisma migrate dev
```

Crie dados na tabela do prompt

```bash
  npx prisma db seed
```

Inicie o servidor

```bash
  npm run dev
```

### Front-end Web

Acesse o diretório do projeto

```bash
  cd nlw-upload.ai/upload-ai-web
```

Instale as dependências

```bash
  npm install
```

Inicie o servidor

```bash
  npm run dev
```

8. Acesse a aplicação no seu navegador:

```
  http://localhost:5173
```
