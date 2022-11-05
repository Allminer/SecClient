# SecClient  安全客户端
# 海外一键安装脚本
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Allminer/SecClient/main/seclient.sh)"
```

# 国内一键安装脚本
```bash
/bin/bash -c "$(curl -fsSL https://cdn.jsdelivr.net/gh/Allminer/SecClient@main/seclientcn.sh)"
```
开启服务
```bash
systemctl start seclient
```

重启服务
```bash
systemctl restart seclient
```
停止服务
```bash
systemctl stop seclient
```
安装好程序以后首先要配置安全客户端的端口指向  打开/opt/seclient/目录下proxy_config.yaml  修改 Target: "${sip}:{sport}"  例：（Target: "baidu.com:3333"）  然后开启客户端服务systemctl start seclient

例：
```bash
Proxies:
  - Listen: ":19001"         配置本地端口
GRPC:
  Target: "baidu.com:3333"     安全客户端端口指向
  TLSConfig:
    Cert: certs/client_cert.pem
    Key: certs/client_key.pem
```

矿机连接 stratum+tcp://本地客户端IP:端口  

例：stratum+tcp://192.168.1.254:19001
