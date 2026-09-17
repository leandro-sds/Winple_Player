# Histórico de versões

> **Sobre o nome:** este programa já se chamou *LS AudioPlayer*. A
> partir da versão 1.0.0 passou a se chamar **Winple Player** — um
> nome próprio, que não depende mais das iniciais do autor. É o mesmo
> programa, recomeçando a numeração de versões do zero sob o novo nome.

## 1.0.0

Primeira versão pública do **Winple Player**.

### Reprodução

- Toca MP3, WAV, OGG, FLAC, M4A, AAC e WMA
- Rádios pela internet (Icecast, Shoutcast e HLS), sem cortes
- Listas de reprodução `.m3u`, `.m3u8` e `.pls` — abre e salva
- Modo aleatório que percorre todas as faixas antes de repetir,
  incluindo a primeira
- Repetir e aleatório ficam salvos entre sessões
- Volume salvo ao fechar
- Avanço automático para a próxima faixa quando uma falha
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

### Integração com o Windows

- Instalador com opções de menu de contexto e player padrão
- Instância única (configurável) - reconectar na mesma rádio não gera
  mais instâncias sobrepostas
- Abre rápido: o motor de reserva do Windows só carrega quando
  realmente necessário, e o programa roda como uma pasta já pronta,
  sem precisar se descompactar toda vez
- Ferramenta para limpar entradas antigas do registro

### Notas técnicas

- Rádios tocam via BASS através de um proxy HTTP local, contornando
  problemas de negociação HTTPS do Windows Media Foundation com
  servidores Icecast
- Arquivos locais também tocam pela BASS, para ter equalizador e
  efeitos; se a `bass.dll` faltar, volta ao motor do Windows
- Leitura de `.m3u`/`.pls` aceita UTF-8 e Latin-1, preservando acentos
  em arquivos salvos por ferramentas antigas
- Caminhos longos e com acentos tratados corretamente
