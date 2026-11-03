# SQL e PostgreSQL
## Conceitos
Tabela, coluna, chave primária, chave estrangeira, constraints, índices e transações.

```sql
CREATE TABLE clientes (
  id bigint GENERATED ALWAYS AS IDENTITY PRIMARY KEY,
  nome text NOT NULL,
  email text UNIQUE,
  criado_em timestamptz NOT NULL DEFAULT now()
);

INSERT INTO clientes (nome, email)
VALUES ('Cliente Exemplo', 'cliente@example.com');

SELECT id, nome, email FROM clientes ORDER BY criado_em DESC;
```

## Cuidados
Conferir `WHERE` em UPDATE/DELETE, usar constraints, escolher tipos adequados, parametrizar consultas, criar índices conforme consultas reais e testar backups/restauração. Modelar entidades e relações antes de criar tabelas.
