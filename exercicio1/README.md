# Exercício 1: mongo:4.2 e mongo-express

## Parâmetro de execução de container (docker run)
```bash
docker run -d --name mongo -p 27017:27017 mongo:4.2
docker run -d --name mongo-express --link mongo:mongo -p 8081:8081 mongo-express
