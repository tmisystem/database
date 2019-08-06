# Database TMS | Souagro Soluções

## Filiais

Tabela contendo todas as filias da empresa.

| campo             | tipo               | descrição                             | Obrigatório |
|-------------------|--------------------|---------------------------------------|-------------|
| code              | number,string      | Identificador único da filial         | sim         |
| name              | string             | Nome                                  | sim         |
| name_f            | string             | Nome fantasia                         | não         |
| cnpj              | string             | CNPJ                                  | sim         |
| ie                | string             | Inscrição estadual                    | não         |
| address_zipcode   | string             | CEP do endereço                       | não         |
| address_street    | string             | Rua do endereço                       | não         |
| address_number    | string             | Número do endereço                    | não         |
| address_district  | string             | Bairro do endereço                    | não         |
| address_city_code | string             | Código IBGE da cidade                 | sim         |
| address_city      | string             | Nome da cidade                        | sim         |
| address_state     | string             | Estado                                | sim         |
| phone             | string             | Telefone                              | não         |
| last_update       | timestamp,datetime | Data e hora da última atualização     | sim         |

## Locais de retirada

Tabela contendo todas os locais de retirada de produtos da empresa.

| campo             | tipo               | descrição                             | Obrigatório |
|-------------------|--------------------|---------------------------------------|-------------|
| code              | number,string      | Identificador único da filial         | sim         |
| name              | string             | Nome                                  | sim         |
| name_f            | string             | Nome fantasia                         | não         |
| cnpj              | string             | CNPJ                                  | sim         |
| ie                | string             | Inscrição estadual                    | não         |
| address_zipcode   | string             | CEP do endereço                       | não         |
| address_street    | string             | Rua do endereço                       | não         |
| address_number    | string             | Número do endereço                    | não         |
| address_district  | string             | Bairro do endereço                    | não         |
| address_city_code | string             | Código IBGE da cidade                 | sim         |
| address_city      | string             | Nome da cidade                        | sim         |
| address_state     | string             | Estado                                | sim         |
| phone             | string             | Telefone                              | não         |
| last_update       | timestamp,datetime | Data e hora da última atualização     | sim         |

## Fornecedores

Tabela contendo todos os fornecedores da empresa.

| campo             | tipo               | descrição                                | Obrigatório |
|-------------------|--------------------|------------------------------------------|-------------|
| code              | number,string      | Identificador único do fornecedor        | sim         |
| type              | string             | F (Física) ou J (Jurídica)               | sim         |
| name              | string             | Nome social                              | sim         |
| name_f            | string             | Nome fantasia                            | não         |
| cpf_cnpj          | string             | CPF ou CNPJ                              | sim         |
| ie                | string             | Inscrição estadual                       | não         |
| address_zipcode   | string             | CEP do endereço                          | não         |
| address_street    | string             | Rua do endereço                          | não         |
| address_number    | string             | Número do endereço                       | não         |
| address_district  | string             | Bairro do endereço                       | não         |
| address_city_code | string             | Código IBGE da cidade                    | sim         |
| address_city      | string             | Nome da cidade                           | sim         |
| address_state     | string             | Estado UF (i.e., GO, RJ, SP, etc)        | sim         |
| phone_1           | string             | Telefone 1                               | não         |
| phone_2           | string             | Telefone 2                               | não         |
| phone_3           | string             | Telefone 3                               | não         |
| email             | string             | Email                                    | não         |
| status            | string             | Status (e.g., habilitado, desabilitado)  | sim         |
| description       | string             | Descrição do fornecedor                  | não         |
| last_update       | timestamp,datetime | Data e hora da última atualização        | sim         |

## Clientes

Tabela contendo todos os clientes da empresa.

| campo             | tipo               | descrição                                | Obrigatório |
|-------------------|--------------------|------------------------------------------|-------------|
| code              | number,string      | Identificador único do cliente           | sim         |
| type              | string             | F (Física) ou J (Jurídica)               | sim         |
| name              | string             | Nome social                              | sim         |
| name_f            | string             | Nome fantasia                            | não         |
| gender            | string             | Sexo, M (masculino) ou F (feminino)      | não         |
| cpf_cnpj          | string             | CPF ou CNPJ                              | sim         |
| ie                | string             | Inscrição estadual                       | não         |
| address_zipcode   | string             | CEP do endereço                          | não         |
| address_street    | string             | Rua do endereço                          | não         |
| address_number    | string             | Número do endereço                       | não         |
| address_district  | string             | Bairro do endereço                       | não         |
| address_city_code | string             | Código IBGE da cidade                    | sim         |
| address_city      | string             | Nome da cidade                           | sim         |
| address_state     | string             | Estado UF (i.e., GO, RJ, SP, etc)        | sim         |
| phone_1           | string             | Telefone 1                               | não         |
| phone_2           | string             | Telefone 2                               | não         |
| phone_3           | string             | Telefone 3                               | não         |
| email             | string             | Email                                    | não         |
| status            | string             | Status (e.g., habilitado, desabilitado)  | sim         |
| description       | string             | Descrição do cliente                     | não         |
| last_update       | timestamp,datetime | Data e hora da última atualização        | sim         |

