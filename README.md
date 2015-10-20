## Influxdb docker 

influxdb的版本是0.9.4.2, 此次dockerfile不适合做influxdb集群.因为在docker run的启动参数里面, 没有映射相关参数.  由此需求的朋友，可以等我下次发布的dockerfile.

现在暂时只有ubuntu, 后期务必会加入centos的支持

###usage:

通过dockerfile构建一个镜像
```
docker build -t fengyun/influxdb Dockerfile
```

启动一个容器
```
docker run --rm -it -p 8083:8083 -p 8086:8086 fengyun/influxdb
```


