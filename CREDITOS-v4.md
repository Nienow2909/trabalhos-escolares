# Cloudsurfer 3 — motion graphic, versão 4

Conceito criativo independente, sem vínculo oficial com a On. Filme horizontal de 50 segundos, 1920 × 1080, 30 fps, com narração em português brasileiro, trilha instrumental original e animação gráfica tridimensional.

## Imagem e produto

As fotos e filmagens de pessoas e do tênis já existiam. Fontes, autores e recortes estão detalhados em [CREDITOS-v2.md](./CREDITOS-v2.md). As mesmas fontes são usadas nesta remontagem: fotos e filmes oficiais do Cloudsurfer 3, plano NPS de montanha e celebração de Arian Ojili/Pexels. A montanha e a celebração são cenas de atmosfera, sem comprovar uso do produto, resultado de vitória ou endosso dos participantes.

A demonstração real de compressão da entressola usa CGI oficial existente, em um painel compatível com a resolução da fonte. O plano em camadas mostra peças físicas já separadas em laboratório; as chamadas identificam palmilha, entressola e solado. A reprodução inversa seguida de um plano do tênis montado é uma transição de edição.

As células ocas e a tipografia extrudada foram construídas em Three.js para a direção gráfica, com luzes e reflexos procedurais de estúdio. São formas explicativas e letras em 3D, sem pretensão de representar geometria técnica fiel do tênis. Não foi criado um modelo 3D completo do Cloudsurfer. O produto é apresentado pelas fotos e filmagens oficiais.

Tipografia 2D: Inter, SIL Open Font License. Tipografia 3D: Helvetiker Bold do pacote Three.js, com licença MAGENTA Ltd. (2004) distribuída em `three/examples/fonts/LICENSE`. Three.js é distribuído sob licença MIT.

## Narração e música

Voz sintética predefinida Piper Faber medium, português brasileiro. Procedência e SHA-256 do modelo em [CREDITOS-v3.md](./CREDITOS-v3.md); o model card declara dataset CC0. As grafias fonéticas usadas na síntese de nomes em inglês não alteram os nomes apresentados na imagem.

Nova trilha e efeitos de transição de 50 segundos, sintetizados para esta versão. Sem amostras de música de terceiros. A mixagem mantém a voz ao centro, reduz o instrumental durante as falas e deixa pausas entre elas. Medição da fonte WAV: −17,13 LUFS integrados, −1,4 dBTP, estéreo 48 kHz/24 bits. Script local `scripts/generate-premium-audio.py`.

## Produção e revisão

Composição Remotion `OnCloudsurferPremium`; gráficos 3D em `PremiumDepth.tsx`. Renderização Chromium/SwiftShader, H.264 e AAC estéreo. As versões 2 e 3 permanecem preservadas para comparação. A versão 4 remonta a narrativa completa com nova voz, música, transições e animação, em vez de anexar outro bloco ao filme anterior.

Quadros representativos da abertura, paisagem, produto, 3D, demonstrações técnicas, corrida e assinatura foram revisados. A exportação final passa por leitura de metadados e decodificação integral; o recibo de entrega registra os resultados e o hash do MP4.
