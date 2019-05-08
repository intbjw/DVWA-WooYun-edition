# DVWA-WooYun-edition
web渗透测试平台在docker上的搭建
## 如何使用

### 1. 创建 docker 镜像(image)

```bash
$ docker build -t wooyun .
```

### 2. 创建 docker 容器(container)

```bash
# 本容器 80 端口映射到宿主机的 8082 端口上
$ docker run -d --name wooyun_vul -p 0.0.0.0:8082:80 wooyun
```
### 3. 访问地址

**安装**

http://127.0.0.1:8082/setup.php


## 配置说明

* mysql 账号
> root/

* apache2 工作目录
> /var/www/html/

* DVWA 账号
> admin/password

## 参考链接

* [DVWA-WooYun-edition地址](https://sourceforge.net/projects/dvwa-wooyun/)
