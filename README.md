# API REST SPRING BOOT e Kotlin

API para Sistema de Avaliação de Créditos para uma empresa de emprestimo, com analise de solicitação de crédito.

Com as seguintes funcionalidades:

## Cliente (Customer):
### Cadastrar:
Request: firstName, lastName, cpf, income, email, password, zipCode e street
Response: String

### Editar cadastro:
Request: id, firstName, lastName, income, zipCode, street
Response: firstName, lastName, income, cpf, email, income, zipCode, street

### Visualizar perfil:
Request: id
Response: firstName, lastName, income, cpf, email, income, zipCode, street

### Deletar cadastro:
Request: id
Response: sem retorno


## Solicitação de Empréstimo (Credit):

### Cadastrar:
Request: creditValue, dayFirstOfInstallment, numberOfInstallments e customerId
Response: String

### Listar todas as solicitações de emprestimo de um cliente:
Request: customerId
Response: creditCode, creditValue, numberOfInstallment

### Visualizar um emprestimo:
Request: customerId e creditCode
Response: creditCode, creditValue, numberOfInstallment, status, emailCustomer e incomeCustomer

Esse projeto foi criado com finalidade de desenvolver e aprender as funcionalidades do kotlin e spring boot.

