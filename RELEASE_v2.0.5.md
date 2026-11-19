# Winple Player 2.0.5

## Botões de mídia
- O Winple Player agora responde aos botões de fones de ouvido e caixas de som Bluetooth: tocar e pausar, próxima e anterior, conforme os botões que o aparelho tiver.
- As teclas de mídia do teclado (tocar/pausar, próxima, anterior e parar) também controlam o Winple, mesmo com ele minimizado.
- No Windows 10 e 11, o Winple aparece no painel de mídia do Windows (ao lado do controle de volume), mostrando o que está tocando. Na rádio, aparece a música do momento quando a rádio informa.
- Os botões de volume do fone continuam controlando o volume do Windows ou do próprio fone, como em qualquer programa.
- O recurso pode ser desligado nas Preferências, na opção "Responder aos botões de mídia".
- Como em qualquer player, os botões ficam com o último programa que tocou alguma coisa: se você estava num vídeo do navegador e depois deu play no Winple, os botões passam a ser do Winple.

## Arquivos compactados
- Novo: Arquivo, Abrir arquivo compactado (Ctrl+Alt+L). Abre ZIP, RAR, 7z e TAR (inclusive .tar.gz, .tar.bz2 e .tar.xz) e toca as músicas e vídeos que estão dentro, com todos os recursos de sempre: plugins, efeitos, crossfade e posição.
- O Winple descompacta só os arquivos de áudio e vídeo, numa pasta própria, e abre essa pasta. Enquanto descompacta, dá para cancelar.
- Nada fica acumulado no computador: os arquivos descompactados são apagados quando o Winple fecha. Por isso, uma lista vinda de um arquivo compactado não é reaberta na próxima vez; o Winple avisa e basta abrir o arquivo de novo.
- Se um arquivo compactado for aberto por engano em "Abrir lista de reprodução" (Ctrl+Shift+L), o Winple avisa: "Para abrir arquivo compactado, pressione Ctrl+Alt+L".
- Arquivos protegidos por senha ou danificados são avisados, e a lista atual não é mexida.

## Diagnóstico e suporte
- Quando um vídeo não toca porque falta um arquivo do VLC (em geral, removido pelo antivírus), o Winple agora diz exatamente qual arquivo falta e como resolver, em vez da mensagem genérica.
- Novo: Ajuda, Verificar arquivos do Winple. Confere se os arquivos de áudio e vídeo do programa estão todos no lugar e, se houver problema, copia um pequeno relatório para colar num e-mail ao suporte.
- Novo: Preferências, Gravar registro de diagnóstico (desligado por padrão). Ligado, o Winple registra o que acontece e qualquer erro inesperado, num arquivo que se abre por Ajuda, Abrir pasta do registro de diagnóstico, para enviar ao suporte quando algo der errado. Ele substitui as duas opções de registro que existiam antes.
- A cada atualização, a parte de vídeos (VLC) é instalada de novo por inteiro. Se algum arquivo dela tiver sido apagado, a atualização já repara.

## Novidades da versão
- Novo: Shift+F1, ou Ajuda, O que há de novo nesta versão. Mostra estas novidades a qualquer momento. Depois de cada atualização, elas também aparecem sozinhas, uma vez, quando o Winple abre.

## Correções
- "Abrir lista de reprodução" agora recusa arquivos que não são listas (áudio, vídeo, programas, compactados). Antes, abrir um arquivo assim por ali enchia a lista de "faixas" sem sentido e podia deixar o arquivo de configurações enorme, deixando o Winple lento para abrir.
- Se o arquivo de configurações estiver danificado e grande demais, o Winple o deixa de lado sozinho, volta às configurações padrão e avisa. Rádios, podcasts e biblioteca não são afetados.

## Como instalar / atualizar
Quem está na versão 2.0.4 recebe esta atualização por dentro do programa: basta responder "Sim, baixar e instalar" no aviso de versão nova.

Quem está numa versão anterior baixa o WinplePlayer_Setup_V2.0.5.exe abaixo e executa. Ele instala por cima da versão anterior, mantendo suas configurações.
