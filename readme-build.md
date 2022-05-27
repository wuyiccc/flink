# 1. MAVEN镜像仓库配置

```shell
        <mirror>
            <id>confluent</id>
            <mirrorOf>confluent</mirrorOf>
            <name>confluent</name>
            <url>http://packages.confluent.io/maven/</url>
        </mirror>
```

# 2. 编译命令

## 2.1 前端项目编译

```shell
cd ./flink-runtime-web/web-dashboard
```

```shell
npm install
```

```shell
npm run build
```

## 2.2 全局编译

```shell
mvn clean install '-DskipTests' '-Dfast'
```