## Produtos

Tabela contendo todos os produtos da empresa.

| campo                 | tipo                | descrição                                            | Obrigatório |
|-----------------------|---------------------|------------------------------------------------------|-------------|
| code                  | number, string      | Identificador único do produto                       | sim         |
| name                  | string              | Nome do produto                                      | sim         |
| unit                  | string              | Unidade de medida (e.g., saco (sc), quilograma (kg)) | sim         |
| amount                | number              | Quantidade no rótulo                                 | não         |
| packing               | string              | Tipo de empacotamento (e.g., SACO)                   | não         |
| packing_desc          | string              | Descrição do pacote                                  | não         |
| manufacturer          | string              | Nome do fabricante                                   | não         |
| density               | string              | Densidade do produto                                 | não         |
| group_product_code    | number, string      | Código do grupo                                      | sim         |
| group_product_name    | string              | Nome do grupo (e.g., sementes, fertilizantes)        | sim         |
| subgroup_product_code | number, string      | Código do subgrupo                                   | não         |
| subgroup_product_name | string              | Nome do subgrupo (e.g., granulados, micronutrientes) | não         |
| group_product_detail  | string              | Detalhe do gruo (e.g., micronutrientes)              | não         |
| supplier_code         | number, string      | Código do fornecedor                                 | sim         |
| supplier_name         | string              | Nome do fornecedor                                   | não         |
| status                | string              | Status do produto (e.g, ativo, destivado, etc)       | sim         |
| conversion_unit       | string              | Unidade de conversão (e.g., quilo, grama)            | não         |
| conversion_factor     | number              | Fator de conversão                                   | não         |
| last_update           | timestamp, datetime | Data e hora da última atualização na tablea          | sim         |

## Pedidos

Tabela contendo todos os pedidos, seus respectivos produtos e a quantidade selecionada de cada produto.

| campo                    | tipo                | descrição                                                                    | Obrigatório |
|--------------------------|---------------------|------------------------------------------------------------------------------|-------------|
| code                     | number, string      | Identificador único o pedido de venda                                        | sim         |
| harvest                  | string              | Label da colheira (e.g., safra/2019, soja/2019, milho/2019)                  | sim         |
| status                   | number              | Status do pedido (e.g., liberado, processando, ativo, cancelado)             | sim         |
| cost                     | number              | Custo total do pedido                                                        | não         |
| unit_cost                | number              | Custo unitário de cada produto do pedido                                     | não         |
| currency                 | string              | Moeda (e.g., real ou dolar)                                                  | não         |
| branch_code              | number, string      | Indentificador único da filial                                               | não         |
| branch_name              | string              | Nome da filial                                                               | não         |
| seller_code              | number, string      | Identificador único do vendedor do pedido                                    | sim         |
| seller_name              | string              | Nome do vendedor do pedido                                                   | sim         |
| regional_code            | string              | Identificador único da regional do pedido                                    | sim         |
| regional_name            | number, string      | Nome da regional do pedido                                                   | sim         |
| client_code              | number, string      | Identificador único do cliente                                               | sim         |
| client_name              | string              | Nome do cliente                                                              | não         |
| product_code             | number, string      | Identificador único do produto                                               | sim         |
| product_amount           | number              | Quantidade do produto no pedido                                              | sim         |
| product_amount_converted | timestamp, datetime | Quantidade do produto convertida em KG para limitar a capacidade do caminhão | sim         |
| product_unit             | string              | Unidade do produto (e.g., saco, kg)                                          | não         |
| product_unit_amount      | number              | Quantidade unitária descrita no rótulo do produto                            | não         |
| product_density          | string              | Densidade do produto                                                         | não         |
| freight_type             | string              | Tipo de frete (e.g, fob, cif)                                                | sim         |
| conversion_unit          | string              | Unidade de conversão (e.g., quilo, grama)                                    | não         |
| conversion_factor        | number              | Fator de conversão                                                           | não         |
| address_city_code        | number              | Código IBGE da cidade                                                        | sim         |
| address_city             | string              | Nome da cidade                                                               | sim         |
| address_state            | string              | Estado UF (i.e., GO, RJ, SP, etc)                                            | sim         |
| group_product_code       | number              | Código do grupo                                                              | não         |
| group_product_name       | number              | Nome do grupo                                                                | não         |
| subgroup_product_code    | number              | Código do subgrupo                                                           | não         |
| subgroup_product_name    | string              | Nome do subgrupo (e.g., granulados, micronutrientes)                         | não         |
| group_product_detail     | sring               | Detalhe do gruo (e.g., micronutrientes)                                      | não         |
| last_update              | timestamp, datetime | Data e hora da última atualização na tablea                                  | sim         |

