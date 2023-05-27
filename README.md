# SecClient  安全客户端
# 海外一键安装脚本
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Allminer/SecClient/main/seclient.sh)"
```

# 国内一键安装脚本
```bash
/bin/bash -c "$(curl -fsSL https://cdn.jsdelivr.net/gh/Allminer/SecClient@main/seclientcn.sh)"
```

# WIN版下载地址
[win版安全客户端.rar](https://github.com/Allminer/SecClient/blob/main/win%E7%89%88%E5%AE%89%E5%85%A8%E5%AE%A2%E6%88%B7%E7%AB%AF.rar)

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
安装好程序以后先执行开启服务命令 systemctl start seclient 然后 访问IP网页进行配置端口为21112  http://ip:21112
(openwrt系统 systemctl命令无效，须要用安装脚本菜单启动程序)



矿机连接 stratum+tcp://本地客户端IP:端口  

例：stratum+tcp://192.168.1.254:19001


适用于矿场，破解宽带运营商的连接数限制，数据加密更安全

# 特别注意
如果allminer服务器后台没有上传自定义证书，那么安全客户端在添加端口的时候，是必须要勾选略过服务器证书检测,

![image](https://github.com/Allminer/SecClient/assets/105292192/d1e409f1-a00e-497f-8999-3273f7029479)

![image](https://github.com/Allminer/SecClient/assets/105292192/b5796c70-e165-4076-b823-cc9ff36d7257)


