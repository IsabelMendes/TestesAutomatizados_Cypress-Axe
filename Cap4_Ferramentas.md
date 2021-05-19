# Capítulo 4 - Ferramentas para testes

As ferramentas que incluí neste curso são apenas um subconjunto e não incluem tudo, porque existem toneladas de ferramentas disponíveis por aí.

No entanto, as ferramentas que vou mencionar devem ajudá-lo a começar.

Vou categorizar as diferentes ferramentas de teste de acessibilidade em três categorias, sobre as quais falarei em diferentes subcapítulos.

1. Ferramentas que requerem assistência humana

2. Ferramentas semiautomáticas na forma de extensões de navegador

3. Ferramentas automatizadas que você pode adicionar em sua base de código e executar como parte de seu pipeline de CI

## Ferramentas que requerem assistência humana

Vamos primeiro dar uma olhada nas ferramentas que requerem assistência humana. Como mencionei no capítulo anterior, você precisa verificar se o seu site pode ser acessado pelo teclado.

Portanto, a primeira ferramenta de teste que pode ajudá-lo a testar a acessibilidade é o seu próprio teclado.

Aqui estão alguns dos atalhos comuns que você pode começar a usar e talvez já conheça alguns deles.

- **ctrl** ou **cmd**, se você for um usuário do Mac, **+ L** colocará o foco na barra de endereço do seu navegador, para que você possa navegar para qualquer site que desejar.

- **tab** é usada para ir para elementos específicos, como links ou botões.

- Pressionar **shift** antes de **tab** simplesmente inverte a direção, para que você possa voltar aos links ou botões anteriores.

- Teclas de seta, é claro, para rolar para uma janela de exibição específica.

- E você também pode usar a barra de espaço para marcar ou desmarcar caixas de seleção ou botões.

- A tecla **enter** também pode ser usada para ativar botões ou links atualmente em foco.


Tenho uma atividade quebra-gelo que você pode experimentar.

Escolha um site que goste de usar e, em seguida, usar apenas o teclado para navegar por ele. 

Em seguida, usar as teclas de atalho do teclado comuns que mencionei anteriormente. Veja se consegue usá-lo sem usar o mouse .

Espero que tenham gostado dessa pequena atividade e conseguido acessar o site de sua escolha sem problemas, espero.

### Screen Readers - Leitores de Tela

A próxima ferramenta que quero apresentar a vocês é o leitor de tela.

Um leitor de tela permite que pessoas com deficiência - especificamente aquelas com deficiência visual - usem um computador.

Ele traduz tudo o que um usuário normalmente vê em sua tela em fala.

Existem muitos leitores de tela que você pode usar para testar, mas aqui estão alguns dos mais populares.

Se você é um usuário de Mac e iPhone, o **VoiceOver** já vem integrado e você só precisa habilitá-lo, o que demonstrarei rapidamente adiante.

**NVDA** e **JAWS** são os dois leitores de tela mais populares para Windows.

O NVDA é uma ferramenta gratuita, enquanto o JAWS é paga.

E, por último, você também tem o leitor de tela **TalkBack** para Android.

Para habilitar o VoiceOver, basta acessar as Preferências do Sistema e selecionar o ícone Acessibilidade.

A partir daí, clique em VoiceOver e simplesmente habilite-o.

Depois de habilitado, você deve começar a ouvir uma voz lendo as descrições dos elementos da página.

Alternativamente, você também pode pressionar **cmd + F5** para ativar e desativar o VoiceOver.

Depois de habilitado, você pode definir seu atalho de teclado para usar o teclado do VoiceOver.

No meu caso, é a tecla **Control + Option**.

Quando quiser consultar os comandos do teclado que vai usar, basta digitar **ctrl + opção + H**, e isso deve mostrar a Ajuda do VoiceOver.

A partir daqui, você pode acessar o Guia do usuário, Comandos gerais e Ajuda do teclado.

Portanto, se você estiver se perguntando qual atalho usar, basta iniciar a Ajuda do VoiceOver e encontrar o comando de que precisa.

Quando terminar, basta pressionar o botão **esc**.

