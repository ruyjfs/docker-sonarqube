# Sonar Docker
## Antes de rodar os comandos do docker é preciso configurar as variaveis de ambiente.
### Já tem algumas configurações pré definidas, com isso basta executar o comando abaixo:
#### Sonar 71
    cp example-71.env .env
#### Sonar 74
    cp example-71.env .env
## Depois de configurar as variáveis de ambiente basta rodar o docker-compose conforme cada ambiente.
### Rodar aplicação localmente
    docker-compose up --build
### Rodar aplicação em ambiente de desenvolvimento
    docker-compose -f docker-compose-dev.yml up --build -d
### Rodar aplicação em ambiente de produção
    docker-compose -f docker-compose-prod.yml up --build -d