---
title: 'Use Cinza'
description: 'Na dúvida, use cinza'
pubDate: '2023-10-24'
heroImage: '/hsv_vs_rgb.png'
---

Cores sempre foram um vetor do desenvolvimento tecnológico, televisão colorida,
mais canais, a compressão posterior para transmitir esses dados... A representação
de imagens é muito querida na tecnologia na medida em que consegue transmitir algumas
ideias de forma direta e humanamente intuitivas.

No entanto, lembro de discussões na concepção do Estabiliza de cores com o chefe Pedro Duarte, e quase sempre gostávamos de cinza (ou tonalidades).
Embora designers possam ter uma explicação humana pra isso, eu acredito que nós éramos influenciados por um fator tecnológico indireto.

![color space](/ciechroma.jpg)

Color pickers normalmente apresentam um plano que inspirado no HSV, e além disso, como framework *mental* o HSV é muito mais simples.
O cinza não fica melhor necessariamente, é que é mais fácil reduzir/aumentar luz, mantendo saturação e hue ou manter os demais e reduzir saturação.

No RGB a equalização das cores não é tão clara para nós desenvolvedores e normalmente não pensamos em "adicionar vermelho, verde ou azul", pensamos na verdade em deixar mais escuro, por isso a tendência pelo monocromatismo que fica ainda mais fácil com color pickers. Que me lembre do livro do [Gonzalez](https://www.imageprocessingplace.com/), o único grande problema é a conversão para outros modelos de canais, uma vez que envolve rotação e translação em eixos espaciais cônicos.

Mas em geral, recomendo utilizar software para escolher a [paleta de cores](https://color.adobe.com/create/color-wheel).
