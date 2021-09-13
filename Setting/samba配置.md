#### 1.通过配置smaba共享终端的目录:  
修改 /etc/samba/smb.conf,在末尾添加：一下内容：
```bash
[workspace]
    comment = workspace
    browseable = yes
    path = /home/*****/workspace
    create mask = 0777
    directory mask = 0777
    force group = nogroup
    public = yes
    available = yes
    writable = yes
```
#### 2.访问该共享目录：
```bash
\\192.168.**.**\workspace
```

#### 3.页面访问：
```bash
file:\\192.168.**.**\workspace
```

