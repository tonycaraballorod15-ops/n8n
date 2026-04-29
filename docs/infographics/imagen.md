# Imagen de la plataforma (TCR Salsa)

La imagen está en este archivo:

- `docs/infographics/tcr-salsa-platform-flow.svg`

## Cómo verla rápido

1. Abre `docs/infographics/tcr-salsa-platform-flow.svg` directamente en tu navegador.
2. O abre este markdown (`docs/infographics/imagen.md`) en GitHub/VS Code para verla embebida.

![Imagen de estructura de plataforma](./tcr-salsa-platform-flow.svg)

## Orden importante de nodos

1. Webhook Create Post (`Webhook_CreatePost`)
2. Normalize Input (`Code_NormalizeInput`)
3. Is Scheduled (`If_Scheduled`)
4. Wait Until Publish (`Wait_UntilPublish`) si es programado
5. Post Facebook (`HTTP_Facebook`)
6. Post Instagram (`HTTP_Instagram`)
7. Post TikTok (`HTTP_TikTok`)
8. Merge Results (`Merge_Results`)
9. Respond Webhook (`Respond_Webhook`)
