# Nossa Contagem Regressiva 💍

Página única e privada com um cronômetro para o dia 22/08/2027 às 16h e um carrossel de fotos do casal. Feita para ser compartilhada apenas com a noiva.

## Estrutura

- `nossa-contagem-regressiva.html` — site completo (HTML, CSS e JS em um único arquivo, sem dependências externas além das fontes do Google Fonts).

## Como abrir

Basta abrir o arquivo `nossa-contagem-regressiva.html` diretamente no navegador (duplo clique) — não precisa de servidor nem de instalação.

## Como trocar a data do cronômetro

No arquivo HTML, procure a linha:

```js
var target = new Date('2027-08-22T16:00:00-03:00');
```

e ajuste a data/hora conforme necessário (formato `AAAA-MM-DDTHH:MM:SS-03:00`, fuso de Brasília).

## Como trocar as fotos do carrossel

Cada foto está marcada com a etiqueta "Adicione uma foto sua aqui" dentro de um bloco `<div class="slide">`. Para usar fotos reais:

1. Substitua o `<div class="wash">...</div>` de cada slide por uma tag `<img src="..." alt="...">` apontando para a foto (local ou em base64).
2. Remova a tag de placeholder (`<span class="tag">`) do slide correspondente.
3. Ajuste as legendas no array `captions` dentro do `<script>`, no final do arquivo.

## Paleta e tipografia

- Cores: terracota (`#b85c38`), creme (`#fbf3e7`), verde-sálvia (`#7c8a5e`) e tons de blush, inspirados na paleta enviada.
- Fontes: Cormorant Garamond (títulos), Parisienne (toques manuscritos) e Jost (textos e números do cronômetro).

## Versão publicada

O site também está publicado como uma página privada, atualizável pelo Claude sempre que o arquivo local mudar.
