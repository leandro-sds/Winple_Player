# Winple Player — Manual do usuário

**Versão 2.0.5**

Um player de áudio e vídeo feito para ser usado inteiro pelo teclado,
com foco em acessibilidade. Toca suas músicas, vídeos, rádios da
internet e podcasts, organiza sua coleção numa biblioteca, abre
arquivos compactados, e tem equalizador, normalizador, controle de
velocidade/tom e suporte a plugins VST.

---

## Como usar, em resumo

O Winple Player não precisa de mouse. A janela é limpa de propósito:
o que está tocando aparece no **título da janela** (que o leitor de
tela anuncia no Alt+Tab) e na barra de status, embaixo.

Ao abrir algo novo — um álbum, uma pasta, uma rádio escolhida na
lista de favoritas ou pela URL, um episódio, algo mandado pelo
DOSVOX —, o título muda na hora e é anunciado uma vez. Ao andar pelo
que já está tocando (B, Z, Numpad 1 e 3, Ctrl+Z, Ctrl+B), seja num
álbum ou nas rádios favoritas, a troca é silenciosa. Já com você na janela do programa, o
leitor de tela **não é interrompido** a cada troca automática de
música ou a cada música nova de uma rádio — mas o **NVDA+T** sempre lê o que está tocando agora, e o
Alt+Tab também. Para ouvir o que está tocando a qualquer momento,
use também **Shift+T**.

Nas músicas do computador, o título traz o número da faixa gravado no
próprio arquivo (a etiqueta de número da faixa, quando existe) e o
nome da música, sem a extensão (".mp3" e afins). Em Preferências, a
opção "Número antes do nome da música, no título" permite trocar esse
número pela posição da música na lista de reprodução (por exemplo, 37
numa lista de 120), ou não mostrar número nenhum. Nos episódios de
podcast, o número é sempre a posição do episódio na lista; nas rádios,
não há número.

Para não interromper o leitor de tela, o programa não anuncia ações
simples como pausar, continuar, parar ou voltar ao início da faixa —
a barra de status mostra o estado. Ele fala o que você precisa saber:
valores que você ajusta (volume, velocidade, tom, balanço), modos que
liga e desliga, avisos e erros.

Você pode fazer tudo de dois jeitos: pelas **teclas de atalho** (mais
rápido) ou pelos **menus** (pressione Alt para abrir). A qualquer
momento, **F1** mostra a lista completa de atalhos numa tela
navegável (Esc fecha), e **Shift+F1** mostra as novidades da versão
que você está usando.

---

## Teclas de atalho

### Controlar a reprodução

| Tecla | O que faz |
|---|---|
| **X** | Toca / volta ao início do arquivo. Em rádio, reconecta |
| **C** ou **Espaço** | Pausa ou continua. Depois de parar (V), toca de novo |
| **V** | Para |
| **Shift+V** | Para com o som sumindo aos poucos |
| **Ctrl+V** | Para quando a faixa atual terminar |
| **B** | Próxima faixa (ou próxima rádio favorita, ou próximo episódio) |
| **Z** | Faixa anterior (ou rádio favorita anterior, ou episódio anterior) |
| **Numpad 3** | Avança 10 faixas de uma vez |
| **Numpad 1** | Volta 10 faixas de uma vez |
| **Ctrl+Z** | Vai para a primeira faixa da lista (ou primeira rádio favorita) |
| **Ctrl+B** | Vai para a última faixa da lista (ou última rádio favorita) |
| **Seta para cima** | Aumenta o volume |
| **Seta para baixo** | Diminui o volume |
| **Seta para a direita** | Avança na música |
| **Seta para a esquerda** | Retrocede na música |
| **Shift+Seta para a direita** | Avança 1 minuto de uma vez |
| **Shift+Seta para a esquerda** | Retrocede 1 minuto de uma vez |
| **Ctrl+Shift+Seta para a direita** | Balanço para a direita |
| **Ctrl+Shift+Seta para a esquerda** | Balanço para a esquerda |
| **T** | Anuncia o tempo atual da faixa |
| **Shift+T** | Fala o que está tocando |
| **Ctrl+T** | Pula para um tempo específico - o campo já vem preenchido com o tempo atual da faixa |
| **Home** | Volta ao início da faixa atual |
| **End** | Vai para o fim da faixa atual |
| **I** ou **Alt+3** | Mostra as informações do que está tocando numa caixa de texto |
| **Ctrl+I** | Copia o artista e a música que estão tocando. Duas vezes rápido copia todas as informações |

Os atalhos de tempo ficam todos na letra T: **T** fala o tempo,
**Shift+T** fala o que está tocando e **Ctrl+T** pula para um tempo.

**Copiando o que está tocando (Ctrl+I):** o programa copia para a
área de transferência e fala o que copiou. Na rádio, copia só a música
do momento, sem o nome da rádio, e avisa quando a rádio não informa a
música; no podcast, o título do episódio e o nome do podcast.
Apertando **Ctrl+I** duas vezes rápido, copia todas as informações, o
mesmo texto da janela que a letra **I** abre. Tudo o que o Winple copia
continua na área de transferência mesmo depois de fechar o programa.

Quando o volume, o balanço, a velocidade ou o tom chegam no limite, o
programa avisa em voz ("Volume no máximo", "Velocidade mínima"...), em
vez de ficar em silêncio.

**Ctrl+V numa rádio:** rádio ao vivo não tem fim de faixa, então o
programa só avisa e sugere o **V** para parar.

### Velocidade e tom

