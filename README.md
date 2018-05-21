# docker-dev-lamp
docker-compse进行的LAMP一键服务启动编排

安装docker-compse以后 下载以下文件 执行以下命令 即可启动服务

#启动、创建进行并开启服务
docker-compose up -d
#重启服务
docker-compose restart
#停止服务并删除容器
docker-compose down



包含以下服务

APACHE:PH5.5
   port:9090  
   端口可自行调整 数据目录可自行参考文件注释 修改挂载点
APACHE:PHP7.0
   port:9097
   端口可自行调整 数据目录可自行参考文件注释 修改挂载点
mysql:5.5
   port:3307  user:admin  password:123456
   数据目录可自行参考文件注释 修改挂载点
mysql:5.6
   port:3308  user:admin  password:123456
   数据目录可自行参考文件注释 修改挂载点
   
memcache  
   port:11211
   
redis
   port 5672  15672
   
dnsmasq
   port:53  8083/web
   
   
