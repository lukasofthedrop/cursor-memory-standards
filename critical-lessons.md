# 🚨 LIÇÕES CRÍTICAS - CNH Social

## ❌ ERROS QUE CUSTARAM VENDAS
1. **UTMs NULL**: Sistema de captura fraco
2. **Gateway sem UTMify**: Webhook não disparava eventos
3. **Falta de fallbacks**: Sem backup quando falhavam

## ✅ SOLUÇÕES IMPLEMENTADAS
1. **Captura AGRESSIVA**: 7 fontes de UTMs
2. **Webhook ROBUSTO**: 3 métodos de disparo
3. **Sistema de RECUPERAÇÃO**: Páginas específicas
4. **Logs DETALHADOS**: Debug completo

## 🎯 PADRÕES OBRIGATÓRIOS
- Sempre implementar captura agressiva
- Múltiplos fallbacks obrigatórios
- Sistema de recuperação automática
- Testes de integração
- Monitoramento contínuo

## 📊 MÉTRICAS DE SUCESSO
- 0 vendas perdidas
- 100% tracking funcionando
- Recuperação automática
- Debug completo disponível

## 🔧 CÓDIGO CRÍTICO
```javascript
// SEMPRE implementar em todos os projetos:
// 1. Captura agressiva de UTMs (7 fontes)
// 2. Webhook robusto (3 métodos de disparo)
// 3. Sistema de recuperação
// 4. Logs detalhados
```