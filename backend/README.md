# Backend ERP Veículos JORM

## Objetivo

Responsável pelas regras de negócio, API e integração com banco de dados do ERP JORM.

---

# Estrutura

## Controllers

Responsáveis por receber as solicitações do sistema.

Exemplos:
- Cadastro de veículos
- Clientes
- Vendas
- Financeiro

---

## Models

Representam as entidades do sistema.

Exemplos:

- Veiculo
- Cliente
- Compra
- Venda
- Usuario

---

## Routes

Definem os caminhos de acesso da API.

Exemplos:

GET /veiculos

POST /veiculos

PUT /veiculos/:id

DELETE /veiculos/:id

---

## Services

Contém as regras de negócio.

Exemplos:

- Cálculo de margem
- Atualização de estoque
- Controle financeiro

---

# Primeiro módulo

Cadastro de Veículos:

Funções:

- Criar veículo
- Consultar veículos
- Alterar dados
- Alterar status
- Registrar custos
- Calcular margem