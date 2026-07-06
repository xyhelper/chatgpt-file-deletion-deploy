# chatgpt-file-deletion-Deploy

chatgpt-file-deletion 快速部署脚本库


## 前置条件
- 一台至少 2 核 2G 内存的服务器,推荐使用香港、新加坡、日本地区的服务器,可以兼顾国内访问。
- 安装了 docker 和 docker-compose
- 安装了 git


## 自动部署

在服务器上执行以下命令即可

```bash
curl -sSfL https://raw.githubusercontent.com/xyhelper/chatgpt-file-deletion-deploy/main/quick-install.sh | bash

```

## 手动部署

1. 克隆本仓库到服务器上

```bash
git clone --depth=1 https://github.com/xyhelper/chatgpt-file-deletion-deploy.git chatgpt-file-deletion
```

2. 进入目录

```bash
cd chatgpt-file-deletion
```

3. 启动服务

```bash
./deploy.sh
```

## 配置docker-compose环境变量
- GPTPROXY=chatgpt接入点地址
- WEBHOOKURL=企业微信机器人webhook地址（如果不用企业微信通知可不配置）
- CONCURRENCY=账号并发数量 

## 使用方法

页面访问地址为 http://服务器 ip:9900/gpt.html



