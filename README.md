# links-andreia-tiktokshop

Landing page estática estilo Linktree pra @comprecomandreia (TikTok Shop).

**Live**: https://sheraos.com.br/compre-com-andreia

## Stack
- HTML/CSS puro, sem build
- Fonte: Google Fonts (Inter)
- Foto local: `andreia.jpeg`

## Editar produtos

No `index.html`, dentro de `<nav class="links">`:

- O primeiro `<a class="link-card">` é o card visível atual. Troca o `href` e os textos.
- Os outros 4 cards estão dentro de um comentário HTML (`<!-- ... -->`). Pra reativar, descomenta o bloco e troca os `href`.

## Trocar emoji por foto real do produto

```html
<span class="thumb t-1" aria-hidden="true">👖</span>
```
vira
```html
<span class="thumb t-1"><img src="produto1.jpg" alt="" style="width:100%;height:100%;object-fit:cover;border-radius:14px"></span>
```

## Deploy na VPS

```bash
cd /opt/andreia-links
git pull
# nginx serve estático, sem build
```
