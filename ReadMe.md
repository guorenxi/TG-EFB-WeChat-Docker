# TG-EFB-Wechat-Docker

EFB-WeChat的Docker部署方式

## 使用

### 配置

根据提示进行配置，`/root/wechat/config`为配置文件目录

```bash
docker run --rm -it --name="efb-wechat" -v /root/wechat/config:/app/config xzsk2/efb-wechat-docker:latest efb-wizard
```

### 运行

```bash
docker run -d --restart=always --name="efb-wechat" -v /root/wechat/config:/app/config xzsk2/efb-wechat-docker:latest
```

### 停止

```bash
docker container stop efb-wechat
```
