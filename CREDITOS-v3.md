# Cloudsurfer — versão estendida com tipografia em stop motion

Vídeo horizontal Full HD de aproximadamente 50 segundos. Os 30 segundos da versão 2 permanecem integralmente no início; foi acrescentada uma sequência de 20 segundos. Conceito criativo independente, sem vínculo oficial com a On.

A sequência adicional usa as mesmas fotos e filmagens oficiais do Cloudsurfer 3 citadas em [CREDITOS-v2.md](./CREDITOS-v2.md), sem gerar novas filmagens. Letras entram em poses discretas, mantidas por três quadros, sincronizadas às frases da narração. Os textos técnicos destacam Surreal™, CloudTec Phase™ e cabedal warp knit.

## Áudio adicional

- Narração sintética em português brasileiro, voz predefinida Faber medium, gerada localmente com Piper. Não reproduz a identidade de uma pessoa escolhida para o anúncio.
- Modelo: [pt_BR-faber-medium](https://huggingface.co/rhasspy/piper-voices/tree/main/pt/pt_BR/faber/medium). [Model card](https://huggingface.co/rhasspy/piper-voices/blob/main/pt/pt_BR/faber/medium/MODEL_CARD), conjunto de dados declarado CC0. SHA-256 do modelo: `858555e3a064209c57088fe6bd70c4c3dc54d03eaa00c45d5ecaf43a33f95aa7`.
- Instrumental: trecho da composição original já criada para o projeto, em volume reduzido sob a voz. Efeitos curtos sintetizados para as entradas das palavras. Sem amostras de música de terceiros.
- As grafias fonéticas utilizadas na síntese de nomes em inglês afetam somente a pronúncia da voz; a tipografia usa os nomes originais do produto.

## Preservação e exportação

O complemento foi renderizado separadamente e anexado por cópia dos fluxos H.264/AAC. O processo confere os 900 quadros decodificados originais e os dados dos pacotes originais de vídeo e áudio, além de decodificar o arquivo final inteiro. A pequena diferença de milissegundos na duração do contêiner corresponde ao preenchimento do áudio AAC.

Scripts locais: `scripts/generate-voice.py`, `scripts/mix-stop-audio.py` e `scripts/append-stop-motion.py`. A composição original e seu arquivo MP4 permanecem intactos.
