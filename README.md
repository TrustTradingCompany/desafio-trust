# desafio-trust
Vaga Fullstack

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

Frontend

* Desenvolver as telas que façam o crud de cada entidade.


**O que irá destacar você**

* Uso de conteiners
* MongoDB

Terminado o projeto, publicar no seu github.