Para mostrar a vocês uma rápida demonstração, abri o site da Deque e percebi que toda vez que focalizo um elemento, uma descrição está sendo lida.

É por isso que é importante usar a estrutura de título, rótulos e descrições corretos, porque isso é o que o leitor de tela lerá em voz alta.

O impacto de não haver texto alternativo é que a descrição não fará sentido para as pessoas que usam leitores de tela.

Se seus usuários têm baixa visão, eles também usarão um recurso de zoom para ampliar o conteúdo, para que possam lê-lo melhor.

Quando eles ampliam o conteúdo do seu site, você precisa ter certeza de que os elementos estão se ajustando bem, e não uns sobre os outros, e que tudo está fluindo bem.

Em alguns casos, quando você aumenta muito o zoom, se um site tiver sido mal projetado, ele pode se tornar ilegível e, portanto, não muito acessível.

Para demonstrar o recurso de zoom, estou usando o site da Deque novamente.

E como sou um usuário Mac, para aumentar o tamanho do conteúdo, preciso pressionar **cmd** e a tecla **+**.

Isso seria equivalente à tecla **ctrl** e **+**, se você estiver no Windows.

O menu desmoronou assim que aproximei o zoom.

Depois de expandida, a navegação ainda é totalmente acessível.

Olhando para isso, você pode ver que todos os elementos estão se agrupando perfeitamente e o conteúdo ainda é muito legível.

Vamos fazer uma pausa rápida. E no próximo subcapítulo, vamos dar uma olhada em algumas extensões de navegador que você pode usar para ajudá-lo a detectar problemas de acessibilidade rapidamente.

## Ferramentas para testes semi-automáticas

### Axe

Vamos começar com Axe.

A extensão do navegador Axe é uma ferramenta baseada na biblioteca ax-core, que atualmente é apoiada pela Deque Systems.

Ele permite que você detecte qualquer problema de acessibilidade rapidamente apenas executando a extensão, esteja você usando o Chrome, Firefox ou Edge.

Eu adicionei o link de download da extensão do Chrome à seção de recursos abaixo, se você quiser adicionar como uma extensão do navegador.

Uma vez instalado, clique em F12 ou clique em Inspecionar. Em seguida, clique na guia "axe- DevTools" com o botão direito e em "Scanear toda página".

Em seguida, será mostrado o relatório de acessibilidade.

Eu executei a verificação no site de Deque e, sem surpresa, eles têm zero violações, o que é esperado.

Agora, vamos escolher um site diferente, como Stack Overflow, e executar a auditoria novamente.

Como você pode ver, as violações são agrupadas e também é mostrado o número de ocorrências para cada uma das violações ocorridas.

Ele fornece este relatório interessante que mostra qual elemento é afetado e qual é o problema de acessibilidade, bem como você pode corrigir esse problema.

Ele também mostra seu impacto e um link externo para mostrar mais informações sobre o assunto.

### Wave

Semelhante ao Axe, você também pode usar WAVE, que é outra ferramenta gratuita e que permite executar verificações de acessibilidade com suas extensões do Chrome.

Novamente, fique à vontade para baixar a extensão, que também incluí no link abaixo para sua referência.

Quando instalado, clique no ícone do WAVE.

Será gerado um relatório que mostra uma análise dos erros de acessibilidade, se houver, seus recursos de acessibilidade, elementos estruturais e também inclui quantos rótulos ARIA a página possui.

Em seguida, na própria página, serão mostrados ícones diferentes, destacando onde estão os problemas e os recursos de acessibilidade.

Clico no botão Exibir detalhes e, em seguida, se você clicar em qualquer um dos ícones, ele destacará qual elemento tem o erro.

Ao clicar em uma referência, você verá os detalhes de qual é o erro e porque é importante resolver o problema.

Também há uma opção para selecionar o código e onde adicionar a correção.

Você também pode inspecionar problemas de contraste de cor no WAVE.

Se você clicar em um dos ícones, será mostrado porque ele falhou.

