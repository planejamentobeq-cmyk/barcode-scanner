# 📷 Leitor de Código de Barras

App web progressivo para leitura de códigos de barras via câmera, acumulando os resultados linha a linha.

## Funcionalidades

- Leitura em tempo real pela câmera traseira
- Suporte a múltiplos formatos: EAN-13, EAN-8, QR Code, Code 128, Code 39, UPC-A, UPC-E, ITF, Data Matrix e mais
- Resultados acumulados com timestamp
- Copiar código individual (clique no item)
- Copiar todos os códigos de uma vez
- Interface otimizada para mobile

## Como usar localmente

Basta abrir o `index.html` em um servidor local (necessário para acessar a câmera via HTTPS).

```bash
npx serve .
```

Ou com Python:

```bash
python3 -m http.server 8080
```

## Deploy na Vercel

1. Faça o fork ou clone deste repositório
2. Conecte o repositório na [Vercel](https://vercel.com)
3. Deploy automático — sem configuração adicional

O `vercel.json` já inclui os headers necessários para permissão de câmera.

## Tecnologias

- HTML/CSS/JS puro (sem build step)
- [@zxing/browser](https://github.com/zxing-js/browser) para decodificação de código de barras
- Deploy estático via Vercel
