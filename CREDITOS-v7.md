# Cloudsurfer 3 — da caixa para o mundo, versão 7

Filme conceitual independente de 104 segundos, horizontal Full HD, 30 fps. O epílogo acrescenta 12 segundos à versão 6, dentro do limite de 15 segundos solicitado. Sem vínculo oficial com a On. As versões 2 a 6 permanecem preservadas.

## Jornada preservada

A abertura com logo, montanha, apresentação do produto, separação e remontagem das quatro camadas, pisada/corrida, site em perspectiva 3D, sacola, confirmação, embalagem e mapa continuam presentes. O fechamento do produto foi deslocado para 99–104 s para acomodar o novo epílogo entre 87 e 99 s. Para montar os primeiros 87 s, são reutilizados os segmentos de render anteriores, em vez do MP4 final v6 como intermediário, evitando uma geração adicional de compressão. O novo master usa H.264 CRF16.

A procedência das fotografias oficiais, dos componentes reais, das filmagens On, da montanha NPS e da embalagem de Kampus Production/Pexels, incluindo URLs, licença, recortes e limites de apresentação, está em [CREDITOS-v6.md](./CREDITOS-v6.md) e nos créditos anteriores. Não foram gerados novos vídeos de pessoas. O material de embalagem representa a preparação de um pedido e não é apresentado como uma instalação ou funcionário oficial da On.

## Novo epílogo

“Da caixa para o mundo” conecta a chegada do pedido ao produto em movimento. A montagem usa detalhes e filmagens oficiais do Cloudsurfer 3 já existentes, com novo enquadramento, tipografia animada e transições. O plano de partículas é CGI oficial; as cenas com pernas e calçado em movimento são filmagens reais. Não se afirma vitória em corrida ou endosso de atleta.

Fontes oficiais do novo epílogo, obtidas a partir da [collection Cloudsurfer 3](https://www.on.com/en-us/collection/cloudsurfer3):

| Tempo no filme | Fonte e recorte | Apresentação |
|---|---|---|
| 87,00–88,60 s | [Macro do solado](https://videos.ctfassets.net/hnk2vsx53n6l/4GuIMyxrssNbXix9bxaoVP/484a6bcb001193f2f9342161bc32d457/On%C3%A2__Cloudsurfer_3_GRADED00663858_2_1.mp4), original 0,00–1,60 s | Detalhe oficial do produto, velocidade 1× |
| 88,60–90,50 s | [Partículas formando a base](https://videos.ctfassets.net/hnk2vsx53n6l/5TbuTugrTpB7OXkTZnHzqL/a074b592cc98dd414d5fbe218304cc46/On%C3%A2__Cloudsurfer_3_GRADED00590932_2_1.mp4), original 3,10–5,00 s | CGI oficial, velocidade 1× |
| 90,50–95,00 s | [Pisada, filme oficial quadrado](https://videos.ctfassets.net/hnk2vsx53n6l/2h9g8vFkgXuiPDjZRdNaz0/e51b799fdf204a361ad2561d4dc54eb0/fw26-cloudsurfer3-pr-product_video-1x1-no_vo-no_sub-6s-none-01_1.mp4), original 0,00–2,25 s | Filmagem real; 0,5× com interpolação de quadros, recorte 2160 × 1216 e saída 1920 × 1080 |
| 94,60–98,60 s | [Corrida, filme oficial 4:5](https://videos.ctfassets.net/hnk2vsx53n6l/1NYgVcfrO0XrvrBVAAbI4K/94767e7d58dbd532597edf7e74df2857/fw26-cloudsurfer3-pr-product_video-4x5-no_vo-no_sub-15s-none-02_1__1__1.mp4), original 11,70–13,60 s | Filmagem real; 0,475× com interpolação para 4 s, 864 × 1080 e 30 fps, proporção vertical preservada dentro da composição; entrada sobreposta à pisada e último quadro mantido durante a saída para papel |

SHA-256 dos arquivos oficiais: macro `72bdf7ef1231de7a9e185f952853a1b526cd39a73c50ff3a98f21e65a3c44706`; partículas `bdae249f9175862892421fba3fe8962d66449afd44b820daa0f8d26d3da1b660`. A procedência e as dimensões originais constam em `out/v5-research/downloaded.json`. Os dois novos recortes reais, respectivos arquivos, hashes, fontes e processamento estão registrados em `out/v7-new-footage.json`. Os áudios originais foram removidos. Os materiais da On são citados como fontes oficiais para este estudo criativo independente; não se afirma que tenham licença aberta de stock.

## Interface e ilustração dimensional

A interface, a compra e o mapa são conceitos animados. Não há transação, preço, endereço, pagamento ou rastreamento reais. A casa representa um destino genérico. O tênis técnico usa fotografias oficiais projetadas sobre meshes com espessura e câmera limitada; as superfícies ocultas são interpretações gráficas, sem se apresentar como GLB oficial, digitalização completa ou modelo de engenharia.

## Voz, música e tipografia

Narração sintética em português brasileiro com Piper Faber medium; a procedência do modelo e de seu conjunto de dados consta em [CREDITOS-v3.md](./CREDITOS-v3.md). A nova trilha e os efeitos foram sintetizados para o projeto, sem amostragem de música de terceiros. Frases e tempos constam em `out/finale-v7-voice-manifest.json`. A medição do áudio efetivamente exportado consta em `out/validation-v7.json` após a validação.

Tipografia Inter, sob SIL Open Font License, conforme [CREDITOS-v4.md](./CREDITOS-v4.md). Animação e render em Remotion/Three.js e composição de vídeo; a intenção visual segue o motion graphic solicitado, sem alegar produção no software After Effects.

## Conferência e preparação de entrega

`scripts/validate-finale-v7.py` verifica 3.120 quadros a 30 fps, duração de 104 s, 1920 × 1080, H.264, AAC estéreo a 48 kHz, decodificação integral, volume do áudio exportado, manifestos de voz e das novas filmagens, e preservação dos MP4 v2–v6 por SHA-256. Gera `out/validation-v7.json` e `out/finale-v7-final-contact.png`, com 30 quadros em grade 6 × 5, incluindo o epílogo e a assinatura do produto.

`scripts/prepare-finale-v7.py` prepara somente um commit local com índice isolado, preservando os blobs de todas as versões anteriores. Não executa push nem publica o vídeo. O recibo local é `delivery-v7.json`, destinado à branch `on-motion-preview`.
