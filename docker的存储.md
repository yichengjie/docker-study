1. 列表volume ```docker volume ls```
2. 查看volume详情 ```docker volume inspect mysql-data```
3. docker container run --name some-mysql -e MYSQL_ROOT_PASSWORD=my-secret-pw -d -v mysql-data:/var/lib/mysql mysql:5.7
