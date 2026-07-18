# Modelo de Dados - Veículos JORM

## Objetivo

Definir a estrutura principal de cadastro e controle dos veículos dentro do ERP JORM.

O veículo será o registro central do sistema, acompanhando todo seu ciclo: compra, preparação, venda e resultado financeiro.

---

# Cadastro do Veículo

## Identificação

- ID do veículo
- Placa
- Renavam
- Chassi
- Marca
- Modelo
- Versão
- Ano de fabricação
- Ano modelo
- Quilometragem
- Cor
- Combustível

---

# Processo de Compra

## Dados da Aquisição

- Data da compra
- Fornecedor / vendedor
- CPF/CNPJ do fornecedor
- Valor pago
- Forma de pagamento
- Observações da compra

---

# Custos do Veículo

## Preparação e Despesas

- Mecânica
- Funilaria
- Pintura
- Higienização
- Documentação
- Taxas
- Despesas diversas

O sistema deverá calcular automaticamente:

Valor de compra + custos = custo total do veículo

---

# Processo de Venda

## Dados da Venda

- Data da venda
- Cliente
- CPF/CNPJ do cliente
- Valor vendido
- Forma de pagamento
- Comissão
- Observações

---

# Resultado Financeiro

O sistema deverá calcular:

Valor vendido - custo total = margem do veículo

Informações:

- Custo total
- Valor de venda
- Lucro bruto
- Margem percentual

---

# Status do Veículo

Fluxo operacional:

1. Em avaliação
2. Comprado
3. Em preparação
4. Disponível para venda
5. Vendido

---

# Histórico

O sistema deverá manter histórico de:

- Alterações de cadastro
- Mudanças de status
- Custos adicionados
- Propostas recebidas
- Venda realizada