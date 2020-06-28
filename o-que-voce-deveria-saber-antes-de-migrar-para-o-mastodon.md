# O que você deveria saber antes de migrar para o Mastodon

*Se você está acompanhando o Twitter recentemente, deve ter ouvido falar de um tal de Mastodon. Mas o que é isso, exatamente? Vale a pena migrar do Twitter para lá, como tanta gente está sugerindo? Nesse post, entenda um pouco mais como essa plataforma funciona e por que você deveria pensar duas vezes antes de se mudar para lá!*

[**LEIA O TEXTO NO BLOG!**](https://esquer.dev/posts/o-que-voce-deveria-saber-antes-de-migrar-para-o-mastodon/)

Recentemente, no Twitter, não se fala em outra coisa: o [Mastodon](https://joinmastodon.org/) é a rede social do momento e todas as pessoas que se importam com direitos humanos, liberdade de expressão, privacidade e proteção de dados devem imediatamente fazer a migração para lá. 

Recentemente, claro, no Twitter **brasileiro**. No final de 2019, [esse mesmo movimento aconteceu na Índia](https://www.firstpost.com/india/as-outrage-over-twitter-indias-alleged-bias-grows-journalists-and-activists-migrate-to-mastodon-how-to-join-this-open-source-micro-blogging-site-7618741.html). Em 2018, [aconteceu na Espanha](https://www.elperiodico.com/es/tecnologia/20181001/mastodon-trending-topic-7065207). Em 2017, [foi com a França](https://www.numerama.com/tech/246010-decouvrez-mastodon-un-clone-de-twitter-libre-open-source-et-decentralise.html). O criador do Mastodon, Eugen Rochko, mais conhecido como [**Gargron**](https://mastodon.social/@Gargron), já está acostumado com isso: o Twitter toma uma medida questionável em relação a alguma conta ou acontecimento, a confusão vai crescendo e um grupo de usuários que se envolveram nela acaba começando um movimento de migração para o Mastodon - a grande salvação.

De fato, não foi a primeira vez que isso aconteceu com o Mastodon e, para a felicidade de Gargron, não vai ser a última. Em todas essas ocasiões, algumas pessoas avisaram: *isso não vai dar certo*, *tem alguns problemas aí* e foram, no geral, ignoradas. Não podemos falar, entretanto, que essas pessoas estavam erradas - ninguém *matou* (**nem vai matar**) *o Twitter*, afinal, e com o tempo o Mastodon foi só esquecido.

Mas como pode tamanha benção ser esquecida? Se é uma rede social **descentralizada, sem propaganda, que protege a privacidade do usuário e bane usuários que disseminam preconceitos**, como pode não dar perfeitamente certo? E por que é que eu estou enrolando tanto em vez de mandar todo mundo criar uma conta lá agora? Bem, a realidade é que esse mundo florido não existe e todas essas alegações maravilhosas do Mastodon só se sustentam como meias-verdades. 

Antes de analisarmos isso, porém, precisamos entender o básico sobre como funciona o Mastodon.

## O que é o Mastodon?

Mastodon não é exatamente uma rede social. O próprio criador prefere descrever como *uma plataforma para se criar sua própria rede social*, o que de fato é mais preciso.

O Mastodon é um sistema descentralizado **federativo**. Federativo, porque qualquer um pode criar sua própria instância do Mastodon, com suas próprias regras, e ela vai conseguir se comunicar com as outras instâncias. Descentralizado, porque cada uma dessas instâncias fica em um servidor diferente, tirando o controle dos dados dos usuários de uma mão só.

E por que é que isso não dá certo? Tá aí o ponto principal do texto - **sistemas federativos promovem uma falsa descentralização**.

Descentralização é uma das coisas mais importantes e valiosas da Internet. Exemplos como o protocolo **BitTorrent** ou a rede **Tor** mostram a descentralização funcionando com maestria: de todos, para todos.

Sistemas federativos, por outro lado, não são bem assim. Não temos todos o poder, nem temos todos o controle dos nossos dados. Basicamente, continuamos com todas as desvantagens de sistemas como o Twitter, mas ainda sem as vantagens que a centralização pode trazer. Vamos entender ponto a ponto.

## Privacidade - Quem controla seus dados?

Como o Mastodon é um sistema federativo, que funciona através de instâncias distribuídas em diferentes servidores, não há uma máquina central que armazena todos os dados dos usuários. Esses dados (tanto os dados pessoais, quanto posts e mensagens diretas) ficam, portanto, no servidor da instância que o usuário se inscreveu.

Bem, se é assim, qual a diferença da forma como o Twitter armazena os dados para como o Mastodon o faz? Ou você já estava achando que não havia diferença? Mas é claro que há, minha cara pessoa que acompanha essa postagem! Enquanto no Twitter você tem uma empresa que pode sofrer prejuízos legais milionários pelo mau tratamento de dados dos usuários, no Mastodon você tem pessoas *possivelmente* leigas, que *possivelmente* nem sabem como tratar os dados dos usuários e, *possivelmente*, nem se importam com isso.

"*Mas o Mastodon te permite escolher a instância que você quer se inscrever! Se você não confia em uma, pode trocar para outra*!" Isso é verdade, perfeito! Podemos, inclusive, definir essa escolha como fez [a pesquisadora Sarah Jamie Lewis em 2018](https://fieldnotes.resistant.tech/federation-is-the-worst-of-all-worlds/) - "***nós só estamos forçando a maior parte dos usuários a escolher um novo ditador para seus dados, sem nenhuma base real que sustente essa decisão***".

Que fique claro, não estou dizendo que você deveria confiar no Twitter. É uma empresa que visa lucro e vai continuar sendo. Mas não, eu não confio mais em uma ativista que arbitrariamente bloqueia e bane pessoas que não concordam com ela e que nem seria capaz de se responsabilizar caso houvesse algum problema.

Ué, mas qual o sentido dessa discussão, se *o Mastodon não retém dados dos usuários*? É óbvio, queridos leitores e queridas leitoras, que isso é mentira. Para entender como funciona o armazenamento de dados de uma instância do Mastodon com mais clareza, em vez de ficar nas suposições e estudo indireto, decidi por à prova - criei minha própria instância do Mastodon por um dia.

As conclusões desse teste? Começando do óbvio - as instâncias no Mastodon precisam, no mínimo, armazenar os dados que permitam ao usuário acessá-las. Isto é, **um e-mail, um nome de usuário e uma senha**, além, claro, das **postagens e mensagens diretas**.

Quanto às mensagens diretas, temos nosso primeiro problema preocupante: elas ficam salvas no banco de dados em texto plano, disponíveis para qualquer administrador da instância lerem e xeretarem o quanto quiserem.

Mas o Twitter não faz isso também? Exatamente, faz! *Continuamos com todas as desvantagens de sistemas como o Twitter, mas ainda sem as vantagens que a centralização pode trazer*. Continuamos com o mesmo problema, mas agora é uma pessoa aleatória que tem acesso a todas as suas mensagens privadas.

O problema das mensagens poderia ser resolvido com a implementação de um sistema de criptografia de ponta-a-ponta, similar ao que o WhatsApp faz com suas mensagens, de modo que somente o destinatário e o remetente de uma mensagem específica consigam lê-la. Inclusive, [há pessoas que fizeram isso em suas próprias instâncias](https://dev.to/tanker/taking-mastodon-security-to-the-next-level-part-1-encrypt-your-toots-2p00), mas não é um comportamento padrão e, sem sombra de dúvidas, é algo que a minúscula minoria dos administradores de instâncias implementarão.

Essa implementação por cima do padrão, entretanto, não é nada mais que uma gambiarra. Um dos maiores motes da descentralização é a proteção da privacidade, e isso não é possível com sistemas federativos que funcionam como o Mastodon funciona.

Uma solução maior, proposta pela própria Sarah Lewis, em seu artigo, é dividir a infraestrutura descentralizada em duas camadas. A primeira como uma forma de se preservar a privacidade dos usuários, estruturada de forma protocolada e persistente, para não ser controlada pelas aplicações. A segunda como uma forma da aplicação se comunicar com o serviço. Sugerir isso, é claro, não adianta - esse não é o objetivo do Mastodon.

As mensagens diretas não são a única coisa que os administradores de uma instância têm acesso. Bizarramente, **eles podem alterar o e-mail de uma conta para qualquer outro e-mail que quiserem, basicamente roubando a conta do usuário!** E note, eu não estou falando de um acesso direto ao banco de dados - isso é uma funcionalidade disponível no painel do administrador. Por quê? Não faço ideia.

Outro ponto importante é que **não existe arrependimento**. Você não pode confiar que apagar uma postagem de uma instância vá apagá-la de todo o Mastodon, se essa postagem já foi propagada para outras instâncias. Apagar sua conta também não adianta, nesse caso.

Podemos comparar até com o e-mail, provavelmente o maior exemplo de descentralização federativa: você pode apagar sua conta de e-mail, mas as pessoas com as quais você se comunicou anteriormente através dessa conta ainda terão acesso aos e-mails que vocês trocaram. Nesse caso, não faço julgamento nenhum, só acho importante que você, leitor, entenda no que está se metendo.

Além do mais, por padrão, as instâncias do Mastodon também coletam **o IP e "outros metadados" do usuário**, o que é compreensível para uma rede social que quer permitir ao seus administradores maior controle sobre os usuários.

A [política de privacidade do mastodon.social](https://mastodon.social/terms), uma instância específica e bem grande do Mastodon, diz que o IP e os metadados dos usuários registrados são armazenados por no máximo 12 meses. Note, porém, que **isso diz respeito a uma instância específica**. Cada instância pode controlar os dados da forma que quiser e não há padrão obrigatório que a plataforma do Mastodon defina.

## A falsa descentralização

A ideia e divulgação do Mastodon como um serviço descentralizado foi o que me atraiu de primeira. Afinal, como eu disse, reconheço a imensa importância de serviços descentralizados para a saúde da Internet atual. Depois de um pouco de pesquisa, entretanto, me decepcionei.

A primeira decepção veio com a incoerência das divulgações do Mastodon. "***Ei, olhe só essa rede social descentralizada, é só fazer o cadastro em mastodon.social***". Agora, releio esses tweets e acho até graça: **como você pode estar divulgando a descentralização se está mandando todo mundo para uma instância específica?**

De fato, essa preocupação não é sem fundamento: [de acordo com um paper apresentado na ICM 2019](http://www.eecs.qmul.ac.uk/~tysong/files/Mastodon.pdf), **aproximadamente 10% das intâncias do Mastodon concentram praticamente metade de todos os usuários**. Além disso, **a interrupção de apenas 10 instâncias poderia remover mais de 60% de todos as postagens dentro do Mastodon**.

Agora sou eu que pergunto a você, leitor: como podemos chamar isso de descentralização?

## Livre de publicidade?

A plataforma Mastodon não vem com uma ferramenta embutida para a publicação de publicidade, isso é fato. Ou seja, não há uma forma embutida na plataforma de uma empresa implantar suas publicidades em uma instância, o que é um belo ponto positivo. Afirmar que é uma rede em que não há publicidade, entretanto, não é exatamente verdade.

Não há regra nenhuma dentro do Mastodon, como plataforma, que proíba a inclusão de publicidade nas instâncias. Isto significa que qualquer instância pode publicar publicidade, seja implementando essa funcionalidade, seja (mal) usando as funcionalidades nativas do Mastodon, como os **anúncios**, que permitem aos moderadores publicarem avisos para todos os usuários dessa instância.

**Por padrão, o Mastodon não tem publicidade. Mas não é regra, e isso é importante entender.**

## Uma rede sem preconceito?

Na intensa divulgação do Mastodon no Twitter brasileiro, ele foi múltiplas vezes tratado como "***um Twitter sem nazistas***" e "***uma rede social que não permite de forma alguma preconceito, descriminação e assédio***". Ora, isso não faz sentido nenhum, e você, aclamado leitor ou aclamada leitora, já deve ter percebido.

Como uma rede descentralizada, que funciona através de instâncias e não é controlada por um único servidor, pode ter regras fixas tão definidas? Especialmente se não há uma divisão de camadas na infraestrutura do serviço, como foi explicado mais acima, como isso seria possível? **Segredo: não é.**

Quando te dizem que o Mastodon não permite preconceito, pergunte a que instância a pessoa está se referindo. Não há regras para a plataforma, as regras são definidas pela própria instância. Para ser listado no [website oficial da plataforma](https://joinmastodon.org/), a instância precisa seguir [algumas regras](https://joinmastodon.org/covenant) (como uma moderação ativa contra racismo, sexismo, homofobia e transfobia), mas **não segui-las não faz a instância deixar de existir, nem impede outras instâncias de se comunicarem com ela**.

O maior escândalo com isso foi referente ao Gab, a rede social feita por nazistas para nazistas, que os bolsonaristas adoram exaltar junto do emoji do sapinho. É, minhas caras pessoas, o Gab já foi uma instância do Mastodon.

Para o Gab, aderir ao Mastodon foi uma salvação. Os aplicativos do Gab estavam banidos da App Store e da Play Store, por motivos óbvios, e isso prejudicava bastante o potencial dessa rede nazista. Tornando-se uma instância do Mastodon, porém, esse problema era resolvido, já que existem diversos aplicativos liberados para se conectar a instâncias dentro do Mastodon.

É claro, a adesão do Gab ao Mastodon deixou muitos usuários antigos do Mastodon indignados. As pessoas exigiam que o administrador geral da plataforma, o **Gargron**, tomasse alguma medida para bloquear o domínio do Gab. A resposta dele, entretanto, foi dizer que não havia como ele fazer nada.

Sua única medida de fato foi recomendar aos administradores de grandes instâncias que bloqueassem o domínio do Gab. Muitos de fato fizeram isso, mas não era uma medida obrigatória. Inclusive, é uma medida um tanto bizarra para uma rede descentralizada federativa. Se uma instância tem o poder de bloquear a comunicação com outras instâncias específicas e ainda impedir que os usuários vejam quais instâncias estão bloqueadas (**sim, isso é uma opção**), perdemos tanto a descentralização quanto a federalização.

Mas, bem, o que é que o Gargron poderia ter feito? Ora, no mínimo transformado em padrão o bloqueio do domínio do Gab para as instâncias, o que não demandava grande trabalho. E isso ainda é uma ideia preguiçosa. **De qualquer modo, meu foco não é nas possibilidades que o criador do Mastodon perdeu, mas em seu *modus operandi* despolitizado**.

O erro na forma de pensar de Gargron fica evidente quando analisamos sua própria instância, a **[mastodon.social](https://mastodon.social)**. Gargron tentou agradar todo mundo: criar um ambiente amigável com pessoas marginalizadas, mas ao mesmo tempo que não fosse necessariamente politizado.

Isso, entretanto, não funciona. Como [uma antiga usuária do Mastodon chamada de ***voz***](https://www.dailydot.com/debug/mastodon-fediverse-eugen-rochko/) explica, essa despolitização transformou o Mastodon, um espaço já predominantemente branco, em um ambiente hostil para usuários negros.

Ficou claro - a **fixação do Gargron em se manter afastado da política tornou o ambiente do Mastodon novamente hostil para minorias e sua moderação não mais protegia corretamente esses usuários**.

## Banimentos arbitrários

Um dos propulsores da grande divulgação do Mastodon aqui no Brasil foi a ação do Twitter de banir algumas contas sem nenhum motivo concreto aparente, algo absurdo e que deve ser repudiado.

A ideia é que no Mastodon não se teria isso, afinal, é uma terra pró liberdade de expressão. Creio que não é preciso muita explicação para se entender que, em um sistema descentralizado federativo, **isso não faz sentido**.

Banimentos de usuários são decisões de administradores e moderadores de instâncias, que podem ser quaisquer pessoas. Um administrador não precisa de um motivo concreto para banir alguém, afinal, o servidor é dele.

Inclusive, como eu posso confiar em uma administradora de instância que costuma bloquear quem discute com ela? Nossa, eu morreria de medo de discordar dela dentro de sua instância, afinal, não quero ser banido! Mas se é assim, cadê a liberdade de expressão?

Muitas vezes, em instâncias maiores, os moderadores nem têm tempo e disposição para analisarem todas as denúncias que recebem. **Isso torna fácil garantir a expulsão de uma conta com uma dose de assédio direcionado**.

Se eu e meu grande grupo de amigos não gostamos de certa pessoa, que convive em certa instância conosco, nada nos impede de denunciar toda e cada postagem dela aos moderadores (e ainda xingá-la bastante nas respostas, para complementar). Pode ter certeza que chegando 50 denúncias diariamente a respeito de uma determinada conta, os moderadores não vão hesitar em banir o respectivo usuário para evitar tumultos.

## "Uma alternativa ao Vale do Silício"

Este pequeno tópico é especial para você, querida pessoa que está lendo esse texto! Para descontrair da árdua leitura e se divertir com belas gargalhadas.

Algumas pessoas andaram se referindo à plataforma do Mastodon como "***uma alternativa aos produtos do Vale do Silício***", o que chega a ser um pouco engraçado. Engraçado porque, no fim, isso não significa nada.

O projeto do Mastodon é apoiado, tanto no uso quanto financeiramente, por uma série de desenvolvedores de software brancos e ricos. Inclusive, é um dos motivos que tanto cansou usuários como a ***voz***, citada mais acima.

Além disso, diversas empresas grandes contribuíram financeiramente com a plataforma. A Samsung Next, por exemplo, [fez uma doação de 70 mil dólares ao Mastodon](https://opencollective.com/mastodon). Claro, isso não transforma o Mastodon em um Facebook nem o Gargron em um Zuckerberg. Só é tolo acreditar que é um projetinho de fundo de quintal da comunidade para a comunidade.

## A controvérsia da prostituição

A [lista de patrocinadores do Mastodon](https://joinmastodon.org/sponsors) é estranha. Me causou estranhamento assim que a vi pela primeira vez. Por quê? Porque há uma grande quantidade de empresas ligadas à fabricação e venda de produtos e brinquedos sexuais, como o [YourDoll](https://www.yourdoll.com/), que vende bonecas sexuais realistas por até quase 5 mil dólares.

O motivo disso? Não sei, nem sei se temos como saber. Mas pesquisando, achei algo que pode estar relacionado: o fato do [Mastodon ter se tornado um refúgio para a prostituição na Internet](https://www.theverge.com/2018/4/11/17188772/trump-sesta-fosta-bill-switter-sex-workers-mastodon).

Com a aprovação do projeto [FOSTA](https://en.wikipedia.org/wiki/Stop_Enabling_Sex_Traffickers_Act) (apoiado tanto pelo Partido Democrata, quanto pelo Partido Republicano), que luta pela clarificação das leis estadunidenses contra o tráfico sexual, sites como o Craigslist pararam de exibir anúncios pessoais (como os de prostitutas) e grande parte do conteúdo sexual das redes sociais foi sumindo. Tudo isso na luta pela prevenção do tráfico sexual.

Isso tudo, é claro, gerou polêmicas, já que muitas prostitutas ficaram sem ter onde divulgar seus serviços. A solução que elas encontraram foi a criação da instância [Switter](https://switter.at/about), atualmente com mais de 276 mil usuários (apesar de apenas 15 mil ativos).

Em um embate entre proteção contra tráfico sexual e espaço para divulgação de serviços de prostituição, o Mastodon serviu e aceitou perfeitamente o último lado.

## Entregando espaços importantes à direita

Enfim, encerramos a análise das especificidades do Mastodon. Agora, quero entender: **por que é que parte da esquerda insiste em entregar de mão beijada nossos espaços para a direita?**

O Twitter é uma das maiores redes sociais do mundo. Assim como o Facebook e o Instagram. E isso não vai mudar, não da noite para o dia, não com uma migração "em massa" sem sentido. Escolher deixar uma plataforma é escolher deixar outras pessoas dominarem ela para você.

Enquanto essas redes continuam gigantes, será que não vale a pena lutarmos pela maior ocupação de nosso grupo nelas? Note, não estou dizendo para você não começar a usar outros tipos de redes sociais - mas não abandone aquelas em que nós estamos, pois já somos fracos mesmo nessas.

É fácil observar como a direita trabalha bem com redes sociais. São presentes e organizados, mesmo com seus robôs, de modo a ocuparem muito do espaço. Mas esse espaço não é deles. A Internet não é deles. Devemos parar de fugir dos espaços dos quais fazemos parte e, em vez disso, fortalecer e engrandecer nossa voz dentro deles!

Resistência, camaradas.

## Por que tanto escândalo?

Depois de tudo isso, só me resta uma dúvida: por que é que o Mastodon está fazendo tanto barulho agora? Por que é que, do nada, alguns influenciadores começaram a divulgar e defender tanto o Mastodon, com unhas e dentes? Bem, eu não tenho uma resposta definitiva para isso.

Algumas hipóteses citavam dinheiro, mas não há nenhuma evidência que sustente isso. Eu acredito que é sobre poder. **Eles não são realmente contra o controle dos seus dados como o Twitter faz, eles só querem ter esse controle, e com o Mastodon essa possibilidade vem de mão beijada**. É óbvio que eles confiam neles mesmos, mas eu não. E você também não deveria.
