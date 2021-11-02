#### 1.获取vps
[access vultr](https://my.vultr.com/)

#### 2.登录vps terminal
```bash
bash <(curl -s -L https://git.io/v2ray.sh)
```
如果提示 curl: command not found ，那是因为你的 VPS 没装 Curl ubuntu/debian 
系统安装 Curl 方法: 
```bash
apt-get update -y && apt-get install curl -y centos
yum update -y && yum install curl -y
```
根据提示安装V2Ray
[参考](https://github.com/xiaoming2028/FreePAC)

#### 3.通过V2Ray查看运行状况


#### 4.优化 V2Ray
```bash
v2ray bbr
# 查看bbr是否重启
lsmod | grep bbr
```

#### 5.查看是否开启2333端口并开启
```bash
firewall-cmd --list-ports
firewall-cmd --zone=public --add-port=2333/tcp --permanent
reboot
```

#### 6.获取vmess
```bash
v2ray url
v2ray qr
```











