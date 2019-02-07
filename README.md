## O que preciso fazer?
Vamos ser práticos e diretos, se você quer trabalhar conosco siga os passos abaixo:
*	Implemente o desafio descrito no tópico abaixo.
*	Faça um push para seu repositório com o desafio implementado.
*	Envie um email para (trabalheaqui@tstech.com.br) avisando que finalizou o desafio com a url do seu fork.
*	Aguarde nosso contato.

## O Desafio de Loja de Carro
Você deverá criar 2 aplicações para cadastramento de veículos a venda:
1. **Back-end:** aplicação .NET WEB-API.
2. **Front-end:** Single Page Application que se comunique com estes serviços (Angular ou React).
**Base de dados:** Fica a seu critério SQL SERVER, Memória, Redis, Mongo, Prostegres, MySql ou qualquer outro meio.

# Requisitos:
-	Permitir o cadastro de veículos.
-	Permitir listar todos os veículos.
-	Permitir alterar um veículo.
-	Permitir deletar um veículo.
-	Permitir o cadastro de propostas.
-	Permitir alterar uma proposta.
-	Permitir deletar uma proposta.
-	Permitir listar todas as propostas.
-	Permitir visualizar um veículo anunciado, ao acessar ele terá todas as informações de cadastro e as propostas relacionadas direcionada a ele.
-	Permitir marcar o veículo como VENDIDO


O cadastro do veículo da aplicação deve conter as seguintes informações:
-	Marca (string)
-	Modelo (string)
-	Ano (int)
-	Preço (int)
-	Vendido (boolean | 0 = À venda | 1 = Vendido)

As propostas devem contém as seguintes informações:
-	Data da proposta (string)
-	Veículo (int ou String)
-	Valor (Decimal)
-	Nome do cliente (String)
Uma proposta só pode ser associada a um veículo cadastrado e não vendido. 
Devido ao prazo, falamos para nosso cliente que não conseguiríamos colocar fotos do carro. Mas, caso consiga finalizar antes do prazo e conseguir disponibilizar imagens do carro, seria bem legal!

## API endpoints
GET /veiculos - Retorna todos os veículos

GET /veiculos/{id} - Retorna os detalhes do veículo (assim como as propostas associadas a ele)

POST /veiculos - Adiciona um novo veículo

PUT /veiculos/{id} - Atualiza os dados de um veículo

PATCH /veiculos/{id} - Atualiza status de venda de um veículo.

DELETE /veiculos/{id} -Apaga o veículo

GET /propostas - Retorna todos as propostas

GET /propostas/{id} - Retorna os detalhes da proposta e do veículo 

POST /propostas - Adiciona uma nova proposta

PUT /propostas/{id} - Atualiza os dados de uma proposta

DELETE /propostas/{id} - Apaga a proposta

## Recomendações gerais:
*	A modelagem dos dados fica a seu critério 
*	Não se preocupe com autenticação ou multitenancy.

## Avaliação
Entre os critérios de avaliação estão:
*	Performance
*	Código limpo e organização
*	Boas práticas de desenvolvimento

### Bonus
Se você fosse utilizar esse sistema comercialmente, que alterações você faria para escalar e/ou facilitar a vida do usuário? (Não é necessário implementar!).
