# Catálogo de animes — Saimo TV

Este projeto organiza uma seleção de animes para o Saimo TV, priorizando áudio japonês e legendas em português do Brasil (PT-BR).

## Situação real do projeto

- A seleção editorial está organizada em [SELECAO-ANIMES.md](SELECAO-ANIMES.md).
- O arquivo de reprodução do Saimo ainda não está pronto: faltam fontes de vídeo diretas, autorizadas e compatíveis.
- Não vou colocar links de páginas como se fossem arquivos de vídeo, nem inventar endereços HLS/MP4. Isso faria o catálogo parecer pronto, mas os episódios não tocariam.

## Como o Saimo lê animes

Segundo a documentação oficial, o arquivo opcional de animes fica em:

`redeflix/links-animes.txt`

Cada anime começa com uma linha contendo título, ano e ID, separados por TAB:

```text
@Título do Anime<TAB>ANO<TAB>ID
```

Cada episódio usa quatro colunas separadas por TAB:

```text
TEMPORADA<TAB>EPISÓDIO<TAB>VERSÃO<TAB>FONTES
```

Exemplo de estrutura (apenas ilustrativo; os endereços abaixo não são fontes reais):

```text
@Anime de Exemplo<TAB>2024<TAB>99
1<TAB>1<TAB>leg<TAB>https://servidor-autorizado/exemplo-episodio-1.m3u8
```

As versões podem ser `dub` (dublado) ou `leg` (legendado). As fontes precisam ser endereços de vídeo completos e acessíveis legalmente. O exemplo oficial também mostra a possibilidade de fontes de reserva.

## Como usar no Saimo

O formato completo do Saimo é publicado em arquivos hospedados na internet. Em **Ajustes → Listas**, o app recebe os endereços-base de canais e de filmes/séries. O arquivo de animes fica dentro da pasta de filmes/séries, em `redeflix/links-animes.txt`.

A documentação oficial explica os demais arquivos obrigatórios, a hospedagem HTTPS e o validador:
https://github.com/SaimoTV/SaimoPlayer/blob/main/docs/formato-saimo.md

## O que falta para ativar a reprodução

1. Confirmar uma fonte oficial que ofereça o anime no Brasil.
2. Confirmar que a fonte permite acesso direto autorizado ao vídeo (não apenas à página do episódio).
3. Confirmar áudio japonês e legenda PT-BR para a temporada/episódio.
4. Só então adicionar o episódio ao arquivo do Saimo e validar a lista.

**Importante:** links de Crunchyroll, Max, YouTube ou outras páginas oficiais podem servir como referência para assistir no serviço, mas não são automaticamente links diretos que o Saimo consiga reproduzir. Não use credenciais, cookies ou links privados de contas.
