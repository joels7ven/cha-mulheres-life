# Chá das Mulheres Life — pacote para GitHub e Hostinger

Este pacote contém o código-fonte do site, sem credenciais do Mercado Pago, dependências instaladas ou arquivos internos de trabalho.

## Envio manual ao GitHub

1. Crie um repositório privado chamado `cha-mulheres-life` no GitHub.
2. Extraia este arquivo ZIP no computador.
3. No repositório, escolha **Add file → Upload files**.
4. Arraste o conteúdo extraído, mantendo as pastas `app`, `public`, `db`, `drizzle`, `worker` e `build`.
5. Use a mensagem `Versão inicial do site` e confirme em **Commit changes**.

## Importante sobre a Hostinger

O site possui checkout transparente, APIs, webhook e armazenamento de pedidos. Portanto, a versão completa não é um site puramente estático.

- A landing page visual pode ser convertida para hospedagem estática.
- O checkout não deve ser publicado como HTML estático, pois depende de código executado no servidor.
- O projeto atual usa Cloudflare Workers e D1 no backend.
- Antes de trocar o domínio para a Hostinger, o backend deve ser adaptado para Node.js e o banco migrado para MySQL ou Supabase.
- Nunca coloque a Public Key e o Access Token reais dentro dos arquivos ou do GitHub. Cadastre-os como variáveis de ambiente na Hostinger.

## Variáveis necessárias

```text
MERCADO_PAGO_PUBLIC_KEY
MERCADO_PAGO_ACCESS_TOKEN
```

O Access Token deve ser marcado como secreto.
