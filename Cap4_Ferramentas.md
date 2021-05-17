# Capítulo 4 - Ferramentas para testes

As ferramentas que incluí neste curso são apenas um subconjunto e não incluem tudo, porque existem toneladas de ferramentas disponíveis por aí.

No entanto, as ferramentas que vou mencionar devem ajudá-lo a começar.

Vou categorizar as diferentes ferramentas de teste de acessibilidade em três categorias, sobre as quais falarei em diferentes subcapítulos.

1. Ferramentas que requerem assistência humana

2. Ferramentas semiautomáticas na forma de extensões de navegador

3. Ferramentas automatizadas que você pode adicionar em sua base de código e executar como parte de seu pipeline de CI

## Ferramentas que requerem assistência humana

Tudo bem, então vamos primeiro dar uma olhada nas ferramentas que requerem assistência humana. Como mencionei no capítulo anterior, você precisa verificar se o seu site só pode ser acessado pelo teclado.

Portanto, a primeira ferramenta de teste que pode ajudá-lo a testar a acessibilidade é o seu próprio teclado.

Aqui estão alguns dos atalhos comuns que você pode começar a usar e talvez já conheça alguns deles.

**ctrl** ou **cmd**, se você for um usuário do Mac, **+ L** colocará o foco na barra de endereço do seu navegador, para que você possa navegar para qualquer site que desejar.

**tab** é usada para ir para elementos específicos, como links ou botões.

Pressionar **shift** antes de **tab** simplesmente inverte a direção, para que você possa voltar aos links ou botões anteriores.

Teclas de seta, é claro, para rolar para uma janela de exibição específica.

E você também pode usar a barra de espaço para marcar ou desmarcar caixas de seleção ou botões de rádio.

A tecla **enter** também pode ser usada para ativar botões ou links atualmente em foco.

Tenho uma atividade quebra-gelo que você pode experimentar.

Se você escolher um site que goste de usar e, em seguida, usar apenas o teclado para navegar por ele e, em seguida, usar os atalhos de teclado comuns que mencionei no slide anterior, veja se você pode usá-lo da mesma forma, sem usar o mouse .

Simplesmente pause este vídeo e gaste alguns minutos fazendo esta atividade para se sentir confortável usando apenas o teclado.

Quando terminar, basta clicar no botão Play e veremos outras ferramentas que você pode usar.

Espero que tenham gostado dessa pequena atividade e conseguido acessar o site de sua escolha sem problemas, espero.

### Screen Readers

De qualquer forma, a próxima ferramenta que quero apresentar a vocês é o leitor de tela.

Um leitor de tela permite que pessoas com deficiência - especificamente aquelas com deficiência visual - usem um computador.

Ele traduz tudo o que um usuário normalmente vê em sua tela em fala.

Existem muitos leitores de tela que você pode usar para testar, mas aqui estão alguns dos mais populares.

Se você é um usuário de Mac e iPhone, o **VoiceOver** já vem integrado e você só precisa habilitá-lo, o que demonstrarei rapidamente no próximo slide.

**NVDA** e **JAWS** são os dois leitores de tela mais populares para Windows.

O NVDA é uma ferramenta gratuita, enquanto o JAWS é comercial.

E, por último, você também tem o leitor de tela **TalkBack** para telefones Android.

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

É por isso que é importante usar a estrutura de título correta, os rótulos e descrições corretos, porque isso é o que o leitor de tela leria em voz alta.

O impacto de não haver texto alternativo é que a descrição não fará sentido para as pessoas que usam leitores de tela.

Se seus usuários têm baixa visão, eles também usariam um recurso de zoom para ampliar o conteúdo, para que possam lê-lo melhor.

Quando eles ampliam o conteúdo do seu site, você precisa ter certeza de que os elementos estão se empilhando bem, e não uns sobre os outros, e que tudo está fluindo bem.

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

Uma vez instalado, apenas clique com o botão direito, clique em Inspecionar e, em seguida, clique na guia "machado".

Em seguida, clique no botão Analisar e, em seguida, será mostrado este relatório de acessibilidade.

Eu executei a verificação no site de Deque e, sem surpresa, eles têm zero violações, o que é esperado.

Agora, vamos escolher um site diferente, como Stack Overflow, e executar a auditoria de machado novamente.

Como você pode ver, as violações são agrupadas e também mostra o número de ocorrências para cada uma das violações ocorridas.