| Tecla | O que faz |
|---|---|
| **Ponto** | Aumenta velocidade ou tom |
| **Vírgula** | Diminui velocidade ou tom |
| **Barra (/)** | Volta velocidade e tom ao normal |

A barra funciona tanto na tecla do teclado principal (inclusive no
teclado ABNT2) quanto na barra do teclado numérico. Também dá para
voltar ao normal pelo menu **Reprodução → Voltar ao normal**.

O que "ponto"/"vírgula" ajustam — **Tom**, **Velocidade** ou **Os
dois juntos** (estilo fita/vinil) — se escolhe em **Arquivo →
Preferências**. "Só velocidade" e "só tom" precisam do arquivo
`bass_fx.dll` presente; sem ele, o programa avisa e usa "os dois
juntos" como reserva.

### Abrir músicas e rádios

| Tecla | O que faz |
|---|---|
| **L** | Abrir um ou mais arquivos (músicas ou vídeos) |
| **Shift+L** | Abrir uma pasta inteira (incluindo subpastas) |
| **Ctrl+Alt+L** | Abrir um arquivo compactado (ZIP, RAR, 7z, TAR) |
| **Ctrl+L** | Abrir uma rádio pela URL |
| **Ctrl+Shift+L** | Abrir uma lista pronta (arquivos .m3u ou .pls) |
| **E** | Enfileirar um ou mais arquivos no fim da lista, sem interromper o que toca |
| **Shift+E** | Enfileirar uma pasta no fim da lista |
| **J** | Ver a lista de reprodução / pular para um arquivo |
| **Ctrl+M** | Abrir a biblioteca |
| **Ctrl+D** | Ver suas pastas favoritas de músicas |
| **Ctrl+Shift+D** | Cadastrar uma pasta favorita |

> Abrir uma pasta nova **substitui** a lista atual, nunca soma com o
> que já estava tocando. Para somar, use **E** ou **Shift+E**
> (enfileirar).

> **Abrindo de fora do programa** — pelo DOSVOX, pelo "Reproduzir com
> Winple Player" do Explorer ou com um duplo-clique —, o que chegou
> (arquivo, pasta ou lista .m3u) sempre **substitui** a lista atual e
> começa a tocar na hora, com o programa fechado ou já aberto.
> Já **dentro** do programa, abrir uma lista pronta (Ctrl+Shift+L)
> **soma** à lista atual, para você montar sua sessão.

Ao abrir uma rádio pela URL, pode digitar o endereço sem o "http://"
(por exemplo `radio.com.br:8000/live`) — o programa completa sozinho.

"Abrir lista de reprodução" (Ctrl+Shift+L) aceita só listas. Se você
escolher ali um arquivo de áudio, vídeo, programa ou compactado, o
Winple recusa e não mexe na lista atual. Para um arquivo compactado,
ele avisa: "Para abrir arquivo compactado, pressione Ctrl+Alt+L".

### Arquivos compactados

**Arquivo → Abrir arquivo compactado** (**Ctrl+Alt+L**) abre arquivos
ZIP, RAR, 7z e TAR (inclusive `.tar.gz`, `.tar.bz2` e `.tar.xz`) e toca
as músicas e vídeos que estão dentro, com todos os recursos de sempre:
plugins, efeitos, crossfade e posição.

- O Winple descompacta só os arquivos de áudio e vídeo, numa pasta
  própria, e abre essa pasta. Enquanto descompacta, dá para cancelar.
- Nada fica acumulado no computador: os arquivos descompactados são
  apagados quando o Winple fecha. Por isso, uma lista vinda de um
  arquivo compactado não é reaberta na próxima vez; o Winple avisa e
  basta abrir o arquivo de novo.
- Arquivos protegidos por senha ou danificados são avisados, e a lista
  atual não é mexida.

### Pastas favoritas

Cadastre as pastas que você mais ouve: **Ctrl+Shift+D** adiciona uma
pasta à lista. Depois, **Ctrl+D** abre a lista — **Enter** toca a
pasta selecionada e **Delete** remove da lista.

O programa guarda o **caminho** das pastas, não a lista de músicas —
ou seja, se você colocar músicas novas nelas depois, elas aparecem
automaticamente da próxima vez, sem precisar refazer nada.

### Modos de reprodução

| Tecla | O que faz |
|---|---|
| **R** | Liga/desliga repetir a lista |
| **S** | Liga/desliga o modo aleatório |

Esses dois modos **ficam salvos**: se você fechar o programa com o
aleatório ligado, ele continua ligado da próxima vez. Com "repetir"
desligado, a lista **para** nos extremos (início/fim) em vez de dar a
volta sozinha — vale também no modo aleatório. (As rádios favoritas
são a exceção: veja abaixo.)

O modo aleatório embaralha a lista inteira e toca **todas as músicas
antes de repetir qualquer uma** — e embaralha de novo, numa ordem
diferente, quando termina a volta. Se você escolher uma música direto
na lista (J), o aleatório continua a partir dela.

### Rádios favoritas

| Tecla | O que faz |
|---|---|
| **Ctrl+Shift+F** | Adiciona a rádio que está tocando aos favoritos |
| **Ctrl+F** | Abre a lista de rádios favoritas |

Na lista de favoritas, você pode:
- **Enter** — toca a rádio selecionada
- **Delete** — remove da lista
- **Ctrl+Seta para cima / para baixo** — muda a rádio de posição
- Botão **Renomear** — dá um nome mais fácil de achar

**Trocando de rádio como num radinho:** depois de tocar uma favorita,
as teclas passam a trocar entre as suas rádios favoritas, em vez de
navegar pela lista de músicas:

