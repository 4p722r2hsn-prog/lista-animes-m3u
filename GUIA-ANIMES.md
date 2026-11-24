# Catálogo de animes — Saimo TV

Este repositório está sendo preparado para organizar animes no Saimo TV.

## Importante sobre a reprodução

O Saimo TV é um reprodutor: ele não hospeda episódios. Para que um episódio toque, o arquivo `redeflix/links-animes.txt` precisa conter uma fonte de vídeo direta e autorizada (por exemplo, um endereço HLS ou MP4 que o usuário tenha direito de acessar). Links de páginas de streaming, páginas de busca e endereços inventados não funcionam como fontes.

Por isso, este guia não inclui links piratas nem fontes fictícias. O arquivo M3U atual foi mantido intacto para não quebrar o que já existe.

## Seleção editorial sugerida

### Clássicos
- Death Note
- Fullmetal Alchemist: Brotherhood
- Hunter x Hunter (2011)
- Naruto
- Code Geass
- Steins;Gate

### Séries recentes (2025)
- Solo Leveling — 2ª temporada
- Sakamoto Days
- DAN DA DAN — 2ª temporada
- Kaiju No. 8 — 2ª temporada
- My Hero Academia — temporada final

### Lançamentos / continuações de 2026
- Jujutsu Kaisen — 3ª temporada
- Frieren e a Jornada para o Além — continuação
- Oshi no Ko — 3ª temporada

A disponibilidade de áudio japonês e legendas em português do Brasil varia por serviço, região e temporada; deve ser confirmada em cada fonte oficial.

## Formato que o Saimo espera

O arquivo de animes é `redeflix/links-animes.txt`. Cada título começa com:

```text
@Título do Anime<TAB>ANO<TAB>ID
```

E cada episódio precisa de uma linha no formato:

```text
TEMPORADA<TAB>EPISÓDIO<TAB>leg<TAB>FONTE_DIRETA_AUTORIZADA
```

Sem uma fonte direta autorizada, não há como prometer reprodução. O exemplo oficial de formato está na documentação do Saimo: https://github.com/SaimoTV/SaimoPlayer/blob/main/docs/formato-saimo.md

## Próximo passo técnico

Quando houver fontes diretas autorizadas, o catálogo pode ser publicado na pasta de filmes e séries e conectado em **Ajustes → Listas** no Saimo. A pasta precisa conter também o índice e os demais arquivos obrigatórios do formato Saimo.
