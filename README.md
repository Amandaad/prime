# Prime · Sistema de vendas e estoque

Aplicação web em PHP 8+ e MySQL para cadastro de produtos e clientes, vendas com baixa automática do estoque e relatórios de operação.

## Como iniciar

1. Crie um banco MySQL e importe `schema.sql` (por exemplo, `mysql -u root -p < schema.sql`).
2. Configure o acesso no `config.php` ou defina as variáveis `DB_HOST`, `DB_PORT`, `DB_NAME`, `DB_USER` e `DB_PASS`.
3. Inicie o servidor local na pasta do projeto: `php -S localhost:8000`.
4. Acesse `http://localhost:8000`.

O PHP precisa das extensões PDO e PDO MySQL. Em produção, defina as credenciais por variáveis de ambiente e sirva a aplicação por um servidor web com HTTPS.

## Funcionalidades

- Cadastro e pesquisa de produtos, categoria, SKU, preço e níveis de estoque.
- Cadastro e pesquisa de clientes.
- Registro de vendas com múltiplos itens, validação de disponibilidade e atualização transacional do estoque.
- Painel com vendas do dia, alertas de reposição e vendas recentes.
- Relatórios de faturamento, ticket médio, produtos mais vendidos e valor em estoque.
