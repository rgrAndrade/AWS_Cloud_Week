# AWS Cloud Week

BootCamp chat serverless na nuvem.

| :placard: Vitrine.Dev |     |
| -------------  | --- |
| :sparkles: Nome        | **AWS Cloud Week**
| :label: Tecnologias | AWS, AWS Lambda Functions, React, Amplify, DynamoDB,  Websocket API  (tecnologias utilizadas)
| :rocket: URL         | Em Desenvolvimento
| :fire: Desafio     | https://lp.dio.me/aws-cloud-week/

 ![af22d4a0-463f-48c5-a70c-4961d5e618d0](https://user-images.githubusercontent.com/104234513/222004997-b63de2d4-8a51-48f7-990e-13f00e14e618.png#vitrinedev)

## Detalhes do projeto

AWS Cloud Week, um projeto de 3 dias para construir uma aplicação de chat serverless na nuvem. Serão apenas alguns passos para construir uma aplicação de chat em tempo real!


# API para chat serverless integrado com API do OpenAI ChatGPT para a AWS Cloud Week

## Passos para o projeto

- Clonar o repositório
- Instalar as dependências com o comando ```npm install```
- Atualizar o arquivo ```.env``` com a sua chave do OpenAI
- Compactar o conteúdo do projeto em um arquivo ```.zip```

## Na AWS

- Acessar o console da AWS
- Criar uma função no serviço AWS Lambda
- Fazer o upload do conteúdo do arquivo ```.zip``` no código da função
- Acessar o serviço AWS API Gateway
- Criar uma API Websocket
- Criar os endpoints (obs: os três primeiros endpoints marcados com ```$``` são padrão de uma API Websocket do API Gateway):
    - ```$connect```
    - ```$disconnect```
    - ```$default```
    - ```setName```
    - ```sendPublic```
    - ```sendPrivate```
    - ```sendBot```

## Testando o Websocket

- Baixar a dependência ```wscat``` através do comando ```npm i -g wscat```. 
- Utilizar o parâmetro ```-g``` para instalar de forma global no sistema operacional, podendo chamá-la de fora do projeto.

### Utilizando o wscat

- ```wscat -c url_de_conexao_do_websocket```
- Exemplo de chamada ```{"action":"sendPublic", "message":"Hello World!"}```
