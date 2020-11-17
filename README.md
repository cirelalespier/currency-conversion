# Conversor de moedas
Esse projeto tem o objetivo de realizar a conversão de moedas.

## Começando

Para executar o projeto, será necessário instalar os seguintes programas:

Git, Node e Visual Studio Code

## Desenvolvimento

Para iniciar o desenvolvimento, é necessário clonar o projeto do GitHub em um diretório de sua preferência:

cd diretórioDeSuaPreferência

git clone https://github.com/cirelalespier/currencyConversion

### Construção

Para baixar as dependências do projeto, executar o comando abaixo:

npm i

### Rodar aplicação

Para iniciar o projeto, executar o comando abaixo:

npm start

#### Listar moedas

Descrição: Endpoint que permite listar as moedas a serem convertidas.

**MÉTODO HTTP / RECURSO**

##### GET /

#### Converter moedas

Descrição: Endpoint que permite a conversão entre duas moedas.

**MÉTODO HTTP / RECURSO**

##### POST /

**REQUEST QUERY**

  from: { type: string, required: true },
  to: { type: string, required: true },
  amount: { type: number, required: true }

Exemplo:

  from: "USD",
  to: "BRL",
  amount: 123.0

#### ADICIONAR MOEDA

Descrição: Endpoint que permite a criação de uma moeda no banco de dados.

**MÉTODO HTTP / RECURSO**

##### PUT /

**REQUEST BODY**

    currency: { type: string, required: true }

Exemplo:

```json
{
  "currency": "ABC"
}
```

#### EXCLUIR MOEDA

Descrição: Endpoint que permite excluir uma moeda no banco de dados.

**MÉTODO HTTP / RECURSO**

##### DELETE /:id

**REQUEST PARAMs**

    id: { type: string, required: true }

### Rodar testes unitários da aplicação

Para iniciar os testes unitários do projeto, executar o comando abaixo:

npm test

# Licença

Não se aplica.

## Decisões de projeto

### Framework
Escolhi usar o Express.js como framework, por ser um framework leve, rápido e flexível que fornece recursos robustos para criar aplicações em Node.js.

### Banco de dados

Utilizei o banco de dados MongoDB com Mongoose, por se tratar de trocas de informações no projeto baseadas em chave a valor, e por necessitar de consultas rápidas e eficientes.

## Contato

Estou à disposição para dúvidas e sugestões!

** Cirela Lespier | lespier.cirela@gmail.com **
