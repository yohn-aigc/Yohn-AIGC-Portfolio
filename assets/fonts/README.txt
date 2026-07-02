字体说明（fonts/）
==================
本站字体全部通过 Google Fonts CDN 在 index.html <head> 的 <link> 里加载：
  Inter / Instrument Serif / Caveat / JetBrains Mono
因此本目录默认留空——无需本地字体文件，也不需要 @font-face。

如果将来要改成「本地字体」以摆脱 CDN 依赖：
  1. 把 .woff2 等字体文件放进本目录 (assets/fonts/)。
  2. 在 src/index.css 里用 @font-face 声明，src 指向 ./assets/fonts/xxx.woff2。
  3. 删除 index.html 中对应的 Google Fonts <link>。
在此之前，请保持 index.html 的 CDN <link> 不动，以免字体加载失效。
