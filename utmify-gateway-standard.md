# 🎯 PADRÃO UTMify + Gateway Integration - CNH Social

## 📋 Estrutura Padrão para Todos os Projetos

### 1. **Configuração UTMify Robusta**
```javascript
// noticia/js/utmify-setup.js
const YOUR_PIXEL_ID = '68789c1b0184c2e57bc706a6';
const YOUR_META_PIXEL_ID = '722536107338358';

// 7 fontes de captura de UTMs:
// 1. URL parameters
// 2. Referrer URL
// 3. localStorage
// 4. sessionStorage  
// 5. Cookies
// 6. Document referrer
// 7. History API
```

### 2. **Webhook Gateway Integration**
```javascript
// src/index.js - Webhook padrão
app.post('/aureolink/webhook', async (req, res) => {
  if (webhookData.status === 'paid' || webhookData.status === 'success') {
    // 3 métodos de disparo UTMify:
    // 1. UTMify API direta
    // 2. Facebook Pixel API
    // 3. Google Analytics 4 API
  }
});
```

### 3. **Sistema de Recuperação**
- Página `/recover-specific-sale.html` para vendas perdidas
- Rota `/webhook/force-purchase` para forçar eventos
- Rota `/webhook/events` para verificar eventos

### 4. **Deploy Structure**
- Frontend: Vercel (estático)
- Backend: Railway (webhooks)
- Sempre usar `railway up` + `vercel --prod`

### 5. **Pixel IDs Padrão**
- UTMify: 68789c1b0184c2e57bc706a6
- Facebook: 722536107338358
- Google Analytics: configurar por projeto

## 🚨 CRÍTICO - NUNCA PERDER VENDA
- Sempre implementar captura agressiva de UTMs
- Múltiplos fallbacks obrigatórios
- Sistema de recuperação automática
- Logs detalhados para debug