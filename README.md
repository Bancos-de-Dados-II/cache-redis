# api-express-sequelize

Exemplo de API REST, com express e sequelize apresentado na disciplina de Bancos de Dados II, do Curso Superior de Tecnologia em Análise e Desenvolvimento de Sistemas, do IFPB/campus Cajazeiras. A API utiliza o redis como cache nos métodos de busca por e-mail com base na técnica de Lazy Load. Convém reforçar que o exemplo foi construído para ser didático, e pode/deve ser refatorado.

## Inicialização
Para inicializar a API vocês deverão:
1. Clonar o repositório
2. Criar na pasta raiz um arquivo .env, que apresenta os parâmetros de configuração do banco

Exemplo do arquivo .env (trocar os valores das chaves pelos dados do seu banco):
```
PG_HOST = localhost
PG_PORT = 5432
PG_USERNAME = postgres
PG_PASSWORD = postgres
PG_DATABASE = teste
API_PORT = 3000
REDIS_HOST = {host do redis cloud}
REDIS_PORT = {porta do redis cloud}
REDIS_USER = {usuário, padrão: default}
REDIS_PASSWORD = {senha do usuário}
```

3. ```npm i```
4. ```npm start```

## Alterar parâmetros
Você deve alerar os dados da conexão do banco e da porta da API no arquivo .env para os dados do seu usuário. **Não esqueça de nunca deixar essas informações públicas, uma vez que esses dados podem ser utilizados por terceiros.**

## Uso
Todos os comandos do uso do banco estão no arquivo index.js. É necessário realizar refatoração do código, pois foi feito de forma simples para facilitar na didática do exemplo.
