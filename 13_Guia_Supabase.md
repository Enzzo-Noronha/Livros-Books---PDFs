# Guia Prático do Supabase
## Componentes
- Database: PostgreSQL.
- Auth: identidade e autenticação.
- Storage: arquivos e políticas de acesso.
- Realtime: atualizações em tempo real.
- Edge Functions: lógica server-side e integrações.

## Fluxo recomendado
Modelar dados → criar tabelas e constraints → definir RLS → configurar Auth → conectar a aplicação → testar permissões → documentar alterações.

## Segurança
- Configurar RLS nas tabelas expostas ao cliente.
- Criar políticas explícitas para cada operação necessária.
- Nunca colocar `service_role` ou segredos no frontend.
- Não confiar em IDs enviados pelo navegador como prova de autorização.
- Testar acesso negado e isolamento entre usuários/empresas.

Documentação oficial: https://supabase.com/docs
Verificar a documentação atual antes de implementar APIs, limites ou padrões em produção.
