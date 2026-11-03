# Protocolo de Diagnóstico de Erros
## Coletar
Comportamento esperado/real, mensagem completa, passos para reproduzir, tecnologia/versões, arquivo relacionado e mudanças recentes. Remover segredos de logs e capturas.

## Método
1. Reproduzir.
2. Identificar camada: interface, rede, backend, banco, configuração ou terceiro.
3. Formular uma hipótese por vez.
4. Fazer uma alteração pequena.
5. Repetir o teste original.
6. Verificar efeitos colaterais.
7. Registrar causa e prevenção.

Não executar comandos destrutivos nem apagar dados sem backup e confirmação. Não declarar resolvido sem validar.
