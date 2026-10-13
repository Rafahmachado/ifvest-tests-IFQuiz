# IFVest - Testes Automatizados do IFQuiz

## Sobre o projeto

Este repositório tem como objetivo apoiar a criação de testes automatizados para o sistema IFQuiz, utilizando Playwright e JavaScript.

O projeto está na etapa inicial de preparação do ambiente e captura dos fluxos de navegação da aplicação. A partir do código gerado pelo Playwright Codegen, serão elaborados e revisados os scripts de teste.

## Objetivos

- Capturar os principais fluxos de navegação do IFQuiz.
- Registrar as interações realizadas na aplicação.
- Utilizar o código gerado como base para a criação dos testes automatizados.
- Desenvolver testes de autenticação, incluindo cenários positivos e negativos.
- Registrar os resultados das execuções e investigar possíveis falhas.

## Tecnologias utilizadas

- **JavaScript:** linguagem utilizada nos scripts de teste.
- **Node.js e npm:** execução do projeto e gerenciamento das dependências.
- **Playwright:** automação do navegador e execução dos testes.
- **Playwright Codegen:** gravação das interações realizadas durante a navegação.
- **GitHub Codespaces:** ambiente de desenvolvimento na nuvem.

## Estrutura do projeto

```text
ifvest-tests-IFQuiz/
├── tests/
│   └── example.spec.js
├── .gitignore
├── package.json
├── package-lock.json
├── playwright.config.js
└── README.md
```

A estrutura será atualizada conforme os fluxos forem capturados e os testes forem desenvolvidos.

## Como acessar o projeto

1. Acesse o repositório no GitHub: https://github.com/Rafahmachado/ifvest-tests-IFQuiz
2. Abra o projeto em um ambiente GitHub Codespaces.
3. No terminal, instale as dependências:

```bash
npm ci
```

4. Instale o navegador Chromium utilizado pelo Playwright:

```bash
npx playwright install chromium
```

## Captura da navegação com Playwright Codegen

Para iniciar a gravação, execute:

```bash
npx playwright codegen "https://ifvest.com.br/"
```


Com o navegador aberto, realize o fluxo que deseja registrar. O Codegen gerará código com base nas interações realizadas, que poderá ser revisado e aproveitado na criação dos scripts de teste.

**Atenção:** a captura da navegação é uma etapa inicial. O código gerado deverá ser revisado antes de ser utilizado como teste automatizado.

## Execução dos testes

Para executar os testes existentes:

```bash
npm test
```

Para abrir a interface de execução do Playwright:

```bash
npm run test:ui
```

## Próximas etapas

1. Capturar os fluxos de navegação do IFQuiz.
2. Revisar e organizar os scripts gerados.
3. Desenvolver os testes positivos e negativos de autenticação.
4. Executar os testes e analisar os resultados.
5. Registrar evidências e possíveis defeitos encontrados.

## Colaboração

As contribuições devem ser enviadas por meio do GitHub. Antes de compartilhar alterações, confira os arquivos modificados e não inclua credenciais, senhas ou dados pessoais nos scripts e nos registros de teste.
