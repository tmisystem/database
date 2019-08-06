# database

## Filiais
| campo             | tipo               | descrição                             | Obrigatório |
|-------------------|--------------------|---------------------------------------|-------------|
| code              | number|string      | Identificador da filial               | sim         |
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
| last_update       | timestamp|datetime | Última atualização do campo na tablea | sim         |

## Fornecedores
| campo             | tipo               | descrição                                | Obrigatório |
|-------------------|--------------------|------------------------------------------|-------------|
| code              | number|string      | Identificador da filial                  | sim         |
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
| last_update       | timestamp|datetime | Última atualização do campo na tablea    | sim         |


