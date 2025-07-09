# ReactGram

## Sobre o Projeto

O ReactGram é um projeto de uma pequena rede social de compartilhamento de fotos, semelhante ao Instagram, desenvolvido como parte do curso **"React do Zero a Maestria"** da Udemy. O principal objetivo deste projeto foi aplicar e consolidar os conhecimentos adquiridos no curso, focando na criação de uma aplicação full-stack com React no frontend e Node.js no backend.

**É importante ressaltar que este projeto foi desenvolvido para fins de aprendizado e não deve ser utilizado em produção.**

## Funcionalidades

O ReactGram permite que os usuários:

- **Criem uma conta e façam login:** Sistema de autenticação completo com validação de dados.
- **Atualizem seus perfis:** Os usuários podem alterar seu nome, biografia, foto de perfil e senha.
- **Publiquem fotos:** Funcionalidade de upload de imagens com título.
- **Visualizem o feed de fotos:** A página inicial exibe as fotos mais recentes de todos os usuários.
- **Curtam fotos:** Os usuários podem curtir e descurtir as fotos.
- **Comentem nas fotos:** É possível adicionar comentários nas publicações.
- **Busquem por fotos:** Um campo de busca permite pesquisar fotos por título.
- **Visualizem perfis de outros usuários:** Ao clicar no nome de um autor de uma foto, o usuário é redirecionado para o perfil dele.

## Tecnologias Utilizadas

### Backend

- **Node.js:** Ambiente de execução para o JavaScript no servidor.
- **Express:** Framework para a criação da API REST.
- **MongoDB com Mongoose:** Banco de dados NoSQL para armazenar as informações de usuários e fotos.
- **bcryptjs:** Para a criptografia de senhas.
- **JSON Web Token (JWT):** Para a criação de tokens de autenticação.
- **Multer:** Middleware para o upload de arquivos.
- **CORS:** Para permitir o acesso da API pelo frontend.
- **Dotenv:** Para o gerenciamento de variáveis de ambiente.

### Frontend

- **React:** Biblioteca para a construção da interface de usuário.
- **React Router Dom:** Para o gerenciamento de rotas na aplicação.
- **Redux com Redux Toolkit:** Para o gerenciamento do estado global da aplicação.
- **React Icons:** Para a utilização de ícones.

## Como Executar o Projeto

Para executar o projeto, você precisará ter o Node.js e o npm (ou Yarn) instalados em sua máquina.

### 1. Backend

Primeiro, clone o repositório e instale as dependências do backend.

```bash
# Navegue para a pasta do backend
cd 12_REACTGRAM/backend

# Instale as dependências
npm install
```

Você precisará criar um arquivo `.env` na raiz da pasta backend com as seguintes variáveis de ambiente:

```
DB_USER=seu_usuario_do_mongodb
DB_PASSWORD=sua_senha_do_mongodb
JWT_SECRET=seu_segredo_jwt
PORT=5000
```

- `DB_USER` e `DB_PASSWORD`: Suas credenciais do MongoDB Atlas.
- `JWT_SECRET`: Uma string secreta para assinar os tokens JWT.
- `PORT`: A porta em que o backend será executado.

Após configurar as variáveis de ambiente, inicie o servidor do backend:

```bash
npm run server
```

O backend estará rodando em `http://localhost:5000`.

### 2. Frontend

Em um novo terminal, navegue para a pasta do frontend e instale as dependências.

```bash
# Navegue para a pasta do frontend
cd 12_REACTGRAM/frontend

# Instale as dependências
npm install
```

Após a instalação, inicie a aplicação React:

```bash
npm start
```

O frontend estará rodando em `http://localhost:3000` e se conectará automaticamente ao backend.
