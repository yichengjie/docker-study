docker学习资料：https://www.docker.tips

### wins安装docker

1. https://www.runoob.com/docker/windows-docker-install.html

### linux安装docker

1. 访问https://get.docker.com 下载脚本为get-docker.sh

   ```
   curl -fsSL get.docker.com -o get-docker.sh
   ```

2. 执行命令```sh get-docker.sh```

3. 验证docker安装完成， 输入名```docker version```看输出结果

4. 步骤3中如果报docker server没有启动，可以通过命令```sudo systemctl start docker```启动

5. 注意docker的命令如果不是root用户都需要加sudo

6. 直接执行get-docker.sh过程中可能会有些因为网路原因报错，手动执行安装依赖即可

   ```yum -y  install deltarpm 
   例如：yum -y  install deltarpm 
   ```

### docker常用命令

1. docker exec -it   ${id}   sh

2. 启动mysql： ```docker run -d -p 3307:3306 -e MYSQL_ROOT_PASSWORD=123456 mysql```

   ```
   https://www.cnblogs.com/sablier/p/11605606.html
   ```

3. 清空所有停用的镜像
    ```text
    docker system prune -f
    ```
4. 运行并自动删除镜像
    ```text
    docker container run --rm -it gcc-demo-new yicj
    ```
### docker使用技巧
1. 合理使用cache（尽量将变化的东西放到后面）
2. 编写.dockerignore文件忽略文件
3. 多阶段构建
4. 尽量使用非root用户

### 学习资料
1. 官网dockerfile学习：https://docs.docker.com/engine/reference/builder/
2. github上docker-library/official-images

### 其他
1. 更新wsl： https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi下载安装
2. 安装zsh：sudo apt-get install zsh

