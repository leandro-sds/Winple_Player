# Winple Player

Um player de áudio e vídeo acessível para Windows, no estilo Winamp
clássico.
Feito para ser usado inteiro pelo teclado, com foco em quem usa leitor
de tela.

**[⬇️ Baixar a última versão](../../releases/latest)**

---

## O que ele faz

- **Toca suas músicas** — MP3, WAV, OGG, FLAC, M4A, AAC, WMA, Opus,
  APE, MPC, WavPack, TTA, OptimFROG e MIDI
- **Toca vídeos** — MP4, MKV, AVI, MOV, WMV, WebM e outros, com troca
  de áudio e legenda (F2 e F3), tela cheia (F11) e o som passando pelo
  equalizador e pelos plugins VST
- **Biblioteca** — suas músicas por artista, álbum, gênero e ano, com
  busca (Ctrl+M)
- **Arquivos compactados** — abre ZIP, RAR, 7z e TAR e toca o que está
  dentro, sem deixar nada acumulado no computador (Ctrl+Alt+L)
- **Toca rádios da internet** — Icecast, Shoutcast e HLS, sem cortes
- **Podcasts** — cadastre pelo feed RSS ou importe de outro aplicativo
  (OPML), ouça direto da internet ou baixe os episódios; o programa
  lembra onde cada episódio parou
- **Rádios favoritas** — cadastre as suas e troque entre elas com B e Z,
  como num radinho
- **Pastas favoritas** — guarda o caminho, não a lista: músicas novas
  aparecem sozinhas
- **Cruzamento entre faixas (crossfade)** — uma faixa vai sumindo
  enquanto a próxima entra, inclusive na troca entre rádios
- **Equalizador, efeitos e normalizador** — graves, médios, agudos,
  eco, reverberação, compressor, coro, flanger, e um normalizador de
  volume com 5 intensidades
- **Velocidade e tom** — ajuste independente (preservando um ou
  outro), ou os dois juntos como fita/vinil
- **Plugins VST** — carregue processadores de áudio externos
- **Botões de mídia** — fones e caixas Bluetooth e as teclas de mídia
  do teclado controlam o Winple, mesmo minimizado
- **Fila** — enfileire arquivos e pastas sem interromper o que toca
  (E, Shift+E, ou "Enfileirar no Winple Player" no Explorer)
- **Modo portátil** — leve o programa e seus dados num pendrive
- **Backup completo** — exporte e importe todas as configurações num
  arquivo, para recuperar tudo rápido ao trocar de computador
- **Retoma de onde parou** — volta com a última playlist pronta pra
  tocar, e cada episódio de podcast continua do ponto exato
- **Se atualiza por dentro** — avisa quando sai uma versão nova e,
  com a sua permissão, baixa, instala e abre de novo sozinho, inclusive
  na cópia portátil
- **Diagnóstico** — confere os próprios arquivos e grava um registro
  para enviar ao suporte quando algo der errado
- **Listas de reprodução** — abre e salva `.m3u`, `.m3u8` e `.pls`
- **Capa do álbum** — extraída automaticamente do arquivo
- **Nome da música ao vivo** — nas rádios que enviam essa informação

## Acessibilidade

Este é o ponto central do projeto, não um detalhe:

- Tudo funciona pelo teclado — o mouse é opcional
- Testado com **NVDA**
- Sem elementos visuais desnecessários competindo por atenção
- O que está tocando aparece no título da janela (que o leitor de tela
  anuncia no Alt+Tab e lê no NVDA+T), sem interromper a cada troca
  automática de música
- Esc volta um nível: do episódio para a lista de episódios, da rádio
  para as favoritas, e daí para a janela principal
- Listas navegáveis em vez de caixas de mensagem
- Avisos falados só quando informam algo útil, sem falatório
- Pressione **F1** a qualquer momento para ver todos os atalhos, e
  **Shift+F1** para ver as novidades da versão

## Atalhos principais

