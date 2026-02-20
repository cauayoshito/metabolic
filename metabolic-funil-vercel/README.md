# Funil Metabolic Manual (Vercel Ready)

## Estrutura
- `/index.html` -> Página do Manual (R$11,97) -> redireciona para checkout Greenn
- `/upsell/index.html` -> Upsell (R$27) -> checkout Greenn
- `/downsell/index.html` -> Downsell (R$17) -> checkout Greenn
- `/obrigado/index.html` -> Obrigado + download do PDF

## Configuração (obrigatório)
Edite:
- `/assets/config.js`

Preencha:
- `checkouts.manual` (Greenn checkout manual)
- `checkouts.upsell` (Greenn checkout upsell)
- `checkouts.downsell` (Greenn checkout downsell)
- `delivery.manualPdfUrl` (link direto do PDF)
- `support.whatsappUrl` (whatsapp suporte)

## Deploy na Vercel (static)
1. Suba estes arquivos em um repositório GitHub.
2. Na Vercel, importe o repo.
3. Framework Preset: **Other**
4. Build Command: **vazio**
5. Output Directory: **.** (raiz)
6. Deploy.

## Configurar redirecionamento no Greenn
- Produto Manual -> Página de obrigado: `https://SEUDOMINIO/upsell/`
- Produto Upsell -> Página de obrigado: `https://SEUDOMINIO/obrigado/?src=upsell`
- Produto Downsell -> Página de obrigado: `https://SEUDOMINIO/obrigado/?src=downsell`

Pronto.
