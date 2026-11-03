# Arquitetura SaaS Multiempresa
Modelo conceitual: empresas (`organizations`), associação usuário-empresa (`memberships`) e tabelas de negócio com `organization_id`.

## Regras
Nunca confiar apenas no ID enviado pelo navegador. Verificar associação e papel, aplicar RLS quando apropriado, evitar segredos no frontend, planejar exportação/remoção de dados e registrar ações administrativas.

## Teste de isolamento
Criar Empresa A e B com usuários distintos. Confirmar que A não consegue ler nem alterar dados de B, para cada tabela e operação, inclusive sem autenticação.
