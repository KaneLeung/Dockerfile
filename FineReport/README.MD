# 帆软报表[FineReport]服务器Dockerfile

> 更新日期：20201126

> 帆软版本：v10.0 试用版

> 欢迎访问我的[Github](https://github.com/KaneLeung/Dockerfile) https://github.com/KaneLeung/Dockerfile

### 方法一：自行打包镜像

1. 从帆软官网下载服务器安装压缩包，[下载地址](https://www.finereport.com/product/download)

2. 将压缩包内tomcat-linux\webapps\webroot\路径下的三个文件夹拷贝到本项目下的webroot文件夹内

3. 打包镜像
```shell
cd 到当前目录
docker build -t finereport:v10.0 .
```
4. 运行打包好的镜像
```shell
docker run -p 8080:8080 -d --name finereport finereport:v10.0
```

### 方法二：直接使用已打包好的镜像

```shell
docker push kaneleung/finereport:v10.0
docker run -p 8080:8080 -d --name finereport finereport:v10.0
```