| Tecla | Ação |
|---|---|
| **F1** | Lista completa de atalhos |
| **Shift+F1** | Novidades desta versão |
| **X** | Tocar / voltar ao início do arquivo |
| **C** ou **Espaço** | Pausar / continuar |
| **B** / **Z** | Próxima / anterior |
| **Setas** | Volume (cima/baixo), avançar/retroceder (lados) |
| **L** | Abrir arquivos |
| **Shift+L** | Abrir pasta |
| **Ctrl+Alt+L** | Abrir arquivo compactado |
| **E** / **Shift+E** | Enfileirar arquivos / pasta |
| **J** | Lista de reprodução |
| **Ctrl+M** | Biblioteca |
| **Ctrl+P** | Preferências |
| **Ctrl+D** | Pastas favoritas |
| **Ctrl+L** | Abrir rádio por URL |
| **Ctrl+F** | Rádios favoritas |
| **Ctrl+Shift+P** | Meus podcasts |
| **T** / **Shift+T** | Tempo da faixa / o que está tocando |
| **Ctrl+T** | Pular para um tempo |
| **I** / **Ctrl+I** | Informações / copiar artista e música |
| **F11** / **F2** / **F3** | Vídeo: tela cheia / áudio / legenda |
| **Esc** | Voltar um nível (episódios, podcasts, favoritas) |
| **Ctrl+E** | Equalizador, efeitos e normalizador |
| **Ponto/Vírgula** | Velocidade ou tom (escolha em Preferências) |

O **[manual completo](MANUAL.md)** tem a lista inteira e explica cada
recurso em detalhe.

---

## Instalação

1. Baixe o instalador na página de **[Releases](../../releases/latest)**.
2. Execute e siga o assistente.
3. Requisitos: **Windows 10 ou 11, 64 bits**. Nenhum outro programa ou
   codec precisa ser instalado.

### Sobre alertas de antivírus

Alguns antivírus podem acusar falso positivo. Isso é comum em programas
acessíveis feitos dessa forma — a ferramenta de empacotamento é a mesma
usada por alguns malwares, então os antivírus desconfiam de tudo que ela
gera. Além disso, o programa faz duas coisas que disparam heurísticas:
baixa dados da internet (é como rádio funciona) e integra com leitores
de tela (que por natureza leem o conteúdo de outras janelas). Se o seu
antivírus reclamar, é seguro liberar o programa na lista de exceções.

Se só os **vídeos** pararem de tocar, é provável que o antivírus tenha
removido algum arquivo da parte de vídeos. O Winple avisa qual arquivo
falta; **Ajuda → Verificar arquivos do Winple** confere tudo, e
instalar o programa de novo por cima (ou atualizar) repõe o que
faltar, sem mexer nas suas configurações.

---

## Sobre o nome

Este programa já se chamou **LS AudioPlayer** (as iniciais do autor,
Leandro Souza). A partir da versão 1.0.0 ele passou a se chamar
**Winple Player** — um nome próprio e original, que não depende mais
das iniciais de ninguém. É o mesmo programa, com um nome novo e uma
identidade pensada para crescer sozinha.

---

## Histórico de versões

Cada lançamento, com tudo que mudou, está em
**[Releases](../../releases)** e resumido no
**[histórico de versões](CHANGELOG.md)**.

---

## Créditos

Desenvolvido por **Leandro Souza**.

**Motor de áudio**: [BASS](https://www.un4seen.com), da un4seen
developments — gratuita para uso não-comercial.

**Suporte a VST**: BASS_VST, por Bjoern Petersen para Silverjuke.net.
VST PlugIn Technology by Steinberg Media Technologies GmbH. Plugins VST
não acompanham o programa — cada um tem sua própria licença.

**Arquivos MIDI**: BASSMIDI, com o soundfont GeneralUser GS, de
S. Christian Collins.

**Vídeos**: [libVLC](https://www.videolan.org), do projeto VideoLAN,
sob a licença LGPL.

**Arquivos compactados**: [7-Zip](https://www.7-zip.org), de Igor
Pavlov, sob a licença GNU LGPL; o código de descompactação de RAR segue
a restrição da licença unRAR.
