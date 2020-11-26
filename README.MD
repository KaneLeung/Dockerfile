# 各类自用的Dockererfile

### 帆软报表服务器(v10.0试用版)
+ 最后更新日期 2020-11-26
[源码位置](https://github.com/KaneLeung/Dockerfile/FineReport)

> 或直接使用已打包好的镜像
```shell
docker push kaneleung/finereport:v10.0
docker run -p 8080:8080 -d --name finereport finereport:v10.0
```