# Exercício 3: postgres e dpage/pgadmin4

## Parâmetro de execução de container (docker run)
```bash
docker run -d --name postgres -e POSTGRES_PASSWORD=root -p 5432:5432 postgres
docker run -d --name pgadmin -e PGADMIN_DEFAULT_EMAIL=admin@admin.com -e PGADMIN_DEFAULT_PASSWORD=admin --link postgres:db -p 5050:80 dpage/pgadmin4
