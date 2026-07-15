# Notas Player

Página HTTPS mínima usada pelo plugin UXP **Notas** para apresentar vídeos do YouTube e streams HLS `.m3u8` com uma origem web identificável.

## Parâmetros

- `v`: identificador de 11 caracteres do vídeo.
- `start`: segundo inicial opcional.
- `hls`: URL HTTPS codificado de um stream `.m3u8`.

Exemplo:

`https://paulojorgebranco.github.io/notas-player/?v=XPtWTT9eY4M&start=67`

`https://paulojorgebranco.github.io/notas-player/?hls=URL_M3U8_CODIFICADO`

O leitor HLS dedicado está em:

`https://paulojorgebranco.github.io/notas-player/hls.html?src=URL_M3U8_CODIFICADO`

Os streams HLS têm de permitir pedidos CORS e não podem depender de uma sessão ou autenticação indisponível no webview.

A página não guarda dados, não usa analytics próprios e não comunica com o plugin.

Os leitores começam com o volume no mínimo audível: 1%.
