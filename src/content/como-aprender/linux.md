---
title: 'Linux'
description: 'Como aprendi linux'
---

De verdade o que me fez aprender Linux e viver no terminal sempre foi utilizar na minha máquina pessoal.

Então isso significa que não é sobre instalar uma VMzinha qualquer ou ligar seu WSL, lançar um docker. Isso é o que você faz *quando você sabe o que está fazendo*.

Quando você usa dual-boot e resolve um problema voltando pro Windows, quando você explora o terminal com o WSL ou uma VM você não aprende o ecossistema que um dev utiliza no Linux. A verdade é essa. Não interessa se você compilou alguns comandos num README, você só está curioso, você não resolve problemas.

Rodar um `dd` errado faz parte, fazer um update que zoa sua distro faz parte, entender quais passos do computador são facilmente automatizáveis só é possível se você diariamente se depara com o terminal e ferramentas de menos baixo nível e com abstrações menores.

Eu já fui sim aquele dev que tinha um `dwm` configurado com tudo no CLI e não acho isso lá tão vantagem hoje em dia. Por quê? Porque a verdade é que GUI também é boa. Os demais ecossistemas são vantajosos na medida em que promovem mais suporte (por isso não recomendo Linux para jogar principalmente multiplayer) e abstrações concretas. O problema é que nem sempre você quer esta abstração no seu caminho (você é um desenvolvedor caramba, é seu dever entender o que está por baixo delas) e nisso esses úteis ecossistemas falham: eles te bloqueiam de descer.

Agora sim, sobre as fontes e metodologias, não necessariamente nessa ordem:
- Instale na sua máquina principal. Reserve outras máquinas para trabalho/projeto ou lazer, mas não as utilize para o seu dia a dia.
- Não caia na bobagem de distro, a maioria não faz diferença. Mas vá e explore, tente outras distros, veja a diferença, veja qual te deixa mais confortável. Hoje eu acho que existem quatro válidas: [Arch](https://archlinux.org/) (atual), [Debian](https://www.debian.org/) (considerando), [Fedora](https://fedoraproject.org/) e [Ubuntu](https://ubuntu.com) (ou [Mint](https://linuxmint.com/)). A maioria das distros não fará diferença entre si a não ser que tenha algum uso específico. Tem uso específico? Procure, é assim que vai entender.
- Continue seu dia a dia no Linux. Sempre que possível tente ver soluções sem GUI.
- Abuse da [Arch Wiki](https://wiki.archlinux.org)
- Mude seu [Desktop Environment](https://wiki.archlinux.org/title/desktop_environment)
- Esqueça seu Desktop Environment, use um [Window Manager](https://wiki.archlinux.org/title/window_manager).
- Já que usa window manager, veja que existem TTY's.
- Espera um pouco... Até agora é só visual e nada de Kernel, porque eu elenquei isso tudo para um desenvolvedor? Simples: essas configurações exigem você entender pathing no linux, config files, diferentes tipos de configurações, formatos, e vai te forçar a aprender que Linux é só o Kernel, mas na prática é todo o ecossistema.
- Tente novos shells como o `zsh` e os configure. Entenda o que é um shell e o que se difere de CLI
- Explore editores de texto no CLI (vim, neovim, nano) ou próximos (emacs).
- Explore as ferramentas e os paths do seu sistema, se você ver algum trabalho manual muito forte, procure como você poderia utilizar ferramentas como `awk`, `shellscript`, `for`, `echo`, `cut`.
- Automatize backups/sincronizações com aplicativos como [rclone](https://github.com/rclone/rclone/)
- Aprenda keybinds e mais importante `tmux`
- Aprenda `ssh`, e utilize junto com `tmux`
- Explore **MAN PAGES** (utilize o man a seu favor)
- Tente mecanismos de consumo da internet por meio de comandos (`curl`, rss, `spotdl`, `yt-dlp`)
- Novamente: tente automatizar as coisas, mesmo que só use uma vez.

Ficou redundante e eu poderia explorar da vez que fiz um módulo do Kernel, mas o que eu queria de verdade mostrar é que se você utilizar o ecossistema linux e lidar ativamente com abstrações que antes o seu sistema operacional escondia de você, você vai ganhar muito conhecimento de como um sistema é organizado, de como ele é configurado e de como você pode extrair o máximo dele. Quantas "automações" eu fiz e utilizei 2 vezes? Talvez para seu dia produtivo no trabalho isso não valha a pena, mas se você tem o propósito de aprender, foram essas automações que influenciaram automações e scripts mais importantes.

Sim, eu sei que você pode usar WSL para isso, pode utilizar PowerShell e provavelmente é o mesmo efeito. A relevância de aprender desse jeito é que quando você está com o seu "escape" próximo (não usar o man, trocar de SO, trocar de ferramenta...), você vai escapar do aprendizado.

Boa sorte, qualquer coisa pode me contatar!