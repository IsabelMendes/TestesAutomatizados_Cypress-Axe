# Cap 7 - Escrevendo os testes de acessibilidade com Cypress

No capítulo anterior, vimos como podemos configurar o Cypress e o Cypress-Axe em um projeto de teste.

Continuaremos com o que temos até agora e, em seguida, começaremos a adicionar alguns testes automatizados de acessibilidade em nosso projeto.

Em termos do que você pode esperar deste capítulo, veremos:

1. Como você pode testar uma página inteira com Cypress-Axe.

2. Análise dos logs e mensagens de erro que recebemos para que possamos entender as diferentes falhas de acessibilidade.

3. Teste em elementos específicos na página.

4. Como você pode desabilitar algumas regras do Axe - eu normalmente recomendo não desabilitar nenhuma regra de acessibilidade, dessa forma você pode validar mais regras tanto quanto possível. Mas, em alguns casos pode ser necessário.


### Vamos começar

Todo o código que você verá hoje estará no repositório público do GitHub, que é adicionado como um link de recurso para este capítulo.

Não se preocupe se não entender imediatamente.

Repassarei o código um por um e tentarei explicar da melhor forma para que fique tudo claro para você.

Para este curso, vamos executar alguns testes de acessibilidade em um dos aplicativos de amostra mais populares que existem - o aplicativo **To Do**.

O link para acessar este aplicativo de tarefas pode ser encontrado aqui: [](https://todomvc.com/examples/react/#/)

Basicamente, este é apenas um aplicativo simples baseado em React para adicionar itens de tarefas e marcá-los como concluídos.

Portanto, como você pode ver aqui, estou apenas adicionando alguns itens de tarefas pendentes como parte da minha lista.

Assim que terminar, posso marcá-lo como concluído e então posso verificar se tenho algum item ativo ou aquele que marquei como concluído.

Também posso excluí-los se quiser.

![](/Users/isabelmendes/Desktop/Captura de Tela 2021-05-26 às 16.19.43.png)

Funcionalmente, você pode ver que funciona, mas como este é um curso sobre teste de acessibilidade, vamos escrever alguns testes que testam o quão acessível é o aplicativo React To Do.

Portanto, voltamos ao VS e o que farei é excluir os outros arquivos de teste que não precisamos para este projeto.

Vou adicionar um novo arquivo de teste, que chamarei de *todo-app.spec.js* e, neste arquivo, adicionarei uma importação aos tipos de referência do Cypress.

Agora, o que isso significa é - para que possamos habilitar o IntelliSense para este projeto, temos que adicionar este tipo de referência.

Isso garantirá que possamos acessar todos os diferentes métodos Cypress automaticamente.

Vou adicionar meu *bloco de descrição* e, no primeiro parâmetro, vou dar a ele um nome que chamarei de "Todo Application".

*Blocos de descrição* no Mocha permite que você agrupe seus testes de uma forma muito mais estruturada.

Se você quiser saber mais sobre a estrutura de teste do JavaScript Mocha, recomendo enfaticamente o curso do Giridhar [](https://testautomationu.applitools.com/mocha-javascript-tests/) na Universidade de Automação de Teste.

Agora, vamos escrever nosso primeiro bloco *it*.

Um bloco *it* no Mocha é uma forma de descrever o que é nosso teste.

Ele aceita dois parâmetros - o primeiro é apenas o título do nosso teste e o próximo parâmetro é a função que contém os diferentes comandos do Cypress que precisamos executar.

Então, o primeiro comando que precisamos é **cy.visit**, que é um método do Cypress, para visitar nosso aplicativo.

O próximo comando vem, na verdade, da biblioteca Cypress-Axe e é chamado de **cy.injectAxe**.

Agora o que esse comando faz é realmente injetar o tempo de execução do axe-core em nosso aplicativo de teste, portanto, ele deve ser adicionado depois que você visitar sua página de teste.

O último comando de que precisamos é **cy.checkA11y** ou **cy.checkAccessibility**.

Este comando irá, na verdade, examinar sua página em busca de falhas de acessibilidade.

> Nota: onde estamos no projeto:
>
> cypress > integration > new> todo-app.spec.js

```javascript
describe('Todo application', () => {
 it('should log any accessibility failures', () => {
   cy.visit('http://todomvc.com/examples/react');
   cy.injectAxe();
   cy.checkA11y();
 });
});
```

Agora vou apenas executar o comando:

```
npx cypress open
```

Se você se lembra do capítulo anterior, usamos este comando para iniciar o executor de teste Cypress.

![](/Users/isabelmendes/Desktop/Captura de Tela 2021-05-26 às 17.40.12.png)

Agora que está carregado, vamos prosseguir e clicar no arquivo de teste que escrevemos e esperar que os testes sejam executados.

![](/Users/isabelmendes/Desktop/Captura de Tela 2021-05-26 às 17.41.22.png)

Pelo que visto acima, o Cypress-Axe detectou 4 erros de acessibilidade.

Existem alguns erros no contraste de cor (color-contrast), alguns erros de acessibilidade na ordem do título (heading-order), ponto de referência principal (landmark-one-main) e também página com título um (page-nas-heading-one).

No próximo subcapítulo, veremos como analisar todas as diferentes regras de violação de acessibilidade que Cypress-Axe nos relatou.

