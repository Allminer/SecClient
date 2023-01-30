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
安装好程序以后访问IP网页进行配置端口为21112  http://ip:21112



矿机连接 stratum+tcp://本地客户端IP:端口  

例：stratum+tcp://192.168.1.254:19001
