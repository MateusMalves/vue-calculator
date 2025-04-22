# Vue Calculadora

Este projeto é uma calculadora aritmética simples desenvolvida com Vue.js. A aplicação permite que os usuários insiram dois números e escolham uma operação aritmética para realizar o cálculo automaticamente.

## Estrutura do Projeto

```
vue-calculadora
├── public
│   └── index.html          # Ponto de entrada da aplicação
├── src
│   ├── components
│   │   └── Calculator.vue  # Componente da calculadora
│   ├── App.vue             # Componente raiz da aplicação
│   ├── main.js             # Ponto de entrada do JavaScript
│   └── assets              # Diretório para arquivos estáticos
├── package.json            # Configuração do npm
├── vite.config.js          # Configuração do Vite
└── README.md               # Documentação do projeto
```

## Instalação

1. Clone o repositório:
   ```
   git clone <URL_DO_REPOSITORIO>
   ```
2. Navegue até o diretório do projeto:
   ```
   cd vue-calculadora
   ```
3. Instale as dependências:
   ```
   npm install
   ```

## Uso

Para iniciar a aplicação, execute o seguinte comando:
```
npm run dev
```

A aplicação estará disponível em `http://localhost:3000` (ou outra porta especificada no terminal).

## Funcionalidades

- Dois campos de entrada para inserir números.
- Um campo de seleção para escolher a operação aritmética (adição, subtração, multiplicação, divisão).
- Cálculo automático ao alterar os valores nos campos de entrada ou na seleção da operação.

## Contribuição

Sinta-se à vontade para contribuir com melhorias ou correções. Faça um fork do repositório e envie um pull request com suas alterações.