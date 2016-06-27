# docker 服务build脚本
------
## 目录
<pre>
--- root
  --- apache (centos6下的httpd服务)
  --- nginx  (ubuntu12.04下的nginx服务)
</pre>

## 如何使用？
```bash
sudo docker pull centos
sudo docker build -t='<resp name:tag>' <Dockerfile>
```
## apache
centos下安装httpd服务，替换端口为`8080`,build完成后启动：
```bash
sudo docker run -d -p 8080:8080 --name httpd <resp name:tag>
```

## nginx
```bash
sudo docker run -d -p 8081:80 --name nginx-httpd <resp name:tag>
```
