# XRayR

Find the source code here: [youzi3/XrayR](https://github.com/youzi3/XrayR)

# 一键安装

```
wget -N https://raw.githubusercontents.com/1660limo/xrayryd/main/install.sh && bash install.sh
```

# Docker 安装

```
docker pull misakano7545/xrayr:latest && docker run --restart=always --name xrayr -d -v ${PATH_TO_CONFIG}/config.yml:/etc/XrayR/config.yml --network=host misakano7545/xrayr:latest
```

# Docker compose 安装

1. 安装docker-compose: 
```
curl -fsSL https://get.docker.com | bash -s docker
curl -L "https://github.com/docker/compose/releases/download/1.26.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
```

2. `git clone https://github.com/youzi3/XrayR-script XrayR-release`
3. `cd XrayR-release`

## Docker compose升级

在docker-compose.yml目录下执行：

```
docker-compose pull
docker-compose up -d
```