Para que uma regra de contraste de cor seja aprovada, o texto normal deve ter uma proporção de pelo menos 4,5: 1 de primeiro plano para fundo e de pelo menos 3: 1 para texto grande.

### Google Lighthouse

Por último, o Google Lighthouse, que já vem integrado se sua versão do Chrome estiver atualizada, também inclui verificações de acessibilidade.

O recurso de acessibilidade deles está usando ax-core como mecanismo, mas o que é ótimo é que você também pode medir outras métricas, como desempenho, práticas recomendadas e SEO.

Para executar o Lighthouse, basta abrir suas ferramentas de desenvolvedor e encontrar a guia Lighthouse.

Quando estiver lá, você pode optar por executá-lo na versão desktop ou móvel.

Vamos clicar em Gerar relatório e então esperar que o Lighthouse escaneie a página inteira.

Depois de concluído, ele fornece essas diferentes pontuações e ao clicar em acessibilidade irá redirecionará para a seção de acessibilidade.

Gosto do fato de eles terem mencionado que apenas um subconjunto de problemas pode ser detectado automaticamente, então isso incentiva a importância de não depender totalmente disso.

Quando você expande uma das violações são mostrados quais os elementos com falha.

Também gosto que mostram as auditorias anteriores, o que é ótimo.

Portanto, antes de terminarmos este capítulo, tenho outra atividade para você, da qual espero que participe novamente.

Desta vez, quero que você use uma das extensões de navegador que mencionei e a use para encontrar quaisquer problemas de acessibilidade no site de sua escolha.

É ótimo se familiarizar com essas extensões de navegador e essa é uma maneira fácil de começar a testar a acessibilidade.

Quando terminar, iremos para o próximo subcapítulo e, em seguida, examinaremos algumas das ferramentas automatizadas para acessibilidade.

## Ferramentas para testes automatizados

A última parte deste capítulo é falar sobre ferramentas automatizadas de acessibilidade que você pode integrar em sua base de código e em seu pipeline de CI.

Novamente, as ferramentas que você verá aqui são apenas um subconjunto.


### Axe-Core
Uma das ferramentas automatizadas de teste de acessibilidade mais populares é o Axe-Core.

Você viu anteriormente que o Axe também tem uma extensão de navegador que você pode usar.

Se você deseja detectar problemas de acessibilidade de maneira automatizada, pode usar diferentes bibliotecas baseadas no Axe-Core.

A filosofia do Axe-Core é capacitar os desenvolvedores, e também os testadores de software, a pensar sobre acessibilidade, integrando testes automatizados o mais cedo possível.

Existem vários projetos por aí que são desenvolvidos com base no Axe-Core; como o Axe CLI, que permite executar testes de acessibilidade diretamente na linha de comando, que examinaremos de perto no próximo capítulo.

O Axe-Core também pode ser integrado às ferramentas de teste de sua escolha, como Jest para teste de unidade, Cypress, Selenium, com Java, C# e Python, WebdriverIO e até mesmo TestCafe.

Você pode encontrar a lista completa de projetos que estão usando Axe-Core nos links abaixo.

Nos próximos capítulos, vou me concentrar mais em como integrar o Axe aos testes com Cypress.

Por fim, a Applitools, fornecedora líder de testes visuais modernos entre navegadores, também lançou seu suporte para acessibilidade automatizada por meio do Contrast Advisor.

Sua IA visual pode ajudá-lo a identificar potenciais violações de contraste de cor, e você pode alternar entre diferentes diretrizes de acessibilidade de conteúdo da web, como 2.0 ou 2.1, e também diferentes níveis de conformidade.

Falarei um pouco mais detalhadamente sobre o Contrast Advisor do Applitools no capítulo final. Sei que este capítulo inteiro foi muito longo, então falarei sobre Axe CLI, Cypress-Axe e o Applitools Contrast Advisor em capítulos futuros.

Espero que tenha dado uma ideia de quantas ferramentas você pode usar, para ajudá-lo a começar com os testes de acessibilidade.

Nenhuma das ferramentas que mencionei irá substituí-lo, quando se trata de fazer esse tipo de teste; em vez disso, eles estão aqui para ajudá-lo.