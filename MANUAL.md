# Winple Player — Manual do usuário

**Versão 1.1.0**

Um player de áudio feito para ser usado inteiro pelo teclado, com foco
em acessibilidade. Toca suas músicas, rádios da internet e podcasts,
com equalizador, normalizador, controle de velocidade/tom e suporte a
plugins VST.

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

Para não interromper o leitor de tela, o programa não anuncia ações
simples como pausar, continuar, parar ou voltar ao início da faixa —
a barra de status mostra o estado. Ele fala o que você precisa saber:
valores que você ajusta (volume, velocidade, tom, balanço), modos que
liga e desliga, avisos e erros.

Você pode fazer tudo de dois jeitos: pelas **teclas de atalho** (mais
rápido) ou pelos **menus** (pressione Alt para abrir). A qualquer
momento, **F1** mostra a lista completa de atalhos numa tela
navegável (Esc fecha).

---

## Teclas de atalho

### Controlar a reprodução

| Tecla | O que faz |
|---|---|
| **X** | Toca / volta ao início do arquivo. Em rádio, reconecta |
| **C** ou **Espaço** | Pausa ou continua |
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
| **Home** | Volta ao início da faixa atual |
| **End** | Vai para o fim da faixa atual |
| **Ctrl+J** | Pula para um tempo específico - o campo já vem preenchido com o tempo atual da faixa |

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
| **L** | Abrir um ou mais arquivos |
| **Shift+L** | Abrir uma pasta inteira (incluindo subpastas) |
| **Ctrl+L** | Abrir uma rádio pela URL |
| **Ctrl+Shift+L** | Abrir uma lista pronta (arquivos .m3u ou .pls) |
| **J** | Ver a lista de reprodução / pular para um arquivo |
| **Ctrl+D** | Ver suas pastas favoritas de músicas |
| **Ctrl+Shift+D** | Cadastrar uma pasta favorita |

> Abrir uma pasta nova **substitui** a lista atual, nunca soma com o
> que já estava tocando.

> **Abrindo de fora do programa** — pelo DOSVOX, pelo "Reproduzir com
> Winple Player" do Explorer ou com um duplo-clique —, o que chegou
> (arquivo, pasta ou lista .m3u) sempre **substitui** a lista atual e
> começa a tocar na hora, com o programa fechado ou já aberto.
> Já **dentro** do programa, abrir uma lista pronta (Ctrl+Shift+L)
> **soma** à lista atual, para você montar sua sessão.

Ao abrir uma rádio pela URL, pode digitar o endereço sem o "http://"
(por exemplo `radio.com.br:8000/live`) — o programa completa sozinho.

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
- **Ctrl+C** ou botão **Copiar link do episódio** (**Alt+C**) —
  copia o **link do episódio** (a página dele, para mandar a alguém).
  Se o episódio não tiver página própria, copia o link do áudio
- **Ctrl+Shift+C** ou botão **Copiar link do áudio** (**Alt+L**) —
  copia o **link direto do arquivo de áudio**
- **Alt+B** — o botão muda de nome conforme o episódio selecionado:
  **Baixar**; **Cancelar download**, enquanto baixa; **Tirar da fila
  de downloads**, se estiver esperando; e **Remover download**, depois
  de baixado (apaga o arquivo, pedindo confirmação)

Os episódios aparecem na mesma ordem em que a plataforma do podcast
publica — quase sempre do mais novo para o mais antigo.

**Ouvindo um episódio**, na janela principal, tudo funciona como num
arquivo comum: **B** e **Z** trocam de episódio, as **setas**, o
**Ctrl+J**, **Home** e **End** avançam e retrocedem, **T** anuncia o
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
termina. Os arquivos ficam na pasta Música, em:

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

Os episódios não baixados tocam direto da internet.
Se você pular para um ponto que ainda não chegou, o programa avisa
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

Na lista, **Enter** toca o item selecionado.

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

### Outros

| Tecla | O que faz |
|---|---|
| **F1** | Mostra a lista de atalhos de teclado |
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

## Verificar atualizações

O programa confere sozinho, discretamente, se existe uma versão mais
nova no GitHub logo depois de abrir — sem interromper nada se não
houver novidade ou se não conseguir verificar. Encontrando algo novo,
pergunta se você quer abrir o navegador para baixar (nunca baixa nem
instala sozinho). Dá para conferir manualmente a qualquer momento em
**Ajuda → Verificar atualizações**.

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
- **Registrar argumentos em log** — só para diagnóstico (grava o que
  outro programa, como o DOSVOX, mandou abrir).
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
- **Modo portátil** — guarda favoritos e configurações na própria
  pasta do programa, em vez do perfil do Windows, pra levar num
  pendrive. Precisa fechar e abrir o programa de novo pra valer.
- **Cruzamento entre faixas (crossfade)** — de 1 a 10 segundos, ou
  desligado. Uma faixa vai sumindo enquanto a próxima entra, sem
  aquele silêncio entre elas. Funciona ao avançar/retroceder
  manualmente (B, Z, Numpad 1/3, Ctrl+Z, Ctrl+B), na troca natural no
  fim da faixa, e também na troca entre rádios favoritas. Episódios de
  podcast não usam cruzamento.
- **Esc também fecha o programa** — desligado por padrão.
- **Permitir aumentar o volume acima de 100%** — desligado por
  padrão; acima de 100% o som pode distorcer, dependendo da faixa.
- **O que "ponto"/"vírgula" alteram** — Tom, Velocidade ou Os dois.
- **Tentar reconectar rádio antes de avançar** — se uma rádio cair, o
  programa tenta reconectar até 3 vezes, esperando cada vez mais entre
  as tentativas, antes de desistir ou passar para a próxima favorita.
- **Registrar conexões com as rádios em log** — desligado por padrão.
  Grava cada conexão do programa com rádios e podcasts no arquivo
  `conexoes.log`, na pasta de dados. Útil para investigar problemas de
  conexão ou bloqueio.
- **Ao terminar um episódio, tocar o próximo da lista** — ligado por
  padrão. Desligado, o programa para ao fim de cada episódio.
- **Episódios guardados por podcast** — quantos episódios mais
  recentes de cada podcast o programa mostra e guarda: **Todos**
  (padrão), 50, 100, 150, 300, 500 ou 1000. Ao mudar, a nova escolha
  vale da próxima vez que você abrir cada podcast.

---

## Integração com o Windows

O registro de "Reproduzir com Winple Player" no menu de contexto do
Windows, e o registro como aplicativo padrão, são feitos pelo
**instalador** (duas opções na hora de instalar) — não é preciso (nem
possível) fazer isso de dentro do programa.

---

## Formatos suportados

**Áudio:** MP3, WAV, OGG, FLAC, M4A, AAC, WMA
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
├── config.json                          (suas preferências)
└── conexoes.log                         (só se o log de conexões estiver ligado)
```

(Ou na própria pasta do programa, se o **modo portátil** estiver
ativado.)

Você chega lá rápido pelo menu **Ajuda → Abrir pasta de dados**.

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
novo. Para investigar um bloqueio, ligue o log de conexões nas
Preferências.

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

Suporte a velocidade/tom preservados: **BASS_FX**. Suporte a plugins
VST: **BASS_VST**, por Bjoern Petersen para Silverjuke.net (LGPL).

Este programa é distribuído gratuitamente.
