# Capítulo 2 - Por que testes de acessibilidade são importantes?

**Em primeiro lugar, fazer testes de acessibilidade é a coisa certa a fazer**.

Precisamos ter empatia com nossos usuários com deficiência e nos colocar no lugar deles.

Como cada vez mais informações podem ser acessadas online, precisamos começar a pensar sobre como todos os nossos usuários usarão nossos produtos.

É importante incluir a todos e isso não beneficia apenas os indivíduos, mas a sociedade como um todo.

**Melhor acessibilidade significa melhor experiência do usuário.**

Por exemplo, se você estiver testando um site com excelente design, animações e todos esses recursos interessantes, mas acessibilidade ruim, isso resultará em uma experiência ruim para o usuário.

Portanto, seu trabalho como testador é ajudar sua equipe a encontrar diferentes problemas de acessibilidade para que você possa ajudar a entregar um produto de alta qualidade.

Freqüentemente, o teste de acessibilidade costuma ser visto como uma reflexão tardia, somente depois que um produto foi implantado para produção.

Algo que funciona funcionalmente não significa necessariamente acessível, portanto, precisamos ter certeza de que também consideramos a experiência do usuário.

**Melhor acessibilidade também significa que você amplia seu alcance para outros públicos.**

Lembro-me de quando a Microsoft lançou o Edge anos atrás e o tornou seu navegador padrão no Windows 10.

Eu estava lendo artigos que diziam que o navegador Edge antigo não era compatível com dispositivos de tecnologia assistiva, o que significa que os cegos na época não podiam acessar o navegador Edge durante seu lançamento inicial porque não era compatível.

Agora, tanto a NV Access, uma organização sem fins lucrativos que é responsável por trazer o software de leitura de tela NVDA, quanto a Microsoft têm trabalhado em conjunto para garantir que o novo navegador Edge esteja acessível para que também possam alcançar usuários cegos.

Se você quiser saber mais sobre esta história, adicionei um link abaixo para um artigo do NV Access, que você pode encontrar na seção de recursos que pode achar relevante.

No capítulo anterior, você aprendeu sobre o caso de acessibilidade do Dominos.

A lei sobre acessibilidade difere de um país para outro, então é melhor verificar os regulamentos de seu país primeiro.

É melhor evitar ações judiciais em primeiro lugar, pois isso causará dores de cabeça e desperdício de dinheiro para quem está sendo processado.

## Como os testes de acessibilidade automatizados podem nos ajudar?

Com a quantidade de verificações de acessibilidade diferentes que precisamos fazer, faz sentido automatizar algumas das verificações e adicioná-las como parte de nosso pacote de regressão automatizado.

Ao automatizar alguns dos testes de acessibilidade, podemos detectar problemas básicos de acessibilidade com antecedência e nos permite colaborar mais com nossa equipe de design e desenvolvimento.

Isso também pode servir como uma documentação viva para sua equipe.

Por exemplo, se sua equipe está tentando ativamente reduzir o número de problemas de acessibilidade em seu site, ter um painel que exibe um relatório da execução de teste servirá como documentação e deixará todos cientes dos problemas que ainda estão pendentes.

O próximo benefício é, creio eu, um dos mais importantes: evitará que quaisquer problemas de regressão relacionados à acessibilidade sejam implantados na produção.

Com os testes automatizados em vigor, você tem essa rede de segurança que os problemas que sua equipe corrigiu no passado não serão implantados na produção novamente, pois agora é coberta por um teste automatizado.

Ele também libera seu tempo para fazer atividades de teste mais complexas, como testar com leitores de tela ou usar o teclado apenas para navegar em um site.

Embora os testes de acessibilidade automatizados detectem apenas um subconjunto dos problemas de acessibilidade existentes, ainda é benéfico tê-los porque nos ajudará a acelerar nosso processo de teste e são baratos para executar.

Por último, ter testes de acessibilidade automatizados fornece um loop de feedback rápido para sua equipe de design e desenvolvimento, especialmente se os testes estiverem sendo executados como parte de seu pipeline de integração contínua.

Sua equipe de desenvolvimento saberá imediatamente se o recurso em que está trabalhando violou alguma regra de acessibilidade.

Da mesma forma, se houver algum erro de contraste de cor detectado, a equipe de design pode ser informada se precisar alterar qualquer um dos tokens de cor escolhidos.

Não é uma bala de prata, é claro, então você não deve usar todos os seus esforços de teste de acessibilidade apenas em testes de acessibilidade automatizados.

Não existe uma ferramenta automatizada de acessibilidade que possa detectar todos os problemas de acessibilidade e só porque sua ferramenta não relatou um problema de acessibilidade em uma regra específica, não significa que ela está acessível.

Eu adicionei um link para uma postagem de blog do governo do Reino Unido onde eles usaram diferentes ferramentas de teste de acessibilidade para testar a página da web menos acessível, que eles criaram como parte desse experimento.

Você pode encontrá-lo na seção de recursos abaixo e eu recomendo fortemente que você leia, se ainda não o fez.

Aqui, eles usam 10 ferramentas diferentes para ajudá-los a detectar problemas de acessibilidade e apenas uma média de 40% dos problemas foram detectados por essas ferramentas.

Isso só prova que a intervenção humana ainda é muito necessária quando se trata de testes de acessibilidade.

## A importância de fazer testes de acessibilidade com usuários reais

Com isso dito, nada supera o teste de acessibilidade real com usuários reais.

Você pode ter todos os testes automatizados de que precisa e até mesmo fazer alguns dos testes você mesmo, mas ainda há muitos benefícios a ganhar se convidar usuários reais com deficiências para testar seu site.

A razão é que eles provavelmente usam diferentes tecnologias assistivas de terceiros e, dessa forma, você tem o conhecimento de primeira mão sobre como eles usam seu produto no dia-a-dia.

Envolva-os quando sua equipe estiver projetando e desenvolvendo um novo recurso.

Eles podem fornecer informações valiosas sobre como tornar seu recurso acessível.

Dito isso, se você pretende obter o envolvimento do usuário, certifique-se de envolver diferentes pessoas com deficiência para obter melhores resultados.

Uma pessoa pode usar uma tecnologia de assistência diferente das outras, então é melhor não depender da opinião de uma pessoa.

Fazer testes de acessibilidade com usuários reais, bem como fazer uma lista de verificação de avaliação, que pode ser conseguida com testes de acessibilidade automatizados e verificando-os você mesmo, é a melhor abordagem para garantir que seu site ou aplicativo seja acessível a usuários com diferentes deficiências.

O bom é que o W3C forneceu um gerador de relatório de avaliação que você pode usar para sua avaliação, que eu vinculei abaixo na seção de recursos.

Mergulhar em testes de acessibilidade pode ser um desafio.

Mesmo comigo mesmo, ainda estou aprendendo muito sobre acessibilidade no dia a dia e espero que, ao fazer este curso, isso sirva como um ponto de partida para o seu aprendizado de acessibilidade.

No próximo capítulo, veremos algumas das verificações de teste de acessibilidade que você pode introduzir como parte de seu processo de teste.

