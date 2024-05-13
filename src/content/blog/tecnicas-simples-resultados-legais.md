---
title: 'Redução à técnica mais fácil: Superpixels e Otsu'
description: 'Revisitando um artigo da faculdade'
pubDate: '2023-10-24'
heroImage: '/multimidia_comparacao.png'
---

Embora eu seja um estudante (até o momento?), reconheço que projetos da faculdade não
são exatamente originais, mas alguns projetos que realizei simplesmente tiveram uma
exigência grande e diferente de outros que possam parecer menos bem "memoráveis" como
gigantes listas de alguma matéria difícil.

Hoje vou só relembrar um pouco deste artigo que produzi nas aulas de Multimídia com o professor Zanchetta. Em verdade vou pincelar os principais feitos e o leitor pode conferir exatamente o que fizemos no:
- [artigo](/artigo_multimidia.pdf)
- [slides](/slides_multimidia.pdf)

Nosso projeto consistiu em analisar o [artigo original](https://ieeexplore.ieee.org/abstract/document/9145240) que consistia em um método de segmentação semi-supervisionado com acurácia para decisão de lesões na pele.

Não somos especialistas, somos e éramos apenas estudantes e precisávamos fazer uma pesquisa em cima deste artigo, nossa ideia foi analisar apenas uma parte do processo: o pré-processamento. Queríamos analisar a diferença de usar superpixels (e qual quantidade adequada), de forma a encontrar máxima performance e bons resultados.

Superpixels é a aplicação de k-médias ou achar k pontos na imagem latentes de proximidade. Exemplo a seguir, observe como pontos são densamente atribuídos ao centro, mas ao redor não tão pequenos nem tão distintos.

![Segmentação em 450 superpixels de lesão de pele](/sp450.png)

Precisávamos de um método para analisar os resultados, e pensamos no método mais simples: o Otsu. Isto é, como separar as imagens em apenas 2 regiões? Usando os canais e encontrando um limiar bom o suficiente! Utilizamos outros métodos do artigo original como Chan-Vese e Active Contour para suavizar as bordas:

![Otsu e Chan-Vese](/comparacao_otsu_chan.png)

Obtivemos o Índice Jaccard e percebemos que quantidades *pequenas* de superpixels são ainda melhores que grandes quantidades, mas fincamos em 800 superpixels a quantidade que obtém menor variância com bons resultados do dataset... Mas o mais engraçado foi que o melhor resultado em verdade foi de 200 surpreendentemente (o menor valor que testamos). Na época descobrimos limitações dos métodos e ruídos, mas foi bem interessante o experimento com aplicação de k-médias na área de processamento de imagens.
