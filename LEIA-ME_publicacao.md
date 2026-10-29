# HFM — publicar a página de testes (GitHub Pages)

Arquivos desta pasta:
- `index.html` — a página de apresentação (o cartaz), com o botão "Quero testar".
- `guia-instalacao.html` — o guia passo a passo.
Os dois ficam na mesma pasta e se ligam por link relativo (`guia-instalacao.html` e `index.html`), então funcionam em qualquer hospedagem, sem editar nada.

## Passo a passo
1. No GitHub, crie um repositório **novo e público**, por exemplo `hfm-site`. Não use o `hfm-gas`: ele é privado e tem o código do sistema.
2. Envie `index.html` e `guia-instalacao.html` (Add file > Upload files > Commit).
3. Em Settings > Pages: Source = "Deploy from a branch", Branch = `main`, pasta `/ (root)`. Salvar.
4. Em 1 a 2 minutos o endereço aparece ali mesmo: `https://devdias-techsolutions.github.io/hfm-site/` (o guia fica em `.../hfm-site/guia-instalacao.html`).
5. Abra no celular e no computador e clique em "Ver o guia de instalação" e de volta (logo no topo do guia).

## Para atualizar depois
Edite ou reenvie o arquivo no mesmo repositório e faça commit. A página atualiza em cerca de 1 minuto.

## Fluxo com os testadores
1. A pessoa abre a página e clica em "Quero testar" (e-mail para devdiastechsolutions@gmail.com).
2. Você responde com o **link da planilha-modelo** (formato `/copy`) e o **endereço do guia**.
3. Mantenha o link da planilha-modelo fora das páginas públicas: assim você controla quem recebe.

## Fase de testes x lançamento
As duas páginas têm `<meta name="robots" content="noindex, nofollow">`, para não aparecerem no Google enquanto o teste é fechado. Quando quiser divulgar, apague essa linha.

## O que foi ajustado nos arquivos originais
- Link do guia no cartaz: de um endereço de artefato do Claude para `guia-instalacao.html`.
- Adicionado o que faltava para funcionar como página própria: `<!doctype>`, `charset` UTF-8, `viewport` (sem ele o celular mostra a página como desktop encolhido), `lang`, descrição, título de compartilhamento e ícone (a logo).
- No guia, a logo do topo agora volta para a página inicial.
