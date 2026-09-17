# Winple Player

Um player de áudio acessível para Windows, no estilo Winamp clássico.
Feito para ser usado inteiro pelo teclado, com foco em quem usa leitor
de tela.

**[⬇️ Baixar a última versão](../../releases/latest)**

---

## O que ele faz

- **Toca suas músicas** — MP3, WAV, OGG, FLAC, M4A, AAC, WMA
- **Toca rádios da internet** — Icecast, Shoutcast e HLS, sem cortes
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
- **Modo portátil** — leve o programa e seus dados num pendrive
- **Backup completo** — exporte e importe todas as configurações num
  arquivo, para recuperar tudo rápido ao trocar de computador
- **Retoma de onde parou** — volta com a última playlist pronta pra
  tocar
- **Verifica atualizações sozinho** — avisa quando sai uma versão
  nova, sem baixar nada sem sua permissão
- **Listas de reprodução** — abre e salva `.m3u`, `.m3u8` e `.pls`
- **Capa do álbum** — extraída automaticamente do arquivo
- **Nome da música ao vivo** — nas rádios que enviam essa informação

## Acessibilidade

Este é o ponto central do projeto, não um detalhe:

- Tudo funciona pelo teclado — o mouse é opcional
- Testado com **NVDA**
- Sem elementos visuais desnecessários competindo por atenção
- O que está tocando aparece no título da janela (que o leitor de tela
  anuncia no Alt+Tab)
- Listas navegáveis em vez de caixas de mensagem
- Avisos falados só quando informam algo útil, sem falatório
- Pressione **F1** a qualquer momento para ver todos os atalhos

## Atalhos principais

| Tecla | Ação |
|---|---|
| **F1** | Lista completa de atalhos |
| **X** | Tocar / voltar ao início do arquivo |
| **C** ou **Espaço** | Pausar / continuar |
| **B** / **Z** | Próxima / anterior |
| **Setas** | Volume (cima/baixo), avançar/retroceder (lados) |
| **L** | Abrir arquivos |
| **Shift+L** | Abrir pasta |
| **Ctrl+P** | Preferências |
| **Ctrl+D** | Pastas favoritas |
| **Ctrl+L** | Abrir rádio por URL |
| **Ctrl+F** | Rádios favoritas |
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
