# Star Wars - RunApi

Aplicativo mobile feito em React Native (Expo) que consome a [SWAPI](https://swapi.info/) para exibir informações do universo Star Wars: personagens, planetas e filmes, navegando por abas.

## Tecnologias

- [Expo](https://expo.dev/) / React Native
- React Navigation (bottom tabs e stack)
- React Native Paper / React Native Vector Icons
- Material UI (`@mui/material`, `@emotion`)

## Funcionalidades

- **Home**: tela de boas-vindas com imagem de fundo temática.
- **Personagens** ([pages/Rebeldes.js](pages/Rebeldes.js)): lista de personagens consumindo `https://swapi.info/api/people`, exibindo nome, peso, altura, cor de cabelo, pele e olhos, ano de nascimento e gênero.
- **Planetas** ([pages/Planetas.js](pages/Planetas.js)): lista de planetas consumindo `https://swapi.info/api/planets`, exibindo nome, período de rotação/órbita, diâmetro, clima, gravidade, terreno, água e população.
- **Filmes** ([pages/ImperioStack.js](pages/ImperioStack.js)): lista de filmes consumindo `https://swapi.info/api/films`, exibindo título, episódio, texto de abertura, diretor, produtor e data de lançamento.

A navegação entre as telas é feita por uma barra de abas inferior, definida em [pages/RoutesTab.js](pages/RoutesTab.js).

## Como executar

### Pré-requisitos

- [Node.js](https://nodejs.org/)
- [Expo CLI](https://docs.expo.dev/get-started/installation/)

### Instalação

```bash
npm install
```

### Rodando o projeto

```bash
npm start       # abre o Expo Dev Tools
npm run android # abre no emulador/dispositivo Android
npm run ios     # abre no simulador/dispositivo iOS
npm run web     # abre no navegador
```

## Estrutura do projeto

```
.
├── App.js                  # Ponto de entrada, envolve a navegação
├── components/
│   └── estiloRebeldes.js   # Estilos compartilhados pelas listas
└── pages/
    ├── Home.js             # Tela inicial
    ├── Rebeldes.js         # Lista de personagens
    ├── Planetas.js         # Lista de planetas
    ├── ImperioStack.js     # Lista de filmes
    └── RoutesTab.js        # Configuração das abas de navegação
```


