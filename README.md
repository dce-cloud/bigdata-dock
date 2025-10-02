# bigdata-dock

基于 Docker Compose 搭建的大数据服务环境

# IP地址

内部IP地址从 172.25.27.3 开始

# 服务清单

| status | service | backend ip | version | 备注 |
|---|---|---|---|---|
| &check; | mysql | 172.25.27.3 | 8.3 | |
| &check; | doris-fe | 172.25.27.5 | 3.1.0 | |
| &check; | doris-be | 172.25.27.6 | 3.1.0 | |
| &check; | jobmanager | 172.25.27.8 | 2.1.0-java17 | |
| &check; | taskmanager-1 | 动态ip | 2.1.0-java17 | |
| &check; | taskmanager-2 | 动态ip | 2.1.0-java17 | |
| &check; | taskmanager-3 | 动态ip | 2.1.0-java17 | |
| &check; | dinky | 172.25.27.15 | 1.2.4 | |

# 使用到的镜像

```json
[
    "apache/doris:be-3.1.0",
    "apache/doris:fe-3.1.0",
    "flink:1.18-scala_2.12-java17",
    "mysql:8.4.6-oraclelinux9",
    "dinkydocker/dinky-standalone-server:1.2.4-flink1.18"
]
```
