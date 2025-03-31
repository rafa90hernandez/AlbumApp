# Projeto Mobile – App de Álbuns (React Native)

Este repositório contém o projeto completo do aplicativo móvel desenvolvido em **React Native** como parte da disciplina de **Desenvolvimento de Sistema Mobile** da PUCRS.

---

## 🌟 Objetivo

O aplicativo permite visualizar usuários, seus álbuns e as fotos de cada álbum. É possível realizar buscas de forma integrada por nome de usuário, título de álbum ou legenda de fotos.

---

## ✅ Funcionalidades Implementadas

### Lista de Usuários
- Exibição dos usuários em **grid**
- Avatares com nomes
- Campo de **busca funcional por nome**
- Ao clicar, navega para os álbuns do usuário

### Tela de Álbuns
- Exibição dos álbuns do usuário selecionado
- Cartões com miniaturas das fotos
- Cabeçalho com **nome, idade, profissão e cidade** do usuário
- Campo de **busca global** (usuário, álbum ou legenda da foto)
- Resultados da busca são **clicáveis e redirecionam**

### Tela de Fotos do Álbum
- Exibição em **grade (3 por linha)** com thumbnails
- Cabeçalho com os dados do usuário
- Campo de **busca global**
- Resultado da busca pode ser:
  - Usuário → redireciona para seus álbuns
  - Álbum → redireciona para as fotos
  - Legenda → exibe a miniatura da foto
- Modal com **foto ampliada e legenda com hashtags**

---

## 🔗 API Utilizada

Foi utilizada a feature **my-json-server** do GitHub para simular a API com imagens reais:

```
https://my-json-server.typicode.com/rafa90hernandez/jsplaceholder/
```

Endpoints:
- `/users`
- `/albums?userId=`
- `/photos?albumId=`

---

## 🧰 Tecnologias

- React Native (CLI)
- JavaScript (sem TypeScript)
- Axios (consumo de API)
- React Navigation (Stack)
- Estilização via `StyleSheet`
- FlatList (com renderização condicional)
- Ícones: `react-native-vector-icons/Ionicons`

---

## ▶️ Como rodar o projeto

```bash
Localize o diretório AlbumApp baixado
cd AlbumApp
npm install
npx react-native run-android
```

Para rodar o Metro Bundler separadamente:
```bash
npx react-native start
```

> Certifique-se de que o emulador Android está ativo antes de rodar.

---

## 📝 Observações

- O app **não utiliza banco de dados nem autenticação**
- Toda a navegação é feita com `React Navigation`
- Filtros e buscas são **realizados em memória**
- O layout foi baseado nos **protótipos da Fase 1**
- A busca é **global** e funcional em todas as telas

---

## 👨‍💻 Desenvolvedor

**Rafael Hernandez**  
📚 PUCRS – Desenvolvimento de Sistema Mobile  
🗖️ Ano: 2025
