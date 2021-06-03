## Axe-Core

Axe-CLI: permite executar testes de acessibilidade diretamente na linha de comando

Pode ser integrado a diferentes ferramentas de testes: Cypress, Selenium, WebdriverIO, etc.

## Axe-CLI

Nenhum código é necessário

### Pré requisitos

IDE instalada e configurada (https://code.visualstudio.com/docs/setup/setup-overview)

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

