## 常用命令

### 查询过滤
- grep -v 申报稿 | sort | uniq --check-chars=6     针对前6个字符去重

### 远程登录
- ssh-keygen -t rsa -b 2048
- ssh-copy-id user@server
- sudo yum install -y sshpass
- sshpass -p password ssh -oStrictHostKeyChecking=no ip

### 进程查看
- nc -v -w5 ip 9092
- netstat -nap | grep pid  
- pwdx pid  查看进程位置

### 文本编码配置
- export LC_ALL="en_US.UTF-8"

### 文件处理
- zip -FF xx.zip --out yy.zip

### 防火墙开关
- sudo firewall-cmd --zone=public --add-port=12301/tcp --permanent
- sudo firewall-cmd --reload
- iptables -A INPUT -p tcp --dport 22 -j DROP
- iptables -A OUTPUT -p tcp --sport 22 -j DROP

### 包依赖修复
- libmysqlclient.so.18: cannot open shared object file: No such file or directory
- sudo PATH=/usr/local/mysql/bin/:$PATH pip install mysql-python

