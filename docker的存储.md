1. 列表volume ```docker volume ls```
2. 查看volume详情 ```docker volume inspect mysql-data```
3. docker container run --name some-mysql -e MYSQL_ROOT_PASSWORD=my-secret-pw -d -v mysql-data:/var/lib/mysql mysql:5.7
4. es安装插件
    ```
    docker cp D:\tools\elk\elasticsearch-analysis-ik-7.6.2.zip 3cff7d7e661a:/usr/share/elasticsearch
    ./bin/elasticsearch-plugin install file:////usr/share/elasticsearch/elasticsearch-analysis-ik-7.6.2.zip
    ```
