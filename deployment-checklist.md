# 🚀 Checklist de Deploy Padrão

## ✅ ANTES DO DEPLOY
- [ ] UTMify configurado com captura agressiva
- [ ] Webhook robusto implementado
- [ ] Sistema de recuperação ativo
- [ ] Logs detalhados funcionando
- [ ] Testes de integração passando

## 🔧 DEPLOY BACKEND (Railway)
```bash
railway up
```
- Sempre verificar se webhook está funcionando
- Testar rota `/webhook/events`
- Verificar logs do Railway

## 🌐 DEPLOY FRONTEND (Vercel)
```bash
vercel --prod
```
- Sempre verificar se UTMify está carregando
- Testar captura de UTMs
- Verificar sistema de recuperação

## 🧪 TESTES PÓS-DEPLOY
- [ ] Captura de UTMs funcionando
- [ ] Webhook disparando eventos
- [ ] Sistema de recuperação ativo
- [ ] Logs detalhados disponíveis
- [ ] Página de debug funcionando

## 🚨 EM CASO DE PROBLEMAS
1. Verificar logs do Railway
2. Verificar logs do Vercel
3. Usar página de debug
4. Forçar evento via webhook
5. Recuperar venda perdida

## 📊 MONITORAMENTO
- Sempre manter página de monitoramento ativa
- Verificar eventos UTMify diariamente
- Monitorar webhooks do gateway
- Backup automático de dados