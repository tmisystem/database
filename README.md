# database

## Filiais
| campo             | tipo               | descrição                             | Obrigatório |
|-------------------|--------------------|---------------------------------------|-------------|
| code              | number,string      | Identificador da filial               | sim         |
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
| last_update       | timestamp,datetime | Última atualização do campo na tablea | sim         |
