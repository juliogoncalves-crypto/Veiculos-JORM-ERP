# Estrutura do Banco de Dados - ERP JORM

## Objetivo

Definir as principais tabelas e relacionamentos do ERP Veículos JORM.

O banco de dados será responsável por armazenar todas as informações da operação.

---

# Tabela: VEICULOS

Cadastro principal dos veículos.

Campos:

- id_veiculo
- placa
- renavam
- chassi
- marca
- modelo
- versao
- ano_fabricacao
- ano_modelo
- cor
- combustivel
- quilometragem
- status
- data_cadastro

---

# Tabela: CLIENTES

Cadastro dos compradores.

Campos:

- id_cliente
- nome
- cpf_cnpj
- telefone
- email
- endereco
- cidade
- estado
- data_cadastro

---

# Tabela: COMPRAS

Registro das aquisições de veículos.

Campos:

- id_compra
- id_veiculo
- fornecedor
- data_compra
- valor_pago
- forma_pagamento
- observacao

---

# Tabela: CUSTOS_VEICULOS

Controle dos gastos de preparação.

Campos:

- id_custo
- id_veiculo
- tipo_custo
- descricao
- valor
- data_custo
- fornecedor

---

# Tabela: VENDAS

Registro das vendas realizadas.

Campos:

- id_venda
- id_veiculo
- id_cliente
- data_venda
- valor_venda
- forma_pagamento
- vendedor

---

# Tabela: USUARIOS

Controle de acesso ao sistema.

Campos:

- id_usuario
- nome
- email
- senha
- perfil
- ativo

---

# Relacionamentos

VEICULOS
|
├── COMPRAS
├── CUSTOS_VEICULOS
└── VENDAS

CLIENTES
|
└── VENDAS

USUARIOS
|
└── Operações do sistema