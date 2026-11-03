# Arquitetura Inicial de SaaS

## Componentes comuns
- Frontend: interface usada pelo cliente.
- Backend/API: regras de negócio e operações protegidas.
- Banco de dados: informações persistentes.
- Autenticação: identidade e sessão.
- Autorização: permissões por usuário, função e organização.
- Armazenamento: arquivos enviados, quando necessário.
- Monitoramento: erros, disponibilidade e uso.
- Cobrança: integração de pagamentos, se aplicável.

## Perguntas antes de escolher a arquitetura
1. Quantos usuários e organizações são esperados inicialmente?
2. Quais dados precisam ser armazenados?
3. Há dados sensíveis?
4. O sistema precisa funcionar offline?
5. Quais integrações externas são indispensáveis?
6. Quais são os custos fixos e variáveis?
7. Quem fará suporte e manutenção?

## MVP
Construir o menor conjunto de funcionalidades que valida o problema principal. Evitar adicionar cobrança automática, integrações complexas ou relatórios avançados antes de validar a necessidade, salvo se forem requisitos essenciais.

## Multiempresa
Se o produto atender várias empresas, definir claramente como os dados são separados. Toda leitura e escrita precisa respeitar a organização autenticada. Criar testes para impedir acesso cruzado.

## Operação
Planejar migrações do banco, backups, logs, recuperação de falhas, atualização de dependências e encerramento de contas.

## Decisões
Registrar tecnologia escolhida, motivo, alternativas consideradas, riscos e data. Não assumir que a mesma arquitetura serve para todos os produtos.
