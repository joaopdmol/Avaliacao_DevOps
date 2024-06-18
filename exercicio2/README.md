# Exercício 2: mariadb e phpmyadmin

## Parâmetro de execução de container (docker run)
```bash
docker run -d --name mariadb -e MYSQL_ROOT_PASSWORD=root -p 3306:3306 mariadb
docker run -d --name phpmyadmin --link mariadb:db -p 8080:80 phpmyadmin/phpmyadmin
