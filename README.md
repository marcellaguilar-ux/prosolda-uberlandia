# Prosolda — site (deploy estático)

Pasta pronta para publicar no **Vercel** (ou qualquer host estático: Netlify, Cloudflare Pages, GitHub Pages).

## Conteúdo
- `index.html` — o site
- `support.js`, `image-slot.js` — runtime/componentes (necessários)
- `media/operacao.mp4` — vídeo do hero
- `image-slots.state.json` — imagens dos produtos / fotos já inseridas
- `vercel.json` — configuração mínima

## Como publicar no Vercel

### Opção A — arrastar e soltar (mais simples)
1. Acesse https://vercel.com e faça login
2. Em **Add New → Project**, ou em https://vercel.com/new, arraste **esta pasta inteira**
3. Framework Preset: **Other** (é um site estático, sem build)
4. Clique em **Deploy**

### Opção B — Vercel CLI
```bash
npm i -g vercel
cd deploy
vercel        # pré-visualização
vercel --prod # produção
```

## Observações
- Não renomeie `image-slots.state.json` — é onde ficam as imagens dos produtos e as fotos.
- Para trocar uma foto depois, basta substituir a imagem dentro do editor e reexportar a pasta.
- O vídeo do hero toca automaticamente, mudo e em loop.
