# database

## Filiais
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



