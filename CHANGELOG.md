# Histórico de versões

> **Sobre o nome:** este programa já se chamou *LS AudioPlayer*. A
> partir da versão 1.0.0 passou a se chamar **Winple Player** — um
> nome próprio, que não depende mais das iniciais do autor. É o mesmo
> programa, recomeçando a numeração de versões do zero sob o novo nome.

## 1.1.0

### Podcasts (novo)

- **Meus podcasts** (Ctrl+Shift+P): cadastre podcasts pelo endereço do
  feed RSS e ouça os episódios direto da internet
- Enter num podcast busca os episódios mais recentes e avisa quantos
  são novos; a lista de episódios segue a ordem da plataforma
- O programa **lembra onde cada episódio parou** e continua dali -
  inclusive tocando pela internet, esperando o trecho chegar
- Ao terminar um episódio, segue para o próximo da lista (configurável)
- **Baixar episódios** (Alt+B) para a pasta Música\Winple Player\Podcasts,
  um de cada vez, em segundo plano; episódio baixado toca do
  computador, sem internet, com avanço e retrocesso instantâneos
- **Atualizar todos** (Alt+T): busca episódios novos de todos os
  podcasts, com andamento falado para listas grandes; podcasts que
  falharem aparecem com o nome e o motivo
- **Importar e exportar** a lista de podcasts em OPML, o formato padrão
  dos aplicativos de podcast
- **Copiar links**: endereço do feed, página do podcast, página do
  episódio e link do áudio (Ctrl+C, Ctrl+Shift+C ou botões)
- Ordem de Meus podcasts: minha ordem, nome (A a Z / Z a A), atualizados
  recentemente ou há mais tempo
- Quantidade de episódios guardados por podcast configurável (padrão:
  todos); marcar como ouvido / não ouvido; descrição do episódio

### Navegação

- **Esc volta um nível**: ouvindo um episódio, volta para a lista de
  episódios; ouvindo uma rádio favorita, volta para a lista de
  favoritas; mais um Esc volta para a janela principal, que fica limpa
- **Shift+T** fala o que está tocando

### Leitor de tela

- O NVDA não é mais interrompido a cada troca automática de música ou
  a cada música nova de uma rádio - e o NVDA+T continua lendo sempre o
  que está tocando agora
- Andar pelo que já está tocando (B, Z, Numpad, Ctrl+Z/B) é silencioso,
  igual em CD, rádios e podcasts; abrir algo novo anuncia o título na
  hora, uma vez
- Falas enxutas: sem "Pausado", "Reproduzindo", "Parado" e afins - só
  valores ajustados, modos, avisos e erros
- Sem mais "painel", "panel" e "gráfico" ao entrar na janela
- Dicas de atalho removidas das telas (estão no F1 e no manual)
- Ordem do Tab corrigida nas telas de podcasts

### Rádio

- O programa se apresenta aos servidores com o próprio nome
  (WinplePlayer), em vez de VLC
- Parar uma rádio ficou instantâneo (antes podia levar até alguns
  segundos em rádios de taxa baixa)
- Enquanto conecta, o título mostra o nome da favorita, não a URL

### Outros

- Capa do álbum anterior não fica mais presa ao abrir algo sem capa
- Fade do avanço dentro da faixa de volta ao tempo original, mais suave
- Programa mais leve: os podcasts só são carregados quando usados, e
  os arquivos de dados ficaram menores
- Preferências: log de conexões (diagnóstico), episódios guardados por
  podcast, tocar o próximo episódio ao terminar
- Instalador: pasta de plugins com permissão para o usuário, programa
  aberto após a instalação como usuário comum, aviso se o Winple
  estiver aberto durante a atualização

## 1.0.3

- O NVDA não fala mais "painel" nem "gráfico" ao voltar para a janela
- Alt+F4 fecha na hora, mesmo ouvindo rádio
- Álbuns e listas abertos pelo DOSVOX (ou pelo Explorer) substituem a
  lista atual em vez de acumular
- Fade ao avançar e retroceder na música mais curto

## 1.0.2

### Proteção contra bloqueio pelas rádios

