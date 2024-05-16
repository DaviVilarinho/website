---
title: 'Python'
description: 'Como você pode aprender python'
---

Bom eu sou suspeito, eu era de Economia em 2019 quando descobri o Python.

No início eu achei que eu ia mudar o mundo, eu fazia contas e algoritmos (simplórios de iniciante) que eu achava que era a automação da minha carteira. Muita coisa aprendi, mas na medida que fui aprendendo Python eu também mudei umas visões da carteira então ficou como aprendizado de automação e consumo de API/páginas.

Mas vamos ao que interessa. Python é uma linguagem interpretada. Sabe o que isso significa, bagre? Que não tem que compilar. Pra quem não é do ramo a diferença pode ser simplificada em:
- Existem linguagens que o seu computador entende "de uma vez" ou quase os comandos que são passados. Isso não necessariamente significa que você tem que escrever o que o computador entende, mas só deixar pronto de alguma forma isso para ele entender no momento que você executar.
- Existem linguagens que algum programa sabe falar pro computador o que é pra ele fazer, mas você fala pra ele outra coisa, como se fosse um tradutor, um *interpretador*.

Isso já explica uma coisa: Python não é bom se você quer falar direto pro PC. Não quero começar uma guerra aqui, eu gosto muito de Python, Python vai ser muito útil pra você, mas se você quer montar um app, um back-end sólido e potente ou mesmo frameworks matemáticos pesados... Não será com isso que você vai fazer viu...

Mas não desanime! Você pode *usar* essas coisas com Python. Python é importante porque é a cola entre sistemas, é aquele canivete multiferramenta salvador, sua caixa de ferramentas preparadas para um monte de problemas difíceis.

Primeiro, eu comecei assistindo tutoriais, mas o *disclaimer* é que eu não sabia programar nada né. Eu comecei assistindo esse curso do [Inteligência Zero](https://www.youtube.com/watch?v=lJjR906426o&list=PLfCKf0-awunOu2WyLe2pSD2fXUo795xRe), e hoje em dia sei que o [Backes](https://www.youtube.com/watch?v=GDCtOyEY1jc&list=PL8iN9FQ7_jt5TITT-3c4L6xNSmQMx1T4e&pp=iAQB) também fez alguns vídeos legais que já dei uma olhada, bem como também li [Python Crash Course](https://nostarch.com/python-crash-course-3rd-edition). Mas honestamente, cursos são ótimos, mas você precisa enxergar usos simples que ajudem sua vida, e eu recomendo isso acima de tudo.

Outra abordagem, embora não tenha seguido diretamente do livro, era a do [Automate the Boring Stuff](https://automatetheboringstuff.com/), mas o conceito é esse mesmo: **AUTOMATIZE AS COISAS CHATAS**. Hoje em dia tem embutido no Excel, utilize se for necessário. Use para consumir API's e criar valores, criar documentos, parsear csv's, mandar mensagens, fazer backups...

Algumas coisas que já fiz:
- Quando comecei, eu tinha um método de analisar ações de empresas com alguns fundamentos. E era bem chato e bem calculado. Então eu fiz o seguinte: traduzi isso numa função `get_invesment_possibility(stock)` em que tinha alguns atributos das empresas como endividamento, lucro por ação, preço, liquidez... E eu rankeava ela em alguns status de 0 a 10 por exemplo. Se o valor fosse a partir de um threshold eu ia e printava num diretório que eu usava bastante, para que eu visse depois. Eu tirei completamente meu trabalho de ir lá nos brokers para já ter ideia de quais ações eu realmente deveria me importar. Não uso mais porque eu mudei de estratégia financeira. Aqui foi bom porque numa tacada só aprendi operações com `file`, `csv`, e a linguagem de forma geral.
- Da mesma forma, não é fácil você fazer a automação acima sem automatizar o consumo das ações. No início eu era muito cavalo e na força do Go Horse eu *consumia as páginas na mão*. Sim, não ria. Mas isso foi bom pro aprendizado, aprendi libs como [BeautifulSoup](https://beautiful-soup-4.readthedocs.io/en/latest/), `requests` e depois o conceito de API e consumi-las também.
- Ainda depois, aprendi um pouco de análise de dados quando tinha grandes datasets. Mais uma vez, Python se mostrou muito útil e você poderia usar para *seus* use cases juntamente com bibliotecas como [numpy](https://numpy.org/) e [pandas](https://pandas.pydata.org/). Use nos seus datasets, tente enxergar padrões, traduza seus problemas em dados para tentar encontrar melhores soluções. Finanças, carros, orçamento, casas, produtividade...
- Aqui já começa a esquentar. Até agora era a visão de um protoeconomista entusiasta de computação e que tava na espera do Sisu soltar a nota de corte, mas depois essas coisas pagaram seus dividendos. Python é muito bom para scripts diários e contato com outras aplicações. Existem programas configuráveis com python como [quteBrowser](https://www.qutebrowser.org/) e [qtile](https://qtile.org/).
- Leatcode é muito bom em python. Ponto. Quaisquer problemas de computação prefira em python. Existem ótimas bibliotecas de consumo e é muito fácil você aprender noção de computação com uma linguagem que estimula ser one file do que um projeto.
- Aliás dito o anterior, code python **SEM** gerar projeto. Evite IDE. Não é que IDE são ruins, mas é que Python é tão bom como ferramenta, que é como se guardasse um canivete numa mochila e não no bolso. Você teria que carregar essa mochila toda hora para o peso de uma ferramenta tão útil e pequena.
- Automatize Backups. Python tem libs à rodo para a maioria das clouds, para zippar ou criar tarballs, use isso a seu favor, elimine o problema da integridade do sistema com inteligência.
- Crie rotinas simples. Na Exacode Python era nosso entrypoint de um monte de contêineres AWS. Um monte de automações do sistema e integrações era Python. A API Java rodava em Lambdas que não permitiam mais que 15 minutos, resultado: chama um contêiner com código Python e ele resolve. Fazíamos disparo em massa, queries avançadas, backups, builds e orquestrações com Python, e isso seria muito útil para você.
- Crie uma API leve, igualmente o item passado, use [Flask](https://flask.palletsprojects.com/en/3.0.x/) ou [Fast API](https://fastapi.tiangolo.com/) para API's internas! Uma coisa rápida, que serve de entreposto entre uma API robusta e um sistema interno que não quer que sobrecarregue a API principal e por aí vai. É igual disse: a cola perfeita, simples e fácil de implementar.

Então era isso que eu tinha para deixar para você, em Python você vai aprender automatizando e dando uso para cenários do seu dia a dia. Cursos serão bons ou para te dar noção de computação ou algum projeto, mas a maioria das coisas você aprenderá resolvendo problemas que o Python tão facilmente te permite resolver.
