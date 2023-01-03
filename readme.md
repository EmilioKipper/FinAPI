# FinAPI - Financeira

## Features

- Criar conta -> POST /account
- Buscar o extrato bancário do cliente -> GET /statement
- Realizar depósito -> POST /deposit
- Realizar saque -> POST /withdraw
- Buscar o extrato bancário do cliente por data -> GET /statement/date
- Atualizar dados da conta do cliente -> PUT /account
- Obter dados da conta do cliente -> GET /account
- Deletar conta -> DELETE /account
- Retornar o saldo -> GET /balance

## Regras de negócio

- Não cadastra uma conta com CPF já existente
- Não busca extrato de conta não existente
- Não faz depósito/saque em conta não existente
- Não faz saque quando saque for maior que o saldo
- Não pode excluir uma conta não existente

## Iniciando a aplicação

Para executar a aplicação é necessário ter instalado NodeJS e yarn/npm, e Insomnia para testes.

1. Clonar o repositório
2. Rodar no terminal o comando para instalar os pacotes: `yarn` ou `npm i`
3. Importar o arquivo collection.json para o Insomnia
