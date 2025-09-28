# bigdata-dock

基于 Docker Compose 搭建的大数据服务环境

# IP地址
内部IP地址从 172.25.27.3 开始

# 服务清单

| status | service | backend ip | version | 备注 |
|---|---|---|---|---|
| doris-fe | 172.25.27.80 | 3.1.0 | |
| doris-be | 172.25.27.81 | 3.1.0 | |
| mysql | 172.25.27.87 | 8.3 | |
| flink-jobmanager | 172.25.27.89 | 2.1.0-java17 | |
| flink-taskmanager | 172.25.27.90 | 2.1.0-java17 | |


# 使用到的镜像
- 默认使用docker.io 镜像
- 若想使用自定义仓库镜像，需要定义 `DOCKER_REGISTRY_URL` 变量

```json
[
    "traefik:v3.4",
]
```
