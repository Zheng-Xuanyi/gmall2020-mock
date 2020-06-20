# gmall2020-mock

## 1.gmall2020-mock-db

这是一个模拟的业务数据生成器

可以根据要求修改gmall2020-mock-db/src/main/resources/application.properties配置文件中的参数


## 2.gmall2020-mock-log

这是一个模拟的日志生成器

1)application.properties配置文件：

```
# 外部配置打开
# logging.config=./logback.xml
#http模式下，发送的地址：生成的日志数据可以通过http请求发送出去，模拟用户端访问日志服务器
mock.url=http://localhost:8080/applog
```

2)logback.xml配置文件：负责日志生成的各项配置：存储位置、生成格式、不同级别日志的存储方式等

使用方法：
- 修改对应的配置文件
- 打包
- java -jar 执行

