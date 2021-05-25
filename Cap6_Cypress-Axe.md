# Capítulo 6 - Configurando o Cypress-Axe para seus testes específicos 

Neste capítulo, obteremos mais informações técnicas e configuraremos o Cypress e o Cypress-Axe para começar a automatizar alguns de nossos testes de acessibilidade.

Nós vamos:

- Criar um projeto de teste simples.

- Ver como podemos instalar o Cypress e o Cypress-Axe neste projeto

- Importar o Cypress-Axe para o nosso projeto para que possamos estender os comandos padrões do Cypress


## Pré requisitos

Como pré-requisito, para instalar o Cypress, você precisa ter o Node e o NPM instalados em sua máquina, bem como o Visual Studio Code.

Se você não tiver esses programas instalados, vá em frente e volte quando tudo estiver pronto.

Você pode consultar os recursos abaixo para encontrar os links sobre como instalar esses programas.


## Instalação e configuração
Em primeiro lugar, vamos fazer a instalação e configuração.

Como já tenho o Node instalado, não preciso fazer a parte da instalação.

Se você quiser descobrir se você instalou o Node com sucesso, basta digitar:

```
node -v
```

Será informado o número da versão que você está usando.

O que faremos agora é criar um novo projeto de teste, que chamarei de cypress-axe-project.

Uma vez que este diretório é criado, vamos prosseguir e ir para este diretório digitando cd, seguido do nome do projeto.

```
cd cypress-axe-project
```

Em seguida, vou digitar o comando

```
npm int -y
```

Este comando irá simplesmente inicializar nosso projeto e criar o pacote que usaremos para o arquivo.

Isso gerenciará todas as dependências do nosso projeto.

Se desejar, você pode pensar neste arquivo de forma semelhante a um arquivo Maven, se você estiver vindo de um ambiente Java.

![](/Users/isabelmendes/Desktop/Captura de Tela 2021-05-25 às 14.41.27.png)

Excelente. Agora que estamos prontos para instalar o Cypress, tudo o que precisamos fazer agora é digitar os comandos:

```
npm i -D cypress@4.8.0 cypress-axe@0.8.1
```

i é um atalho para instalar, -D porque queremos salvá-lo em nossas dependências de desenvolvimento neste projeto específico.

Em seguida, o nome do pacote, cypress, seguido por uma versão específica.

E, claro, também adicionaremos o pacote cypress-axe.

Eu escolhi codificar os números de versão para esses dois pacotes, então eu sei que este curso sempre funcionará no recurso no caso de novas versões apresentarem problemas de compatibilidade.

Agora, vamos apenas esperar que o processo de instalação seja concluído, e isso pode levar mais tempo para alguns, especialmente se esta for a primeira vez que você instala o Cypress.

> Nota da tradutora: os dois pacotes também podem ser instalados através dos comandos abaixo, sem danos ao projeto.

```
npm install cypress --save-dev
npm install --save-dev cypress-axe
```

 

