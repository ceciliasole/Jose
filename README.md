# Sílabas y Sonidos

Página estática de una sola pieza (`index.html`), sin dependencias ni paso de compilación. Pensada para publicarse en Vercel, igual que el portal de horas.

## Publicar en `jose.impactese.com`

1. <https://vercel.com/new> → **Import** `ceciliasole/Jose`. Framework: **Other**. Sin build command ni output directory. Production Branch: la rama que quieras publicar.
2. **Project → Settings → Domains → Add** → `jose.impactese.com`.
3. En el DNS de `impactese.com`, crear el `CNAME` de `jose` con el destino que muestre Vercel (si usás Cloudflare, "DNS only" hasta que emita el certificado). No tocar los registros existentes.

`vercel.json` pide a los buscadores que no indexen el sitio (`X-Robots-Tag: noindex`). Borrá ese bloque cuando quieran que aparezca en Google.
