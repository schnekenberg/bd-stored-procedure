--- Projeto: Stored Procedures ---

Este repositório contém a implementação de 10 exercícios práticos de Stored Procedures utilizando PostgreSQL (PL/pgSQL), desenvolvidos em ambiente de laboratório com Google Colab integrado ao banco de dados na nuvem via Neon.

--- Objetivos ---
Aplicar conceitos avançados de banco de dados, com foco em:
- Criação e uso de Stored Procedures
- Manipulação de dados com PL/pgSQL
- Implementação de regras de negócio no banco
- Uso de transações e tratamento de erros
- Automação com jobs agendados (pg_cron)

--- Tecnologias utilizadas ---
- PostgreSQL (PL/pgSQL)
- Neon (PostgreSQL Serverless)
- Google Colab
- Python (psycopg2 para conexão)
- pg_cron (agendamento de tarefas)

--- Modelagem do Banco ---
O banco simula um sistema de e-commerce com as seguintes tabelas:
- customers
- products
- orders
- order_items
- audit_logs

--- Como Executar ---
I) Crie um banco de dados PostgreSQL na plataforma Neon.
II) Abra o notebook do projeto no Google Colab.
III) Configure a string de conexão/credenciais do Neon no notebook.
IV) Execute as células para:
- conectar ao banco de dados
- executar os scripts SQL (schema + procedures/functions)
- executar as queries dos exercícios

--- Principais Conceitos Aplicados ---
- Procedures com parâmetros IN e OUT
- Controle transacional (BEGIN, COMMIT, ROLLBACK)
- Tratamento de exceções (EXCEPTION)
- Logging com RAISE NOTICE e tabela de auditoria
- Automação com CRON no PostgreSQL

--- Benefícios do Uso de Stored Procedures ---
- Melhor performance (execução pré-compilada)
- Redução de tráfego entre aplicação e banco
- Centralização da lógica de negócio
- Maior segurança e controle de acesso
- Reutilização de código

--- Observações ---
- Todos os testes foram realizados no ambiente Google Colab
- O banco de dados foi hospedado na plataforma Neon
- Scripts podem ser adaptados para execução local
