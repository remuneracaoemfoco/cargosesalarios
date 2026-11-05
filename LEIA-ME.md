# Páginas oficiais do funil de VSL (2026-11-05)

Pasta pronta com as 6 páginas do funil, para copiar para a raiz do repositório remuneracaoemfoco/cargosesalarios (deploy automático na Vercel).
Cada pasta tem o nome da URL oficial. Substituem as pastas de teste com o mesmo nome (pg01-of01).

| Pasta | Origem aprovada |
|---|---|
| fcs-entrada-pg01-of01 | 2026-11-05_pagina-entrada-vsl-layout-prisciane_v6.html |
| fcs-upsell-pg01-of01 | 2026-10-29_pagina-upsell-vsl-layout-prisciane_v3.html |
| fcs-downsell-pg01-of01 | 2026-11-05_pagina-downsell-vsl-layout-prisciane_v4.html |
| fcs-obrigado-entrada-pg01-of01 | 2026-10-29_pagina-obrigado-entrada-vsl-base-v3_v1.html |
| fcs-obrigado-upsell-pg01-of01 | 2026-10-29_pagina-obrigado-upsell-vsl-base-v3_v1.html |
| fcs-obrigado-downsell-pg01-of01 | 2026-10-29_pagina-obrigado-downsell-vsl-base-v3_v1.html |

## O que foi alterado em relação às páginas aprovadas
- GTM-NXXH6G42 (head e noscript) nas 3 páginas.
- Embeds oficiais da Vturb (player no lugar do placeholder + preloads no head): VSL_ENTRADA_OUT26, VSL_UPSELL_OUT26-1, VSL_DOWNSELL_OUT26.
- Upsell e downsell: botão "Quero ser VIP" trocado pelo iframe oficial de 1 clique (365453 e 818936).
- Entrada: 3 CTAs com link 6LiYmi, agora com data-fcs-acao="comprar" (convenção das páginas de teste).
- Removido material interno: faixa "RASCUNHO", caixas de pendência, lista de pendências, caixa de notas e botão "Notas", painel de teste.
- Títulos limpos (sem "Rascunho" e "layout Prisciane"). noindex mantido.
- Entrada: 18 imagens saíram do HTML (2,3 MB) e foram convertidas para WebP na subpasta img/. HTML 61 KB + imagens 905 KB (antes 1,7 MB).
- Entrada: liberação por pitch. O botão de compra do topo e todo o conteúdo entre o player e o rodapé estão com class `liberar-pitch` e `display:none`. Rodapé, aviso de cookies e WhatsApp ficam sempre visíveis. Upsell e downsell ficam sempre visíveis.
- Obrigados (3): GTM nas 3, removidos a faixa "RASCUNHO LOCAL", a caixa de notas internas e o botão "Notas"; títulos sem "(base v3)"; 2 imagens por página saíram do HTML (210 KB para 16 KB) e viraram WebP em img/. Sem botão de venda e sem data-fcs-acao, como na regra original.
- Texto e copy das páginas não foram alterados.

## ANTES DE PUBLICAR
[FEITO por Danilo em 05/11] No player de ENTRADA da Vturb (id vid-6ae0ad22c7321bec2b3b7ec6), criar o botão de ação "Mostrar conteúdo oculto" com Class `liberar-pitch`, no tempo do pitch, marcando "Definir como tempo do pitch" e "Manter exibição em visitas futuras" (mesma configuração validada em 12/10 no player de teste). Sem esse botão, a página de entrada fica mostrando só título, vídeo e rodapé, e ninguém consegue comprar.


## Como subir
Copie as 6 pastas (fcs-*-pg01-of01) para a raiz do repositório remuneracaoemfoco/cargosesalarios, substituindo as de teste de mesmo nome, e faça um commit só. Não mexer nas pastas pg99 nem no index.html da raiz.
