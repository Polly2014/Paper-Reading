# Docker Portainer使用笔记
## What is Portainer
> Portainer是一款轻量级的图形化管理工具，通过它我们可以轻松管理不同的docker环境。Portainer部署和使用都非常的简单，它由一个可以运行在任何docker引擎上的容器组成。Portainer提供管理docker的containers、images、volumes、networks等等。它兼容独立的docker环境和swarm集群模式。基本满足中小型单位对docker容器的管理工作。
## Portainer部署
```sh
# 从仓库中查询Portainer相关镜像
docker search portainer
# 拉取Portainer镜像到本地
docker pull portainer/portainer
# 创建Volume
docker volume create portainer_data
# 启动Portainer
docker run -d \
  -p 9000:9000 \
  --name portainer \
  --restart always \
  -v /var/run/docker.sock:/var/run/docker.sock \
  -v portainer_data:/data \
  portainer/portainer
```
