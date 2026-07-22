# Inventário.Log — Site

Site institucional em HTML/CSS puro (sem build, sem framework), pensado para ir evoluindo aos poucos até virar o site oficial da empresa.

## Estrutura

```
index.html                 → landing page (home)
assets/css/site.css        → estilos compartilhados (cores, tipografia, componentes)
servicos/inventario-log.html → apresentação completa do app (deck standalone)
servicos/consultoria.html    → apresentação completa da consultoria (deck standalone)
```

A paleta e as fontes (Sora, Inter, IBM Plex Mono) foram extraídas das duas apresentações originais para manter a mesma identidade visual em todo o site.

## Rodar localmente

Como é HTML puro, basta abrir `index.html` no navegador. Para simular melhor um ambiente de produção (URLs relativas, etc.), rode um servidor local, por exemplo:

```
npx serve .
```

ou, com Python:

```
python -m http.server
```

## Deploy

O site é publicado via **GitHub Pages**, direto a partir da branch `main` (pasta raiz). Qualquer commit enviado para `main` atualiza o site publicado em alguns minutos.

## Próximos passos (TODO)

- Substituir os contatos de exemplo em `index.html` (seção `#contato`) pelos reais.
- Adicionar logo/favicon definitivo em `assets/img/`.
- Revisar o texto da seção "Sobre" com a história real da empresa.
- Avaliar transformar os decks de `servicos/` em páginas de serviço no mesmo estilo do site (hoje eles ainda são as apresentações originais, incorporadas como estão).
