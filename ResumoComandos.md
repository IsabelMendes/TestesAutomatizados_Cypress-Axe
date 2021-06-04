## Axe-Core

Axe-CLI: permite executar testes de acessibilidade diretamente na linha de comando

Pode ser integrado a diferentes ferramentas de testes: Cypress, Selenium, WebdriverIO, etc.

## Axe-CLI

Nenhum código é necessário

### Pré requisitos

Node (https://nodejs.org/en/download/) e NPM (https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) instalados

### Instalando o Axe-CLI

```
npm install -g axe-cli
```

-g: vamos adicionar globalmente.

```
 axe https://www.ifnmg.edu.br/cursos
```

```
axe https://www.ifnmg.edu.br/cursos --browser chrome
```

- Se você deseja executar o teste em um navegador real, o que você pode fazer é passar o parâmetro do navegador seguido do nome do navegador.

```
axe https://www.ifnmg.edu.br/cursos, https://www.ifnmg.edu.br/portal
```

- Analisar duas páginas ao mesmo tempo

```
axe https://www.ifnmg.edu.br/cursos --disable color-contrast
```

- Desabilitar a busca por erros de contraste

```
axe https://www.ifnmg.edu.br/cursos --save ifnmgTestResults.json
```

## Cypress-Axe

### Pré requisito

1. IDE instalada e configurada (https://code.visualstudio.com/docs/setup/setup-overview)

2. Node + NPM

3. Criar um diretório: Cypress-axe-project

4. No terminal e dentro do diretório digite o comando que irá inicializar o projeto e gerenciar todas as depêndencias

   ```
   npm int -y
   ```

5. Instalando o Cypress e o Cypress-Axe:

   ```
   npm install cypress --save-dev
   npm install --save-dev cypress-axe
   ```

6. Para abrir o executor de teste do Cypress:

   ```
   npx cypress open
   ```

    Npx: executa um comando específico

7. Importar os comando que precisamos do Cypress-Axe, dentro de support/index.js:

    import './comands'; import 'cypress-axe';

   

   
