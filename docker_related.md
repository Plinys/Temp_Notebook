## Mysql 相关
### 如何远程连接运行于docker容器上的Mysql
- 获取远程mysql的host和port
    可通过 docker inspect <container_name> 查看IP地址，mysql默认运行于3306端口
- 进入容器开启远程访问
    进入mysql容器 ：docker exec -it <container_name> bash
    进入mysql: mysql -u roor -p 
    开启远程访问：ALTER USER 'root'@'%' IDENTIFIED WITH mysql_native_password BY 'root'