### Pedidos com previsão de entrega de cada produto

Tabela contendo a quantidade que deve ser entrege de cada produto do pedido e que deve ser entrega em uma determinada data.

Caso a empresa não trabalhe com esse tipo de agendamento podemos considerar apenas a tabela de pedidos e a quantidade do produto do pedido.
Desta forma, ela irá perder a capacidade de filtrar os pedidos por data de agendamento.

| campo                    | tipo                | descrição                                                                    | Obrigatório |
|--------------------------|---------------------|------------------------------------------------------------------------------|-------------|
| code                     | number, string      | Identificador único para a previsão de entrega                               | sim         |
| order                    | number, string      | Identificador único o pedido de venda                                        | sim         |
| harvest                  | string              | Label da colheira (e.g., safra/2019, soja/2019, milho/2019)                  | sim         |
| status                   | number              | Status do pedido (e.g., liberado, processando, ativo, cancelado)             | sim         |
| cost                     | number              | Custo total do pedido                                                        | não         |
| unit_cost                | number              | Custo unitário de cada produto do pedido                                     | não         |
| currency                 | string              | Moeda (e.g., real ou dolar)                                                  | não         |
| branch_code              | number, string      | Indentificador único da filial                                               | não         |
| branch_name              | string              | Nome da filial                                                               | não         |
| seller_code              | number, string      | Identificador único do vendedor do pedido                                    | sim         |
| seller_name              | string              | Nome do vendedor do pedido                                                   | sim         |
| regional_code            | string              | Identificador único da regional do pedido                                    | sim         |
| regional_name            | number, string      | Nome da regional do pedido                                                   | sim         |
| client_code              | number, string      | Identificador único do cliente                                               | sim         |
| client_name              | string              | Nome do cliente                                                              | não         |
| product_code             | number, string      | Identificador único do produto                                               | sim         |
| product_amount           | number              | Quantidade do produto no pedido                                              | sim         |
| product_amount_converted | timestamp, datetime | Quantidade do produto convertida em KG para limitar a capacidade do caminhão | sim         |
| product_unit             | string              | Unidade do produto (e.g., saco, kg)                                          | não         |
| product_unit_amount      | number              | Quantidade unitária descrita no rótulo do produto                            | não         |
| product_density          | string              | Densidade do produto                                                         | não         |
| product_delivery_date    | timestamp, datetime | Data de previsão de entrega da quantidade agendada do produto                | sim         |
| product_selected         | number              | Quantidade selecionda do produto no pedido para entrega                      | sim         |
| freight_type             | string              | Tipo de frete (e.g, fob, cif)                                                | sim         |
| conversion_unit          | string              | Unidade de conversão (e.g., quilo, grama)                                    | não         |
| conversion_factor        | number              | Fator de conversão                                                           | não         |
| address_city_code        | number              | Código IBGE da cidade                                                        | sim         |
| address_city             | string              | Nome da cidade                                                               | sim         |
| address_state            | string              | Estado UF (i.e., GO, RJ, SP, etc)                                            | sim         |
| group_product_code       | number              | Código do grupo                                                              | não         |
| subgroup_product_code    | number              | Código do subgrupo                                                           | não         |
| subgroup_product_name    | string              | Nome do subgrupo (e.g., granulados, micronutrientes)                         | não         |
| group_product_detail     | sring               | Detalhe do gruo (e.g., micronutrientes)                                      | não         |
| last_update              | timestamp, datetime | Data e hora da última atualização na tablea                                  | sim         |


