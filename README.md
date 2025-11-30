# — React Native + Expo + API Pública (Coinbase)

Este projeto tem como objetivo criar um aplicativo simples utilizando **React Native**, **Expo** e **TypeScript**, capaz de consumir uma **API pública** e exibir os dados em tela.

A API escolhida foi a **Coinbase Exchange Rates API**, que fornece taxas de câmbio em tempo real.

---

## 🚀 Tecnologias utilizadas

* **React Native**
* **Expo**
* **TypeScript**
* **Axios**
* **Coinbase API**

---

## 🎯 Objetivo

O aplicativo deve:

* **Consumir dados** de uma API pública
* **Exibir as informações** na interface
* Mostrar **estados de carregamento** e **erro**
* Mostrar a **lista com os dados** retornados pela API

---

## 🔗 API Utilizada

**Coinbase Exchange Rates API**

Endpoint utilizado:

`https://api.coinbase.com/v2/exchange-rates?currency=BTC`

A API retorna **taxas de câmbio** referentes a **1 BTC** em diversas moedas.

---

## 📂 Estrutura de Pastas

src/
 ├── api/
 │     └── apiClient.ts
 ├── screens/
 │     └── HomeScreen.tsx
 └── types/
       └── index.ts

App.tsx


* **`api/apiClient.ts`**: Arquivo responsável por configurar o **Axios**.
* **`types/index.ts`**: Define os **tipos TypeScript** utilizados no projeto.
* **`screens/HomeScreen.tsx`**: Tela principal que **consome a API**, trata os **estados (loading/erro)** e **exibe os dados**.
* **`App.tsx`**: Ponto de entrada da aplicação.

---

## ▶️ Como executar o projeto

1.  **Clone o repositório**:
    ```bash
    git clone [https://github.com/SEU-USUARIO/NOME-DO-REPO.git](https://github.com/SEU-USUARIO/NOME-DO-REPO.git)
    cd NOME-DO-REPO
    ```

2.  **Instale as dependências**:
    ```bash
    npm install
    # ou
    yarn
    ```

3.  **Execute o app**:
    ```bash
    npx expo start
    ```

> Use o **Expo Go** no seu celular para visualizar o app.

---

## 🧩 Funcionamento

Ao iniciar o aplicativo:

1.  Uma **requisição HTTP** obtém as taxas de câmbio da Coinbase
2.  Os dados retornam em formato de **objeto** e são convertidos para **array**
3.  Uma **lista** exibe cada moeda e seu valor
4.  Um **indicador de carregamento** aparece enquanto os dados são buscados
5.  Caso ocorra **erro**, uma mensagem é exibida

