# Lances Vôlei

Programa para Windows que tira as pausas do vídeo de um jogo de vôlei. Sobra só a bola em jogo, pronta para assistir com os alunos ou salvar num vídeo menor para mandar pra eles.

Tudo roda no próprio computador, sem custo por jogo, e os vídeos não saem do PC. A internet só é usada para baixar jogos do YouTube.

## Como instalar

1. Baixe o [LancesVolei.zip](https://github.com/eduardoweberai-cloud/lances-volei/releases/latest/download/LancesVolei.zip).
2. Clique com o botão direito no arquivo baixado e escolha **Extrair tudo**.
3. Na pasta extraída, dê dois cliques em **Instalar**. Se o Windows avisar que protegeu o computador, clique em **Mais informações** e depois em **Executar assim mesmo**.

O programa é instalado em `%LOCALAPPDATA%\Programs\LancesVolei`, com um atalho na área de trabalho. Não precisa de administrador nem de instalar mais nada: o pacote já traz Python, ffmpeg e Node.

Precisa de Windows 10 ou 11 (64 bits) e de uns 2 GB livres para instalar, fora o espaço dos vídeos.

## Componentes

- Detecção da bola: modelo VballNet de [asigatchov/fast-volleyball-tracking-inference](https://github.com/asigatchov/fast-volleyball-tracking-inference) (MIT)
- [Python 3.14](https://www.python.org/) (PSF), [onnxruntime](https://github.com/microsoft/onnxruntime) (MIT), [yt-dlp](https://github.com/yt-dlp/yt-dlp) (Unlicense), [Node.js](https://nodejs.org/) (MIT)
- [ffmpeg](https://ffmpeg.org/), build do [gyan.dev](https://www.gyan.dev/ffmpeg/builds/) (GPLv3, código-fonte em ffmpeg.org)
