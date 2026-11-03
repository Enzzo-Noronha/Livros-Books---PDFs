# Segurança Web — Regras Práticas

## Segredos
- Nunca incluir senhas, tokens, chaves privadas ou credenciais em código versionado.
- Usar variáveis de ambiente e serviços apropriados de gerenciamento de segredos.
- Se um segredo for exposto, revogá-lo e gerar outro; apagar o texto do arquivo não é suficiente.

## Autenticação e autorização
- Autenticação responde quem é o usuário; autorização define o que ele pode fazer.
- Verificar permissões no servidor em cada operação protegida.
- Não confiar em botões ocultos ou verificações feitas apenas no frontend.
- Usar mecanismos de autenticação reconhecidos e armazenar senhas com algoritmos apropriados, nunca em texto puro.

## Dados e entradas
- Validar formato, tamanho e conteúdo das entradas.
- Usar consultas parametrizadas para banco de dados.
- Codificar ou sanitizar conteúdo de acordo com o contexto de exibição.
- Coletar somente os dados necessários.
- Definir retenção, exclusão e acesso aos dados.

## SaaS multiusuário
- Garantir isolamento de dados entre empresas/contas.
- Testar se um usuário consegue acessar registros de outro.
- Aplicar políticas de acesso no backend e no banco de dados.
- Não confiar apenas em um identificador enviado pelo navegador.

## Operação
- Manter dependências atualizadas.
- Registrar eventos relevantes sem guardar segredos.
- Fazer backups e testar restauração.
- Planejar atualizações e resposta a incidentes.
- Consultar a documentação oficial e os requisitos legais aplicáveis ao projeto.

## Limite
Este documento é uma lista inicial, não substitui auditoria de segurança ou aconselhamento jurídico.