Ele fornece este relatório interessante que mostra qual elemento é afetado e qual é o problema de acessibilidade, bem como como você pode corrigir esse problema.

Ele também mostra seu impacto e um link externo para mostrar mais informações sobre o assunto.

### Wave

Semelhante ao Axe, você também pode usar WAVE, que é outra ferramenta gratuita que você pode usar e que permite executar verificações de acessibilidade com suas extensões do Chrome e do navegador.

Novamente, fique à vontade para baixar a extensão, que também incluí no link abaixo para sua referência.

Quando instalado, clique com o botão direito e selecione WAVE.

Será gerado um relatório que mostra uma análise dos erros de acessibilidade, se houver, seus recursos de acessibilidade, elementos estruturais e também inclui quantos rótulos ARIA a página possui.

Em seguida, na própria página, ela será anotada com ícones diferentes, destacando onde estão os problemas e os recursos de acessibilidade.

Simplesmente clico no botão Exibir detalhes e, em seguida, se você clicar em qualquer um dos ícones, ele destacará qual elemento tem o erro.

Ao clicar em uma referência, você verá os detalhes de qual é o erro e por que é importante resolver o problema.

Também há uma opção para selecionar o código - basta clicar no código e isso irá destacar o próprio código, para que você saiba onde adicionar o texto alternativo para este exemplo.

Você também pode inspecionar problemas de contraste de cor no WAVE.

Se você clicar em um dos ícones aqui, será mostrado por que ele falhou.

Para que uma regra de contraste de cor seja aprovada, o texto normal deve ter uma proporção de pelo menos 4,5: 1 de primeiro plano para fundo e de pelo menos 3: 1 para texto grande.

### Google Lighthouse

Por último, o Google Lighthouse, que já vem integrado se sua versão do Chrome estiver atualizada, também inclui verificações de acessibilidade.

O recurso de acessibilidade deles está usando ax-core como mecanismo, mas o que é ótimo é que você também pode medir outras métricas, como desempenho, práticas recomendadas e SEO.

Para executar o Lighthouse, basta abrir suas ferramentas de desenvolvedor e encontrar a guia Lighthouse.

Quando estiver aqui, você pode optar por executá-lo na versão desktop ou móvel.

Vamos clicar em Gerar relatório e então esperar que o Lighthouse escaneie a página inteira.

Depois de concluído, ele fornece essas diferentes pontuações e clicar em acessibilidade o redirecionará para a seção de acessibilidade.

Gosto do fato de eles terem mencionado que apenas um subconjunto de problemas pode ser detectado automaticamente, então isso incentiva a importância de não depender totalmente disso.

Quando você expande uma das violações, isso mostra quais são os elementos com falha.

Também gosto que mostre as auditorias anteriores, o que é ótimo.

Portanto, antes de terminarmos este capítulo, tenho outra atividade para você, da qual espero que participe novamente.

Desta vez, quero que você use uma das extensões de navegador que mencionei e a use para encontrar quaisquer problemas de acessibilidade no site de sua escolha.

É ótimo se familiarizar com essas extensões de navegador e essa é uma maneira fácil de começar a testar a acessibilidade.

Então, vá em frente e pause este vídeo. Quando terminar, iremos para o próximo subcapítulo e, em seguida, examinaremos algumas das ferramentas automatizadas para acessibilidade.

## Ferramentas para testes automatizados

A última parte deste capítulo é falar sobre ferramentas automatizadas de acessibilidade que você pode integrar em sua base de código e em seu pipeline de CI.

Novamente, as ferramentas que você verá aqui são apenas um subconjunto.


### Axe-Core
Uma das ferramentas automatizadas de teste de acessibilidade mais populares é o Ax-Core.

Você viu nos slides anteriores que Ax também tem uma extensão de navegador que você pode usar.

Se você deseja detectar problemas de acessibilidade de maneira programática, pode usar diferentes bibliotecas baseadas no Ax-Core.

A filosofia do Ax-Core é capacitar os desenvolvedores, e também os testadores de software, a pensar sobre acessibilidade, integrando testes automatizados o mais cedo possível.

Existem tantos projetos por aí que são desenvolvidos com base no Ax-Core; como o Ax CLI, que permite executar testes de acessibilidade diretamente na linha de comando, que examinaremos de perto no próximo capítulo.