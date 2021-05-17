# Capítulo 3 - Verificações nos testes de Acessibilidade Web

## Verificações que podem ser automatizadas

Vejamos algumas das regras de acessibilidade que podem ser cobertas por uma ferramenta automatizada.

Uma ferramenta automatizada pode detectar se sua página não tem um **título de página**.

O título da página é importante porque é a primeira coisa que o leitor de tela diz quando um usuário visita sua página.

Sem um título de página, seus usuários ficarão confusos quanto à página em que estão, especialmente se tiverem várias guias abertas.

A próxima verificação são as **alternativas de texto de imagem**.

Uma ferramenta de teste de acessibilidade automatizada pode verificar se as imagens têm o atributo de texto alternativo.

Se você tem usuários cegos, eles dependem muito desses textos alternativos para ajudá-los a entender as imagens que não podem ver.

Uma ferramenta automatizada também pode verificar se possui a estrutura de título correta e se há algum elemento de título ausente.

Por exemplo, é recomendado que sua página tenha pelo menos um título.

Ter uma boa estrutura de títulos ajuda em como sua página será acessada usando apenas o teclado.

Semelhante ao **contraste de cor** - uma ferramenta de teste de acessibilidade pode ajudá-lo a detectar qualquer elemento em sua página que não tenha contraste de cor suficiente e pode relatar problemas preliminares básicos.

Isso é útil porque alguns usuários acharão difícil ler o texto se não houver contraste suficiente entre o texto e o fundo.

Você também pode usar uma ferramenta automatizada para detectar erros em sua **estrutura HTML**.

Por exemplo, ele pode relatar se há algum elemento ou atributo obrigatório ausente em qualquer um de seus elementos HTML.

Uma ferramenta automatizada também pode relatar problemas relacionados à falta de **rótulos ARIA** necessários.

O atributo aria-label é usado como um rótulo para elementos onde o rótulo não está visível na tela.

Isso é particularmente útil para usar leitores de tela.

Este é apenas um subconjunto, é claro, mas se você quiser saber mais informações sobre quais outras regras podem ser automatizadas, você pode verificar as regras de acessibilidade de Deque em uma das ferramentas fornecidas, que também exploraremos mais detalhes no próximo capítulo.


# Verificações que você precisa testar
Agora vamos ver quais verificações você precisa testar.

Huh ... espere ... as verificações são todas semelhantes. Achei que os testes automatizados deveriam cobrir isso.

As ferramentas automatizadas existem para ajudá-lo a detectar se esses atributos estão presentes.

Por exemplo, ele relatará se um elemento de título está lá, mas você ainda precisa verificar se o título da página faz sentido. É fácil de entender?

É semelhante com as outras regras, como as alternativas de texto de imagem.

Você pode adicionar esse atributo, mas ainda precisa verificar se o valor desse atributo faz sentido, especialmente quando está sendo usado por um leitor de tela.

Ainda precisamos verificar se a estrutura do título faz sentido usando o teclado para acessar a página.

Com o contraste de cores, você não pode simplesmente confiar no que a ferramenta está lhe dizendo. Você ainda precisa avaliar isso manualmente. A ferramenta está aqui apenas para nos orientar.

Com a estrutura HTML, você ainda precisa usar o teclado para testar se a estrutura faz sentido ao acessá-la apenas com o teclado.

E, por último, com os rótulos ARIA, você ainda precisa usar um leitor de tela para determinar se o nome do rótulo fornecido faz sentido e dá mais significado ao elemento em que está se concentrando.

Como você pode ver, a intervenção humana ainda é muito necessária se você estiver fazendo testes de acessibilidade.

A automação pode nos ajudar com problemas técnicos no início, mas não pode ser 100% confiável.

Os dos slides anteriores são apenas verificações para você começar, e há outras verificações que você também deve observar.

Por exemplo, se você tiver formulários em seu site, precisará certificar-se de que haja feedback fornecido sempre que os usuários enviarem o formulário ou cometerem erros.

As mensagens devem ser claras e fáceis de entender.

Se você tiver algum vídeo incorporado, precisa testar se as legendas estão claras e representam bem o vídeo.

Se você tiver animações, certifique-se de que haja uma opção para desativar isso, pois os usuários podem considerá-las atraentes. Dê a eles a opção de controlá-lo.

Conforme mencionado no slide anterior, você ainda precisa usar o teclado para verificar algumas das verificações automatizadas de acessibilidade, portanto, isso é muito importante ao fazer o teste de acessibilidade.

Seu teclado é uma ótima ferramenta de acessibilidade.

Quando você foca em um elemento, fica claro? Os usuários sabem que estão naquele elemento?

Seu site tem fontes claras? Certifique-se também de que o conteúdo é fácil de ler e compreender.

Se você tiver áudio ou vídeos, certifique-se de que os níveis de áudio possam ser modificados e que seus usuários possam controlá-los.

O layout é responsivo? Se eles estiverem no celular, você está exibindo a versão móvel?

Os botões ou links são grandes o suficiente? Portanto, quando estiverem usando dispositivos com portas de visualização menores, eles podem acessar facilmente.

Eu sei que existem toneladas de verificações que você pode começar a fazer, e é um bom começo ter um plano de acessibilidade em vigor.

## Dicas para fazer testes de acessibilidade

Aqui estão algumas dicas que você pode usar.

**Primeiro, decida dentro de sua equipe qual nível das Diretrizes de Acessibilidade de Conteúdo da Web você deseja alcançar**.

Se você deseja alcançar 2.1 e o Nível AA, comece no Nível A primeiro e vá subindo até o AA lentamente.

**Envolva-se com sua equipe de UX e colabore com eles.**

Use personas de usuário com base em usuários reais e use isso como um guia.

**Comece o teste em uma página básica e apenas brinque com ela**.

**Use mais o teclado e tente não usar o mouse**.

Aprenda os atalhos de teclado de que você precisa para navegar por suas páginas.

**Brinque com leitores de tela.**

Se você é um usuário Mac, o VoiceOver já vem integrado e só precisa ser ativado.

Se você estiver em uma máquina Windows, o NVDA é um dos leitores de tela mais populares que as pessoas com deficiência usam.

**Desligue os alto-falantes** e teste se há uma maneira de ativar as legendas ou legendas ocultas.

**Use uma lista de verificação de teste de acessibilidade** para ter uma ideia sobre o que rastrear e o que sugerir para suas equipes corrigirem.

**Faça testes exploratórios** e limite o tempo de suas sessões. Defina a meta que deseja alcançar.

Costumo encontrar a maioria dos bugs de acessibilidade fazendo testes exploratórios.

E, por último, **decida quais outras ferramentas podem ajudá-lo**.

Existem toneladas de ferramentas de teste de acessibilidade gratuitas por aí, e você está com sorte porque, no próximo capítulo, apresentarei uma visão geral de algumas das ferramentas que você pode usar.

