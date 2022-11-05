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