| Tecla | Nas rádios favoritas |
|---|---|
| **B** / **Z** | Próxima / rádio anterior |
| **Numpad 3** / **Numpad 1** | Avança / volta 10 rádios |
| **Ctrl+Z** | Primeira rádio favorita |
| **Ctrl+B** | Última rádio favorita |

A navegação entre favoritas é sempre **circular**, com ou sem
"repetir" ligado: passou da última, recomeça da primeira (e
vice-versa). Com uma favorita só, o programa avisa em vez de
reconectar a mesma rádio. Volta ao normal quando você abrir uma música
ou pasta.

**Pausar uma rádio:** uma pausa curta continua de onde parou. Se a
rádio ficar pausada por mais de 1 minuto, o programa libera a conexão
com o servidor; ao continuar (C, Espaço ou X), ele reconecta já no ao
vivo.

**Backup:** o menu Rádios tem **Exportar** e **Importar**, para
guardar suas rádios num arquivo ou levá-las para outro computador.

### Podcasts

| Tecla | O que faz |
|---|---|
| **Ctrl+Shift+P** | Abre "Meus podcasts" |

**Cadastrar um podcast:** em "Meus podcasts", use o botão **Adicionar
podcast** (**Alt+A**) e cole o endereço do **feed RSS** do podcast.
O programa busca o podcast na hora e anuncia o nome e quantos
episódios ele tem.

Na tela **Meus podcasts**:
- **Enter** — busca os episódios mais recentes e abre a lista deles,
  anunciando quantos episódios novos chegaram desde a última vez