- Corrigido laço infinito de reconexão quando o servidor aceitava e
  derrubava a conexão logo depois; agora desiste após 3 tentativas
- Limite de segurança de conexões por servidor, com aviso falado
- Servidor que recusa a conexão não recebe mais novas tentativas por
  outros caminhos
- Leitor de nome da música não fica mais consultando rádios que falharam
- X na mesma rádio não abre mais duas conexões; X repetido é ignorado
- Trocar rápido de favorita com B/Z conecta só a rádio onde você parou
- Rádio pausada por mais de 1 minuto libera a conexão

### Rádios em geral

- Rádios Shoutcast antigas abrem normalmente
- Quando uma rádio não abre, o NVDA avisa
- V enquanto uma rádio conecta cancela de verdade
- Endereço de rádio sem "http://" funciona

### Atalhos

- Ctrl+Z e Ctrl+B nas rádios favoritas (primeira e última)
- Navegação circular nas favoritas (B, Z, Numpad 1 e 3)
- B/Z não vão mais para a rádio errada depois de mover, remover ou
  importar favoritas
- Modo aleatório: Z, Numpad, Ctrl+Z e Ctrl+B voltaram a funcionar
  depois de mudar a lista
- Tecla barra (/) devolve velocidade e tom ao normal
- Volume, balanço, velocidade e tom avisam quando chegam no limite

## 1.0.1

### Rádio

- Reconexão automática **unificada**: agora rádios favoritas também
  tentam reconectar na mesma rádio (até 3 vezes, com espera crescente
  entre tentativas) antes de avançar pra próxima - antes, uma
  favorita pulava pra próxima na primeira queda, sem tentar voltar
  nela primeiro
- Reconexão configurável: opção "Tentar reconectar rádio antes de
  avançar" nas Preferências, ligada por padrão - desligando, volta a
  pular direto pro destino final assim que a rádio cair
- Proteção contra travamento quando a internet cai por completo: um
  limite total de falhas seguidas (em qualquer rádio, favorita ou
  não) faz o programa parar de vez, com um aviso único, em vez de
  ficar ciclando pelas favoritas sem parar - importante especialmente
  pra quem usa leitor de tela, já que tentativas rápidas demais em
  sequência podiam sobrecarregar o próprio NVDA
- Espera entre tentativas de reconexão agora é crescente (3s, 6s,
  12s), não fixa - mais respeitoso com os servidores das rádios, e
  reduz o risco de ser identificado como acesso automatizado

### Preferências

- Reorganizadas em duas seções: "Geral" primeiro, "Rádio" depois -
  antes as opções apareciam meio misturadas
- Corrigida a leitura pelo NVDA da opção "Tom/Velocidade": não é mais
  anunciada como se pertencesse ao grupo "Rádio"

### Desempenho

- Timer principal de atualização mais leve (1 segundo em vez de meio
  segundo) - os valores mostrados já não tinham mais resolução que
  essa, então rodar mais rápido só gastava processamento à toa
- Checagem de "outra instância tentou abrir o programa" separada num
  timer próprio, bem mais lento - antes rodava junto com o timer de
  reprodução, o tempo todo, mesmo com o programa parado
- Corrigido vazamento de memória: trocar de rádio favorita repetidas
  vezes numa sessão longa fazia a lista de reprodução crescer sem
  limite, pra sempre - agora a entrada atual é reaproveitada em vez
  de acumular

## 1.0.0

Primeira versão pública do **Winple Player**.

### Reprodução

- Toca MP3, WAV, OGG, FLAC, M4A, AAC, WMA e MPEG/MPG
- Rádios pela internet (Icecast, Shoutcast e HLS), sem cortes
- Listas de reprodução `.m3u`, `.m3u8` e `.pls` — abre e salva
- Modo aleatório que percorre todas as faixas antes de repetir,
  incluindo a primeira
- Repetir e aleatório ficam salvos entre sessões
- Volume salvo ao fechar
- Avanço automático para a próxima faixa quando uma falha, com
  proteção contra listas com várias faixas quebradas seguidas (para
  em vez de ficar tentando sem parar)
