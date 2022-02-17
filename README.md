# desafio-trust

## Etapas

### Backend

Desenvolver uma api usando Node.js que faça o crud de três entidades (cliente, produto e invoice e invoice itens).

As entidades possuem os seguintes campos:

Cliente

* ID (Auto incremento)
* Razão Social  (max: 50)
* Nome Fantasia (max: 50)
* CNPJ (max: 14)
* e-mail (max: 80)
* telefone (max: 12)

Produtos

* ID (Auto Incremento)
* NCM (Nomenclatura Comum do Mercosul) (max: 8)
* Descrição (max: 50)
* Ativo (boolean default true)

Invoice

* ID (Auto Incremento)
* Ordem de compra (varchar 30)
* Cliente (int - FK cliente)
* Data de Emissão (data - default data corrente)
* Previsão de chegada (data)

Invoice Itens

* ID (Auto incremento)
* Número da Invoice (int - fk invoice)
* Produto (int - fk produto)
* Quantidade (decimal)
* Valor unitário (decimal)
* Valor Total (decimal)

Usuários

* ID
* e-mail (max: 50)
* senha (possuir no minimo 8 caracteres contendo ao menos uma letra maiúscula, um número e um caracter especial).
* ativo (default true)
* ultimo_acesso


Desenvolver as rotas para realizar cada operação (criação, alteração e exclusão de entidades - no caso de exclusão utilizar soft deletes)
As rotas, com exceção de login, devem ser protegidas com autenticação.

As entidades devem possuir validação dos campos (e-mail válido, cnpj válido etc... )

## Frontend

Desenvolver as telas que façam o crud de cada entidade utilizando vue.

* Como usuário eu gostaria de me autenticar.
* Como usuário eu gostaria de poder cadastrar/alterar/excluir um cliente.
* Como usuário eu gostaria de poder cadastrar/alterar/excluir um produto.
* Como usuário eu gostaria de poder cadastrar/alterar/excluir uma invoice.
* Como usuário eu gostaria de poder cadastrar/alterar/excluir um produto da invoice.

**O que irá destacar você**

* Uso de conteiners.
* MongoDB.
* Padrões de Projeto.
* Testes unitários.

Terminado o projeto, publicar no seu github.