- **Alt+T** — **Atualizar todos**: busca episódios novos de todos os
  podcasts de uma vez e anuncia onde chegou coisa nova (por exemplo,
  "Episódios novos em 2 podcasts: Sentido da Bola, 1; Por Dentro da
  Bíblia, 2"). Na lista, esses podcasts passam a mostrar quantos
  episódios novos têm, até você abrir cada um. Também fica no menu
  **Podcasts → Atualizar todos os podcasts**. Com muitos podcasts, a
  atualização pode levar alguns minutos: a barra de status mostra o
  andamento a cada podcast, o leitor de tela fala o andamento a cada
  10 segundos ("40 de 200"), e apertar **Alt+T** de novo no meio fala
  o andamento na hora. Dá para continuar ouvindo e usando o programa
  enquanto isso.
  Se algum podcast não puder ser atualizado, o resumo final diz o
  nome dele e o motivo (por exemplo, "o endereço do feed não existe
  mais"), e na lista o podcast fica marcado com "não atualizou" e o
  motivo, até a próxima atualização dar certo.
- **Delete** ou **Alt+R** — remove o podcast (pede confirmação)
- **Alt+O** — escolhe a ordem da lista: **Minha ordem** (padrão),
  **Nome (A a Z)**, **Nome (Z a A)**, **Atualizados recentemente
  primeiro** ou
  **Atualizados há mais tempo primeiro**. A escolha fica guardada.
- **Ctrl+Seta para cima / para baixo** — muda o podcast de posição
  (na ordem "Minha ordem")
- **Ctrl+C** ou botão **Copiar endereço do feed** (**Alt+C**) —
  copia o **endereço do feed** (para colar em outro programa de
  podcast)
- **Ctrl+Shift+C** ou botão **Copiar página do podcast** (**Alt+P**)
  — copia a **página do podcast** (para mandar a alguém). Se o podcast
  não informar uma página, copia o feed

O programa **não** procura episódios novos sozinho, em segundo plano:
ele só busca quando você abre um podcast (Enter) ou pede para
atualizar todos (Alt+T). Assim ele não fica usando a internet sem
você saber.
- **Alt+I** — importa podcasts de um arquivo OPML
- **Alt+X** — exporta seus podcasts para um arquivo OPML

Na lista de **episódios**, cada
linha traz o título, a data, a duração e a situação do episódio:
**novo**, **ouvido** ou **parou em** tantos minutos.
- **Enter** — toca o episódio e fecha as telas
- **Alt+D** — mostra a descrição do episódio
- **Alt+M** — marca como ouvido / não ouvido
- **Ctrl+D** — o leitor de tela lê a descrição do episódio ali mesmo,
  sem abrir janela (Alt+D abre a descrição numa caixa de texto)
- **Ctrl+C** ou botão **Copiar link do episódio** (**Alt+C**) —
  copia o **link do episódio** (a página dele, para mandar a alguém).
  Se o episódio não tiver página própria, copia o link do áudio
- **Ctrl+Shift+C** ou botão **Copiar link do áudio** (**Alt+L**) —
  copia o **link direto do arquivo de áudio**
- **Alt+B** — o botão muda de nome conforme o episódio selecionado:
  **Baixar**; **Cancelar download**, enquanto baixa; **Tirar da fila
  de downloads**, se estiver esperando; e **Remover download**, depois
  de baixado (apaga o arquivo, pedindo confirmação)
- **Alt+N** — **Cancelar todos os downloads**. O botão aparece só
  enquanto há downloads em andamento ou na fila

**Marcando vários episódios:**
- **Espaço** — marca e desmarca o episódio. O leitor de tela fala
  "Marcado" no começo de cada um que estiver marcado
- **Ctrl+A** — marca todos; **Ctrl+Shift+A** — desmarca todos
- Com episódios marcados, o botão **Baixar** (**Alt+B**) passa a se
  chamar, por exemplo, **Baixar 5 marcados**, e coloca todos na fila
  de uma vez. Os que já estão baixados ou na fila são pulados, e o
  programa fala um resumo
- Com episódios marcados, **Ctrl+C** e o botão **Copiar links dos
  marcados** (**Alt+C**) copiam os links de todos eles, um por linha.
  **Ctrl+Shift+C** e **Copiar links do áudio dos marcados**
  (**Alt+L**) copiam os links diretos dos arquivos de áudio

Marcar não atrapalha o Enter: ele continua tocando o episódio
selecionado.

Os episódios aparecem na mesma ordem em que a plataforma do podcast
publica — quase sempre do mais novo para o mais antigo.

**Ouvindo um episódio**, na janela principal, tudo funciona como num
arquivo comum: **B** e **Z** trocam de episódio, as **setas**, o
**Ctrl+T**, **Home** e **End** avançam e retrocedem, **T** anuncia o
tempo, e velocidade, tom e efeitos funcionam normalmente.

**O programa lembra onde cada episódio parou.** Ao voltar num
episódio, ele avisa ("Continuando de 23 minutos") e segue dali. Ao
chegar perto do fim, o episódio é marcado como ouvido.

**Tocando em sequência:** quando um episódio termina, o programa
segue sozinho para o próximo da lista — normalmente o episódio
anterior a ele, já que a lista vem do mais novo para o mais antigo.
No último da lista, ele avisa "Fim da lista de episódios". Entre um episódio e outro há uma pausa curtinha,
enquanto o próximo conecta. Se preferir que o programa pare ao fim de
cada episódio, desligue a opção nas Preferências.

**Baixando episódios:** o download acontece em segundo plano, um
episódio de cada vez — dá para pedir vários, e eles entram numa fila.
Na lista, cada episódio mostra se está **baixado**, **baixando** ou
**na fila para baixar**, e o programa avisa quando cada download
termina. Quando um download falha por instabilidade do servidor, o
programa tenta de novo sozinho, até 3 vezes, e avisa a cada tentativa;
um download cortado no meio também é percebido e baixado de novo. Os
arquivos ficam na pasta Música, em:

```
Música\Winple Player\Podcasts\Nome do podcast\
    2025-05-20 - Programa 01.mp3
    2025-12-09 - Programa 29.mp3
```

A data na frente deixa os arquivos em ordem, do mais antigo para o
mais novo. Um episódio baixado toca direto do computador: começa na
hora, funciona sem internet e avançar ou retroceder é instantâneo. Se
você apagar ou mover o arquivo por fora, o programa volta a tocar o
episódio pela internet.

Os episódios não baixados tocam direto da internet. Se o servidor
responder mal, o programa tenta de novo sozinho, até 3 vezes. Se você pular para um ponto que ainda não chegou, o programa avisa
que aquele trecho ainda não foi baixado — é só tentar de novo daqui a
pouco. Se a conexão cair no meio, ele avisa e guarda onde estava:
**X** ou **Espaço** continuam dali.

**Sem internet**, "Meus podcasts" mostra a última lista de episódios
guardada.

**Trazendo seus podcasts de outro programa:** quase todo aplicativo de
podcast (AntennaPod, Podcast Addict, Pocket Casts e outros) exporta a
lista de inscrições num arquivo **OPML**, geralmente numa opção
chamada "Exportar OPML" ou "Exportar inscrições". No Winple, use
**Podcasts → Importar podcasts (OPML)** (ou **Alt+I** em "Meus
podcasts"). O programa soma os podcasts do arquivo aos que você já
tem, sem duplicar, e avisa quantos entraram. Os episódios de cada um
são buscados só quando você abrir aquele podcast — assim o programa
não sai abrindo dezenas de conexões de uma vez.

O caminho inverso também funciona: **Podcasts → Exportar podcasts
(OPML)** gera um arquivo com todos os seus podcasts, para levar para
outro programa ou para o celular.

O Spotify não permite exportar a lista de podcasts; quem ouve só por
lá precisa cadastrar os podcasts pelo endereço RSS.

### Lista de reprodução

| Tecla | O que faz |
|---|---|
| **J** | Abre a lista do que está tocando |
| **Ctrl+B** | Vai para a última faixa |
| **Ctrl+Del** | Remove a faixa atual da lista |

Na lista (J):
- **Enter** — toca o item selecionado
- **Alt+B** — vai para o campo de busca: digitar parte do nome vai
  filtrando a lista (sem diferença entre maiúsculas, minúsculas e
  acentos)
- **Shift+Enter** — põe a música na **fila a seguir**: ela toca logo
  depois da atual. Várias músicas postas assim tocam na ordem em que
  foram pedidas
- **Delete** — remove da lista
- A primeira letra continua pulando entre as músicas

O menu **Lista** também tem **Limpar lista** e **Salvar lista como
M3U**.

### Biblioteca

| Tecla | O que faz |
|---|---|
| **Ctrl+M** | Abre a biblioteca |

A biblioteca organiza suas músicas por **artista**, **álbum**,
**gênero** e **ano**, a partir das etiquetas gravadas nos arquivos. Na
primeira vez, o programa oferece a pasta Música e as suas pastas
favoritas; as pastas se escolhem depois em **Biblioteca → Pastas da
biblioteca**. A primeira leitura roda em segundo plano e fala o
andamento a cada 10 segundos; nas vezes seguintes, o programa só lê o
que mudou. Para ler de novo na hora, use **Biblioteca → Atualizar
biblioteca**. Ao abrir o programa, nada da biblioteca é carregado.

Dentro da biblioteca:
- **Enter** — entra no artista ou álbum; numa música, toca a partir
  dela
- **Backspace** ou **Esc** — volta um nível; Esc no primeiro nível
  fecha a biblioteca
- **Ctrl+Enter** — toca tudo do artista, álbum, gênero ou ano
- **Shift+Enter** — põe na fila a seguir
- **Alt+E** — enfileira no fim da lista
- **Alt+I** — informações da música
- **Alt+B** — busca em tudo
- **Alt+V** — "Ver por": Artistas, Álbuns, Gêneros, Anos, Todas as
  músicas ou Adicionadas recentemente
- A primeira letra pula para os itens da lista, como no J

Tocando algo pela biblioteca, **Esc** na janela principal reabre a
biblioteca onde você estava, sem parar a música.

Um álbum separado em subpastas, como CD1 e CD2, aparece como dois
álbuns. Os vídeos ficam fora da biblioteca, que é só de músicas.
Remover uma pasta da biblioteca não apaga nenhum arquivo do computador.

### Vídeos

O Winple toca vídeos (MP4, MKV, AVI, MOV, WMV, WebM e outros) do mesmo
jeito que as músicas: abra pelo **L**, pela pasta, pelo Explorer ou por
um arquivo compactado. A imagem aparece na janela do programa, e o som
passa pelo volume, balanço, equalizador, normalizador e plugins VST,
como o das músicas. O programa acerta a sincronia entre a voz e a
imagem sozinho, sem nenhum ajuste.

| Tecla | O que faz |
|---|---|
| **F11** | Tela cheia (Esc ou F11 de novo sai) |
| **F2** | Troca a faixa de áudio (por exemplo, português / inglês) |
| **F3** | Troca a legenda (ou desliga) |
| **Alt+V** | Menu Vídeo: escolhe o áudio e a legenda pela lista |

Com a opção **Preferir áudio em português nos vídeos** ligada (no menu
Vídeo ou nas Preferências), um vídeo dublado já começa no áudio em
português.

### Arquivos MIDI

Arquivos MIDI (`.mid`, `.midi`, `.rmi`, `.kar`) tocam com um soundfont,
o conjunto de sons dos instrumentos. O programa já vem com o
**GeneralUser GS**. Para usar outro, vá em **Preferências → Escolher
soundfonts para arquivos MIDI**: ali dá para adicionar os seus
(`.sf2`, `.sf3` ou `.sfz`), escolher qual usar e abrir a pasta de
soundfonts.

### Botões de mídia

O Winple responde aos botões de fones de ouvido e caixas de som
Bluetooth (tocar e pausar, próxima e anterior, conforme os botões que o
aparelho tiver) e às teclas de mídia do teclado (tocar/pausar,
próxima, anterior e parar), mesmo com ele minimizado.

No Windows 10 e 11, o Winple aparece no painel de mídia do Windows (ao
lado do controle de volume), mostrando o que está tocando. Na rádio,
aparece a música do momento, quando a rádio informa.

- Os botões de volume do fone continuam controlando o volume do Windows
  ou do próprio fone, como em qualquer programa.
- Como em qualquer player, os botões ficam com o último programa que
  tocou alguma coisa: se você estava num vídeo do navegador e depois
  deu play no Winple, os botões passam a ser do Winple.
- O recurso pode ser desligado nas Preferências, na opção "Responder
  aos botões de mídia".

### Equalizador, efeitos e normalizador

| Tecla | O que faz |
|---|---|
| **Ctrl+E** | Abre o equalizador, os efeitos e o normalizador |

**Importante:** tudo nessa tela — equalizador, efeitos, normalizador
e VST — vale **por padrão só para músicas/arquivos locais** (e
episódios de podcast). Rádios não passam por aqui, porque cada uma já
vem processada do lado de quem transmite; empilhar processamento nosso
por cima soa estranho em algumas delas. Mas isso é configurável: a
opção "Usar os mesmos efeitos nas rádios", na mesma tela do Ctrl+E,
liga esse processamento pras rádios também, pra quem preferir.

Ajuste **graves**, **médios** e **agudos** de -15 a +15 (0 é o som
original), usando as setas do teclado ou digitando o número.

Também há efeitos que você pode ligar e desligar: **eco**,
**reverberação**, **compressor**, **coro** e **flanger**.

**Normalizador de volume:** equilibra faixas altas e baixas (ajuda a
ouvir conversas/trechos baixos sem estourar os altos). Tem 5
intensidades: Muito leve, Leve, Médio, Forte e Muito forte.

Tudo fica salvo automaticamente.

**Plugins VST:** a mesma tela permite carregar um plugin VST 2.x
(efeitos profissionais de terceiros). Coloque seus plugins (arquivos
`.dll`) na pasta **plugins**, ao lado do programa — o botão
correspondente na tela leva direto lá. Por padrão valem só para
arquivos locais, mas isso também é configurável (mesma opção acima).
Cada plugin tem sua própria licença; o Winple Player sabe
hospedá-los, mas não vem com nenhum incluído.

Na lista de plugins, **Espaço** ou **Enter** liga e desliga o plugin
selecionado — só ele entra ou sai, os outros continuam como estão. Os
plugins processam o som **depois** do equalizador, dos efeitos e do
normalizador, na ordem da lista. O Winple Player usa plugins **VST 2 de
64 bits**; se um plugin não puder ser ativado (por exemplo, por ser de
32 bits, ser VST3 ou depender de algum arquivo que não está instalado),
o programa avisa o motivo — inclusive quando o plugin falha ao abrir
uma música. O plugin precisa ter os mesmos bits do Winple Player: o
Winple de 64 bits usa plugins de 64 bits. Se você atualizar um plugin para uma versão
com outros parâmetros, os ajustes antigos dele são descartados, para
não irem parar no parâmetro errado.

### Outros

| Tecla | O que faz |
|---|---|
| **F1** | Mostra a lista de atalhos de teclado |
| **Shift+F1** | Mostra as novidades desta versão (também em Ajuda → O que há de novo nesta versão) |
| **Ctrl+P** | Abre as Preferências |
| **Alt** | Abre os menus |
| **Alt+F4** | Fecha o programa (na hora, mesmo com rádio tocando) |
| **Esc** | Volta um nível (veja abaixo). Fora disso, fecha o programa, se a opção estiver ativa nas Preferências |

**Esc volta um nível, como num menu:**

- Ouvindo um **episódio de podcast**: Esc para o episódio (guardando
  onde parou) e volta para a **lista de episódios** daquele podcast,
  já no episódio que estava tocando. Esc de novo volta para **Meus
  podcasts**, e mais um Esc volta para a janela principal.
- Ouvindo uma **rádio favorita**: Esc para a rádio e volta para a
  **lista de rádios favoritas**, já na rádio que estava tocando. Esc de
  novo volta para a janela principal.
- Tocando algo pela **biblioteca**: Esc reabre a biblioteca onde você
  estava, sem parar a música.
- Vendo um **vídeo em tela cheia**: Esc sai da tela cheia.

Voltando à janela principal por esse caminho, sem escolher nada nas
listas, o que estava tocando é fechado e a janela fica limpa (o ponto
onde o episódio parou fica guardado). Daí em diante, o Esc segue a
opção "Esc fecha o programa".

A placa de som usada pelo programa se escolhe em **Reprodução → Placa
de som** (vale a partir da próxima vez que abrir o programa).

---

## Retomando de onde parou

Ao fechar o programa com algo tocando, ele guarda a lista inteira e
qual faixa estava na vez. Na próxima abertura, o nome já aparece no
título — é só apertar **X** ou **Espaço** para continuar direto dali,
sem precisar reabrir a pasta ou a rádio manualmente. Se era um
episódio de podcast, ele continua também do ponto exato onde parou.

---

## Modo portátil

Em **Arquivo → Preferências**, dá para fazer o programa guardar
favoritos e configurações na própria pasta dele, em vez do perfil do
Windows — útil para levar num pendrive. A troca só vale a partir da
próxima vez que abrir o programa.

---

## Backup completo

Em **Ajuda → Exportar todas as configurações**, você salva num único
arquivo tudo o que o programa guarda: preferências, pastas favoritas,
rádios favoritas e seus podcasts (com o ponto onde cada episódio
parou). Útil antes de desinstalar o programa ou trocar de computador —
exporte antes, e depois é só usar **Ajuda → Importar todas as
configurações** para recuperar tudo de uma vez, sem reconfigurar do
zero. Os episódios de cada podcast são buscados de novo na primeira
vez que você abrir o podcast.

Importar **substitui** o que estiver configurado no momento (não
junta com o que já existe, diferente do importar de rádios, que
pergunta se você quer juntar) — o programa confirma antes de
prosseguir. Feche e abra o Winple Player de novo depois de importar,
para tudo entrar em vigor.

---

## Atualizações

O programa confere sozinho, discretamente, se existe uma versão mais
nova no GitHub logo depois de abrir — sem interromper nada se não
houver novidade ou se não conseguir verificar. Dá para conferir a
qualquer momento em **Ajuda → Verificar atualizações**, e desligar a
verificação automática nas Preferências.

Encontrando uma versão nova, ele pergunta antes de fazer qualquer
coisa. Respondendo **"Sim, baixar e instalar"**:

1. O programa baixa a atualização, falando o andamento, e confere se o
   arquivo chegou inteiro. O download pode ser cancelado a qualquer
   momento.
2. Ele pergunta se pode fechar para instalar.
3. O Windows pede a permissão de costume. Depois disso, a instalação
   acontece sem perguntas e o Winple abre de novo sozinho, já
   atualizado, com todas as suas configurações. Respondendo "Não" na
   permissão do Windows, o Winple continua aberto na versão atual.

Se o download falhar por algum motivo, o programa oferece abrir o
navegador, como antigamente.

O **Winple portátil** também se atualiza por dentro, na mesma pasta
onde está, mantendo as configurações e sem a pergunta de permissão do
Windows (ela só aparece se a pasta for protegida, como Arquivos de
Programas).

Depois de cada atualização, as novidades da versão aparecem sozinhas,
uma vez, quando o Winple abre. Para vê-las de novo, use **Shift+F1**.

---

## Diagnóstico e suporte

Quando algo não funciona, o Winple tem duas ferramentas para ajudar o
suporte a descobrir o motivo:

- **Ajuda → Verificar arquivos do Winple** — confere se os arquivos de
  áudio e vídeo do programa estão todos no lugar e, se houver problema,
  copia um pequeno relatório para colar num e-mail ao suporte.
- **Gravar registro de diagnóstico** (nas Preferências, desligado por
  padrão) — ligado, o Winple registra o que acontece e qualquer erro
  inesperado, no arquivo `registro_winple.txt`. Ele se abre por
  **Ajuda → Abrir pasta do registro de diagnóstico**. Para usar: ligue
  a opção, repita o que deu problema e mande o arquivo ao suporte.

Quando um vídeo não toca porque falta um arquivo da parte de vídeos
(em geral, removido pelo antivírus), o Winple diz exatamente qual
arquivo falta e como resolver. Cada atualização instala de novo, por
inteiro, a parte de vídeos; por isso, atualizar ou reinstalar o
programa por cima já repara esses arquivos.

Se o arquivo de configurações estiver danificado e grande demais, o
Winple o deixa de lado sozinho (como `config_danificado.json`), volta
às configurações padrão e avisa. Rádios, podcasts e biblioteca não são
afetados.

---

## Preferências

No menu **Arquivo → Preferências** (ou **Ctrl+P**), você pode ajustar:

- **Passo de volume** — de quanto em quanto o volume muda a cada
  toque nas setas.
- **Passo de avanço/retrocesso** — quantos segundos as setas
  laterais pulam.
- **Atraso antes de tocar streams** — normalmente 0 (imediato). Se
  alguma rádio específica engasgar ao iniciar, aumentar isso pode
  ajudar.
- **Permitir mais de uma instância** — por padrão, só uma janela do
  programa abre por vez; tentar abrir de novo só traz a janela já
  aberta pra frente.
- **Gravar registro de diagnóstico** — desligado por padrão. Ligado,
  o programa registra o que acontece e qualquer erro inesperado, para
  enviar ao suporte (veja "Diagnóstico e suporte"). Substitui as duas
  opções de log que existiam antes.
- **Abrir a última playlist ao iniciar** — ligado por padrão; se
  desmarcar, o programa abre limpo, sem carregar a sessão anterior.
- **Ao abrir um único arquivo, carregar também as outras faixas da
  mesma pasta** — desligado por padrão; se ligar, clicar num arquivo
  no Explorer carrega a pasta inteira, começando por ele.
- **Falar porcentagem ao aumentar ou diminuir o volume** — ligado por
  padrão. Anuncia o volume a cada 5% enquanto você mexe nas setas.
  Desligando, a barra de status continua mostrando o número, só para
  de falar — exceto o aviso de risco de distorção acima de 100%, que
  sempre é falado, independente desta opção.
- **Responder aos botões de mídia** — ligado por padrão. Fones e
  caixas Bluetooth e as teclas de mídia do teclado controlam o Winple
  (veja "Botões de mídia").
- **Verificar atualizações ao abrir o programa** — ligado por padrão.
- **Modo portátil** — guarda favoritos e configurações na própria
  pasta do programa, em vez do perfil do Windows, pra levar num
  pendrive. Precisa fechar e abrir o programa de novo pra valer.
- **Cruzamento entre faixas (crossfade)** — de 1 a 10 segundos, ou
  desligado. Uma faixa vai sumindo enquanto a próxima entra, sem
  aquele silêncio entre elas. Funciona ao avançar/retroceder
  manualmente (B, Z, Numpad 1/3, Ctrl+Z, Ctrl+B), na troca natural no
  fim da faixa, e também na troca entre rádios favoritas. Episódios de
  podcast não usam cruzamento.
- **Número antes do nome da música, no título** — o número da faixa
  gravado no arquivo (padrão), a posição da música na lista de
  reprodução ou nenhum número.
- **Entrada suave no começo de cada música e episódio** — ligada por
  padrão: cada faixa começa baixinho e sobe até o seu volume em 1,5
  segundo. Desligada, a faixa começa direto no volume
  escolhido. Não muda os outros fades (setas, Shift+V, cruzamento).
- **Esc também fecha o programa** — desligado por padrão.
- **Permitir aumentar o volume acima de 100%** — desligado por
  padrão; acima de 100% o som pode distorcer, dependendo da faixa.
- **O que "ponto"/"vírgula" alteram** — Tom, Velocidade ou Os dois.
- **Tentar reconectar rádio antes de avançar** — se uma rádio cair, o
  programa tenta reconectar até 3 vezes, esperando cada vez mais entre
  as tentativas, antes de desistir ou passar para a próxima favorita.
- **Ao terminar um episódio, tocar o próximo da lista** — ligado por
  padrão. Desligado, o programa para ao fim de cada episódio.
- **Episódios guardados por podcast** — quantos episódios mais
  recentes de cada podcast o programa mostra e guarda: **Todos**
  (padrão), 50, 100, 150, 300, 500 ou 1000. Ao mudar, a nova escolha
  vale da próxima vez que você abrir cada podcast.
- **Preferir áudio em português nos vídeos** — ligado por padrão. Um
  vídeo dublado já começa no áudio em português (a mesma opção do menu
  Vídeo).
- **Escolher soundfonts para arquivos MIDI** — escolhe o conjunto de
  sons usado nos arquivos MIDI (veja "Arquivos MIDI").

---

## Integração com o Windows

O registro de "Reproduzir com Winple Player" e "Enfileirar no Winple
Player" no menu de contexto do Windows (para arquivos de áudio, vídeo
e pastas), e o registro como aplicativo padrão, são feitos pelo
**instalador** (duas opções na hora de instalar) — não é preciso (nem
possível) fazer isso de dentro do programa. A cópia portátil não
registra nada no Windows.

**"Enfileirar no Winple Player"** soma os arquivos ou a pasta ao fim da
lista atual, sem interromper o que está tocando — o mesmo que o **E**
e o **Shift+E** dentro do programa.

**Abrir vários arquivos pelo Explorer:** selecione as músicas e aperte
Enter (ou use "Reproduzir com Winple Player"). Todas entram numa lista
só, em ordem alfabética, e o Winple começa a tocar a primeira. O
Windows permite isso com até **100 arquivos** de uma vez; acima disso,
ele passa a abrir o player do próprio Windows. Para abrir mais de 100
músicas, use a **pasta**: com o foco na pasta, "Reproduzir pasta com
Winple Player" no menu de contexto, ou Shift+L dentro do programa, ou
as pastas favoritas — pela pasta não há limite.

---

## Formatos suportados

**Áudio:** MP3, WAV, OGG, FLAC, M4A, AAC, WMA, Opus, APE (Monkey's
Audio), MPC (Musepack), WV (WavPack), TTA, OFR/OFS (OptimFROG)
**MIDI:** MID, MIDI, RMI, KAR
**Vídeo:** MP4, MKV, AVI, MOV, WMV, WebM, FLV, M4V, MPG, MPEG, TS,
M2TS, 3GP, OGV, VOB
**Compactados:** ZIP, RAR, 7z, TAR, TAR.GZ (TGZ), TAR.BZ2, TAR.XZ
**Listas:** M3U, M3U8, PLS
**Rádios:** streams por HTTP e HTTPS (Icecast e Shoutcast, inclusive
servidores Shoutcast antigos). Rádios em HLS (`.m3u8` como fonte ao
vivo) tocam pela BASS quando o arquivo `basshls.dll` está presente;
sem ele, tocam pelo motor do Windows — funcionam, mas sem
equalizador/efeitos/normalizador.
**Podcasts:** feeds RSS com episódios em áudio (MP3, M4A, AAC, OGG,
Opus e outros).

---

## Onde ficam seus dados

Suas rádios favoritas, podcasts e configurações ficam em:

```
%APPDATA%\Winple Player\
├── radios_WinplePlayer.json             (suas rádios favoritas)
├── podcasts_WinplePlayer.json           (seus podcasts e episódios)
├── podcasts_estado_WinplePlayer.json    (onde cada episódio parou e quais foram ouvidos)
├── biblioteca_WinplePlayer.db           (a biblioteca de músicas)
└── config.json                          (suas preferências)
```

(Ou na própria pasta do programa, se o **modo portátil** estiver
ativado.)

Você chega lá rápido pelo menu **Ajuda → Abrir pasta de dados**.

O registro de diagnóstico, quando ligado, fica à parte, em
`%LOCALAPPDATA%\Winple Player\registro_winple.txt` — o menu **Ajuda →
Abrir pasta do registro de diagnóstico** leva até ele.

Os episódios de podcast **baixados** ficam em outro lugar, na sua
pasta Música: `Música\Winple Player\Podcasts\`.

Esses arquivos **não são apagados** quando você atualiza o programa.

---

## Perguntas comuns

**A rádio demora um pouquinho para começar. É normal?**
Sim. O programa carrega um pedaço do áudio antes de começar a tocar,
para não cortar depois. É uma troca proposital: um instante a mais no
início, em troca de uma reprodução estável. Ao passar rápido pelas
favoritas com B/Z, o programa também espera um instante antes de
conectar, para conectar só a rádio onde você parou.

**Uma música da minha pasta não tocou. O que houve?**
O programa avisa o motivo na barra de status e pula para a próxima
automaticamente, sem travar o resto da pasta. Costuma ser arquivo
corrompido ou incompleto.

**A tecla Espaço muda a velocidade ou o tom?**
Não — Espaço (e C) só pausam e continuam a reprodução. Velocidade e
tom se ajustam com ponto/vírgula, e voltam ao normal com a barra (/)
ou pelo menu Reprodução → Voltar ao normal.

**Onde encontro o endereço RSS de um podcast?**
Costuma aparecer no site do podcast como "RSS" ou "Feed". Podcasts
hospedados no Spotify for Creators (o antigo Anchor) têm um endereço
no formato `https://anchor.fm/s/..../podcast/rss`.

**O programa pode fazer um servidor de rádio me bloquear?**
O Winple Player foi feito para evitar isso: ele espera cada vez mais
entre as tentativas de reconexão, desiste depois de poucas, não abre
conexões duplicadas com a mesma rádio e nunca abre mais de 20
conexões em 10 minutos com o mesmo servidor. Se esse limite for
atingido, o programa avisa e espera alguns minutos antes de tentar de
novo. Para investigar um bloqueio, ligue o registro de diagnóstico nas
Preferências.

**Um vídeo não toca, mas as músicas tocam. O que fazer?**
Quase sempre é o antivírus, que removeu ou bloqueou algum arquivo da
parte de vídeos. O Winple avisa qual arquivo falta. Use **Ajuda →
Verificar arquivos do Winple** para conferir, libere a pasta do Winple
no antivírus e instale o programa de novo por cima (ou atualize): a
instalação repõe a parte de vídeos inteira, sem mexer nas suas
configurações.

**Abri um arquivo compactado e a lista não voltou na próxima vez.**
É de propósito: os arquivos descompactados são apagados quando o
Winple fecha, para não acumular no computador. É só abrir o arquivo
compactado de novo (Ctrl+Alt+L).

**Como o programa se identifica para rádios e podcasts?**
Como "WinplePlayer", seguido da versão. Nos podcasts, isso ajuda os
criadores a saber de qual programa vieram os ouvintes.

**Posso usar em qualquer computador?**
O Winple Player funciona no Windows 10 e 11, em versões de 64 bits.

---

## Créditos

Desenvolvido por Leandro Souza.

Motor de áudio: **BASS**, de un4seen developments
(www.un4seen.com) — gratuita para uso não-comercial.

Suporte a velocidade/tom preservados: **BASS_FX**. Arquivos MIDI:
**BASSMIDI**, com o soundfont **GeneralUser GS**, de S. Christian
Collins. Suporte a plugins VST: **BASS_VST**, por Bjoern Petersen para
Silverjuke.net (LGPL).

Vídeos: **libVLC**, do projeto VideoLAN (www.videolan.org), sob a
licença LGPL.

Arquivos compactados: **7-Zip**, de Igor Pavlov (www.7-zip.org), sob a
licença GNU LGPL; o código de descompactação de RAR segue a restrição
da licença unRAR.

Este programa é distribuído gratuitamente.
