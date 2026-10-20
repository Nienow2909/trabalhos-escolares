# Cloudsurfer 3 — camadas e jornada da compra à entrega, versão 6

Filme conceitual independente de 92 segundos, horizontal Full HD, 30 fps. Sem vínculo oficial com a On. As versões 2, 3, 4 e 5 permanecem preservadas.

## Abertura e remontagem do tênis

A sequência apresenta o tênis montado, separa cabedal, palmilha, entressola e solado, descreve cada componente e remonta o produto. CloudTec Phase™ e Surreal™ são apresentados na mesma entressola; não foi acrescentada uma placa Speedboard ou uma quinta camada.

A animação é uma ilustração dimensional construída com fotos oficiais projetadas sobre meshes com espessura e animadas em espaço 3D. A palmilha e as duas peças do solado usam imagens dos componentes reais em um quadro do filme de laboratório. Superfícies ocultas e espessuras são interpretações gráficas: não se trata de um GLB oficial, digitalização completa ou modelo de engenharia. Não foi utilizado o modelo de outro tênis como se fosse um Cloudsurfer.

Fotos: `hero-cloudsurfer3-billboard.jpg`, da [collection oficial Cloudsurfer 3](https://www.on.com/en-us/collection/cloudsurfer3), conforme [CREDITOS-v2.md](./CREDITOS-v2.md). Quadro de palmilha: 2,12 s de `cloudsurfer3-layers.mp4`, derivado do filme oficial citado nos créditos anteriores.

## Filmagens reais preservadas da versão 5

- Pisada e compressão sobre pedra em estúdio: [filme original](https://videos.ctfassets.net/hnk2vsx53n6l/nmBX4YSrxkTDdcN13t61x/1ebc9094461004a39a4ab0dd3abcf98c/a67a294f-bf7a-4875-a7a2-9cebe10a2ea3_1.mp4), fonte na mesma collection oficial; trecho 0,20–4,20 s, sem áudio original.
- Corrida em esteira: [tech-film-standard-desktop.mp4](https://videos.ctfassets.net/hnk2vsx53n6l/3mAjMRCT6GLz4kKNPyrKK3/c5e3e5ebd47d039c89fd475bf8249343/tech-film-standard-desktop.mp4), trecho 14,40–20,40 s, sem áudio original. Planos do produto em movimento, sem os apresentadores.
- Montanha: plano NPS já creditado em [CREDITOS-v2.md](./CREDITOS-v2.md), usado como atmosfera, sem identificar o calçado do participante.

Essas fontes oficiais e o material NPS mantêm a procedência e os limites descritos em [CREDITOS-v5.md](./CREDITOS-v5.md) e nos créditos anteriores. As filmagens já existiam; não foram gerados novos vídeos de pessoas. Não se estabelece vitória em corrida ou endosso de atletas.

## Nova filmagem de embalagem

“[Person Putting a Product In a Box](https://www.pexels.com/video/person-putting-a-product-in-a-box-7855140/)”, de [Kampus Production](https://www.pexels.com/@kampus/), Pexels, vídeo 7855140. Uso sob a [Pexels License](https://www.pexels.com/license/), que permite uso e edição gratuitos, inclusive comercial; atribuição é apreciada, mas não obrigatória.

O arquivo original público, 2560 × 1440 a 25 fps, foi recortado de 0,25 a 12,25 s, acelerado em 1,5× e exportado como `public/media/v6-packing-real.mp4`: 8 s, 1920 × 1080, 30 fps, sem áudio. SHA-256 do recorte: `430162d8326784e693eb1b761344f33732d9c1f4b0f837a9546aa3d056d091b4`. A procedência completa, o URL do MP4, o hash original e o processamento constam em `out/v6-packing-source.json`.

Na montagem, o recorte de 8 s é acelerado para caber em 7 s, mantendo o início e o fechamento da caixa. A cena mostra mãos colocando um produto embrulhado numa caixa kraft e fechando a tampa. É uma representação de preparação de pedido, sem alegar que seja uma instalação, funcionário ou embalagem oficial da On.

## Site, sacola, confirmação e mapa

A interface de produto, a adição à sacola, a confirmação de compra e o mapa do percurso até uma casa foram desenhados e animados para este conceito. A interface em perspectiva 3D não captura nem executa uma compra real. Não há transação, dados de pagamento, endereço, preço ou rastreamento reais. O percurso é ilustrativo; a casa não representa a residência do usuário.

## Texto, voz, música e tipografia

Textos e narração em português descrevem as quatro camadas e a jornada ilustrativa do pedido sem acrescentar materiais, placas ou promessas de desempenho não comprovadas. Narração sintética em português brasileiro com Piper Faber medium; modelo e procedência em [CREDITOS-v3.md](./CREDITOS-v3.md). Frases, tempos e parâmetros da nova mixagem constam em `out/journey-v6-voice-manifest.json`.

Instrumental e efeitos foram sintetizados para o projeto, sem música de terceiros amostrada. A medição do áudio efetivamente exportado consta em `out/validation-v6.json` após a validação. Tipografia Inter/OFL, conforme [CREDITOS-v4.md](./CREDITOS-v4.md). Render com Remotion/Three.js; as transições seguem a intenção visual solicitada, sem alegar produção no software After Effects.

## Conferência e preservação

O validador `scripts/validate-journey-v6.py` verifica 2.760 quadros a 30 fps, duração de 92 s, 1920 × 1080, H.264, áudio AAC estéreo a 48 kHz, decodificação integral, volume do áudio exportado, manifesto da voz e preservação dos MP4 anteriores por SHA-256. Ele produz `out/validation-v6.json` e um contato de 24 quadros em grade 6 × 4, incluindo as etapas de compra, embalagem e mapa.

O preparador `scripts/publish-journey-v6.py` cria apenas um commit local com índice isolado, preservando os arquivos anteriores. Não executa push nem publica o vídeo; o recibo de preparação é `delivery-v6.json`, destinado à branch `on-motion-preview`.
