<div align="center">
  <img src="./.github/banner.jpg" alt="Banner-project" />
</div>

## Tópicos

<div>
 • <a href="#-sobre-o-projeto">Sobre o Projeto</a> </br>
 • <a href="#-tecnologias">Tecnologias</a> </br>
 • <a href="#-layout">Layout</a> </br>
 • <a href="#-funcionalidades">Funcionalidades</a> </br>
 • <a href="#-estrutura-de-pastas">Estrutura de pastas</a> </br>
 • <a href="#-estrutura-de-componentes">Estrutura de componentes</a> </br>
 • <a href="#-estrutura-do-banco-de-dados">Estrutura do banco de dados</a> </br>
 • <a href="#-como-executar-o-projeto">Como executar</a> </br>
 • <a href="#-como-contribuir">Como contribuir</a> </br>
 • <a href="#-autor">Autor</a> </br>
 • <a href="#user-content--licença">Licença</a></br>
</div>

## Sobre o projeto

Este projeto é uma iniciativa de compartilhar com a comunidade
do EstudeCê um template mais padrão para o readme dos repositórios.

## Tecnologias

#### **Website** ( [ReactJS](https://reactjs.org/) + [TypeScript](https://www.typescriptlang.org/) )

- [React Hook Form](https://react-hook-form.com/)
- [React Icons](https://react-icons.github.io/react-icons/)
- [Axios](https://github.com/axios/axios)
- [StyledComponents](https://styled-components.com/)
- [Yup](https://github.com/jquense/yup)

#### **Mobile** ( [React Native](https://reactnative.dev/) + [TypeScript](https://www.typescriptlang.org/) )

- [Expo](https://expo.dev/)
- [Axios](https://github.com/axios/axios)
- [StyledComponents](https://styled-components.com/)

#### **API** ( [NodeJS](https://nodejs.org/en/) + [TypeScript](https://www.typescriptlang.org/) )

- [Mongoose](https://mongoosejs.com/)
- [Express](https://expressjs.com/pt-br/)

#### **Utilitários**

- Banco de dados: **[MongoDb](https://www.mongodb.com/)**
- Protótipo: **[Figma](https://www.figma.com/)** → **[Protótipo (Projeto)](link-para-o-figma-do-teu-projeto)**
- Editor: **[Visual Studio Code](https://code.visualstudio.com/)** → Extensions: **[Prettier](https://prettier.io/)** + **[EditorConfig](https://editorconfig.org/)**
- Fontes: **[OpenSans](https://fonts.google.com/specimen/Open+Sans)**
- Versionamento: **[Git](https://git-scm.com)**
- Padronização de código: **[ESLint](https://eslint.org/)**

## Layout

O layout da aplicação está disponível no Figma:

<a href="link-para-o-figma-do-projeto">
  <img alt="Made by vitor" src="https://img.shields.io/badge/Acessar%20Layout%20-Figma-%2304D361">
</a>

<p align="center">
  <img src="./.github/layout.png" alt="layout-project" />
</p>

## Funcionalidades

Features que estão sendo adicionadas na aplicação

**Front-end Web**

- [ ] Features do Front-end

**Front-end Mobile**

- [ ] Features do mobile

**Back-end**

- [x] Estruturar uma forma de linkar o data com o workout
- [ ] Features do back-end

## 🛠 Estrutura de pastas e componentes

Afim de facilitar a organização e manutenção do código, foi definido um padrão para organização das pastas neste projeto.

**Front-end Web**

→ \_assets: Contém a estilização global, icones, fontes, tema da aplicação, itens de estilo que são reutilizáveis e imagens; <br />
→ components: Todos os componentes globais do projeto; <br />
→ context: Armazena os contextos da aplicação; <br />
→ services: Todos os acessos externos; <br />
→ utils: Funcionalides que são utilizadas em diversos locais da aplicação; <br />
→ types: Todos as interfaces que são utilizadas em diversos locais da aplicação; <br />
→ hooks: Custom hooks; <br />

Todos os componentes criados vão seguir uma mesma estrutura de organização:
→ index.tsx: Responsável por exportar o componente; <br />
→ interface.ts: Responsável por exportar as interfaces; <br />
→ styles.ts: Responsável por toda estilização do componente; <br />

**Back-end**

→ models: Todos os models de Schema para adicionar ao banco de dados; <br />
→ useCases: Armazena todos os casos que são úteis a aplicação. A pasta useCases possui a mesma separação dos models do Schema ; <br />

## Como executar o projeto

Este projeto é divido em duas partes:

1. Backend (pasta api)
2. Frontend Web (pasta client)

💡 O Frontend precisa que o Backend esteja sendo executado para funcionar.

### Pré-requisitos

Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas: <br />
→ [Git](https://git-scm.com);<br />
→ [Node.js](https://nodejs.org/en/);<br />

Além disto é bom ter um editor para trabalhar com o código como [VSCode](https://code.visualstudio.com/);

Para executar o banco de dados MongoDb, foi utilizado a aplicação do [MongoDB Community](https://www.mongodb.com/try/download/community), mas existem outras alternativas como o [Docker container](https://www.docker.com/resources/what-container/)

#### 🎲 Rodando a aplicação (Backend)

```bash
# Clone este repositório
$ git clone https://github.com/estude-ce/Projeto.git
# Vá para a pasta da aplicação Back End
$ cd api
# Instale as dependências
yarn install
# Rode a aplicação
yarn start
# A aplicação será aberta na porta:3001 - acesse http://localhost:3001
```

---

#### 🧭 Rodando a aplicação web (Frontend)

```bash
# Clone este repositório
$ git clone https://github.com/estude-ce/Projeto.git
# Vá para a pasta da aplicação Front End
$ cd client
# Instale as dependências
yarn install
# Rode a aplicação
yarn start
# A aplicação será aberta na porta:5173 - acesse http://localhost:5173
```

# Como contribuir

Caso queira contribuir, seja corrigindo bugs, adicionando comentários ou novas features, você pode seguir o seguinte tutorial:

- Faça um **[fork](https://help.github.com/pt/github/getting-started-with-github/fork-a-repo)** desse repositório
- **[Clone](https://help.github.com/pt/github/creating-cloning-and-archiving-repositories/cloning-a-repository)** o repositório que você fez o fork em seu computador
- Crie uma branch com a sua feature: `git checkout -b minha-alteracao`
- Envie suas alterações para a _staging area_: `git add .`
- Faça um commit contando o que você fez: `git commit -m "feat: minha nova alteracao!"`
- Faça um push para a sua branch: `git push origin minha-alteracao`
- Agora é só abrir uma _pull request!_

_Caso tenha alguma dúvida, confira este [guia de como contribuir no GitHub](https://github.com/firstcontributions/first-contributions/blob/master/translations/README.pt_br.md) :)_

<br />

# Entre em contato

**Linkedin**: link-para-o-linkedin

Desenvolvido por **Meu nome** 👋🏻
