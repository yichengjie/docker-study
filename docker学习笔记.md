1. docker学习资料：https://www.docker.tips

### linux安装docker

1. 访问https://get.docker.com 下载脚本为get-docker.sh

   ```
   curl -fsSL get.docker.com -o get-docker.sh
   ```

2. 执行命令```sh get-docker.sh```

3. 验证docker安装完成， 输入名```docker version```看输出结果

4. 步骤3中如果报docker server没有启动，可以通过命令```sudo systemctl start docker```启动

5. 注意docker的命令如果不是root用户都需要加sudo