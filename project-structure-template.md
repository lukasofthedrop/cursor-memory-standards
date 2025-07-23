# 📁 Estrutura de Projeto Padrão

## Frontend (Vercel)
```
noticia/
├── js/
│   ├── utmify-setup.js          # Configuração UTMify
│   ├── aureolink-pix-generator.js
│   └── utmify-config.js
├── index.html                   # Landing principal
├── finalizacao.html            # Checkout
├── recover-specific-sale.html  # Recuperação
└── monitor-funil.html          # Monitoramento
```

## Backend (Railway)
```
src/
├── index.js                     # Webhooks + APIs
├── package.json
└── railway.json
```

## Configurações
```
├── vercel.json                  # Deploy frontend
├── railway.json                 # Deploy backend
└── package.json                 # Dependências
```

## 🚨 Arquivos Críticos
- `noticia/js/utmify-setup.js` - SEMPRE implementar captura agressiva
- `src/index.js` - SEMPRE implementar webhook robusto
- `recover-specific-sale.html` - SEMPRE ter página de recuperação