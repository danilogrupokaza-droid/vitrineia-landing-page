# vitrineia-us-landing

Landing page da Fase 2 – Med Spa (inglês).

## Deploy no Vercel

1. Crie um novo repo no GitHub: `vitrineia-us-landing`
2. Suba os arquivos desta pasta
3. Acesse [vercel.com](https://vercel.com) → New Project → importe o repo
4. Deploy automático (static site, zero config)

## Antes de subir: atualize o `index.html`

Linha ~340 do `<script>`:

```js
const API_URL     = 'https://SEU_RAILWAY_URL/api/leads';
const BUSINESS_ID = '8308b000-eb0d-4ac4-a6ad-1e3ca9399936';
```

Substitua `SEU_RAILWAY_URL` pela URL do serviço Railway após o deploy da API.

## O que está incluído

- Design luxury / med spa com tipografia Cormorant Garamond
- Formulário com validação client-side completa
- Consentimento TCPA (SMS + email) – obrigatório nos EUA
- Captura de UTM params (utm_source, utm_medium, utm_campaign)
- Detecção automática de fonte por referrer (Instagram, Google, etc.)
- Formatação automática de telefone US → E.164
- Estado de loading e sucesso
- Layout responsivo (mobile-first)
- Headers de segurança via vercel.json