- Rádio avulsa (URL digitada, ou lista com uma única rádio) que cai
  sozinha durante a reprodução tenta reconectar na mesma URL antes de
  desistir, em vez de pular pra qualquer outra coisa - rádios
  favoritas continuam avançando pra próxima da lista normalmente,
  como sempre
- Reconhece na hora arquivos que claramente não são áudio (texto,
  manifestos de streaming de vídeo abertos por engano) - mostra um
  aviso direto, sem travar tentando
- Abrir um único arquivo pode carregar também as outras faixas da
  mesma pasta (configurável)

### Cruzamento entre faixas (crossfade)

- De 1 a 10 segundos, configurável nas Preferências
- Funciona ao avançar/retroceder manualmente (B, Z, Numpad 1/3,
  Ctrl+Z, Ctrl+B) e também na troca natural, no fim da faixa
- Equalizador/normalizador/VST/velocidade já aplicados na próxima
  faixa antes dela começar a tocar - sem salto perceptível
- Também funciona na troca de rádio (favoritas): técnica assimétrica
  - a rádio nova entra em volume cheio assim que conecta; a antiga
    desvanece suavemente só depois

### Rádios favoritas

- Cadastro com nome próprio, reordenável
- B e Z trocam entre as favoritas, como num radinho
- Exportar e importar em `.json`
- Nome da música ao vivo (metadados ICY) e nome da rádio, ambos no
  título da janela - formato "Artista - Música - Rádio - Winple
  Player", como no Winamp clássico
- Rádios em HLS tocam pela própria BASS (via `basshls.dll`), com a
  mesma confiabilidade das demais - o motor do Windows fica só como
  última reserva

### Pastas favoritas

- Cadastro de várias pastas
- Guarda o caminho, não a lista: músicas novas aparecem sozinhas

### Backup

- Exportar/importar só as rádios favoritas, num arquivo `.json`
- Exportar/importar TODAS as configurações de uma vez (preferências,
  pastas e rádios favoritas) - útil pra recuperar tudo rápido depois
  de reinstalar o programa ou trocar de computador

### Áudio

- Equalizador de três bandas (graves, médios, agudos)
- Efeitos: eco, reverberação, compressor, coro e flanger
- Normalizador de volume, com cinco intensidades
- Suporte a plugins VST 2.x, com vários simultâneos
- Velocidade e tom ajustáveis, com opção de preservar um ou o outro
- Por padrão, nada disso vale para rádio (cada uma já vem processada
  de quem transmite) - mas é configurável pra quem preferir
- Todos os ajustes ficam salvos

### Acessibilidade

- Uso completo por teclado
- Testado com NVDA
- Lista de atalhos navegável em F1
- Interface enxuta, sem avisos desnecessários
- Capa do álbum extraída dos arquivos
- Fala a porcentagem do volume ao ajustar nas setas (configurável) -
  o aviso de risco de distorção acima de 100% sempre fala, mesmo
  desligado

### Integração com o Windows

- Instalador com opções de menu de contexto e player padrão
- Instância única (configurável) - tentar abrir de novo traz a
  janela já aberta pra frente automaticamente, em vez de mostrar um
  aviso; reconectar na mesma rádio não gera mais instâncias
  sobrepostas
- Abre rápido: o motor de reserva do Windows só carrega quando
  realmente necessário, e o programa roda como uma pasta já pronta,
  sem precisar se descompactar toda vez
- Ferramenta para limpar entradas antigas do registro

### Notas técnicas

- Rádios tocam via BASS através de um proxy HTTP local, contornando
  problemas de negociação HTTPS do Windows Media Foundation com
  servidores Icecast
- A conexão com a rádio é montada manualmente (sem `urllib`), pra
  evitar bloqueio por parte de provedores que rejeitam especificamente
  esse tipo de pedido
- Arquivos locais também tocam pela BASS, para ter equalizador e
  efeitos; se a `bass.dll` faltar, volta ao motor do Windows
- Leitura de `.m3u`/`.pls` aceita UTF-8 e Latin-1, preservando acentos
  em arquivos salvos por ferramentas antigas
- Caminhos longos e com acentos tratados corretamente
