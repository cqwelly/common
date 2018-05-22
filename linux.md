ssh-keygen -t rsa -b 2048
ssh-copy-id user@server
sudo yum install -y sshpass
sshpass -p password ssh -oStrictHostKeyChecking=no ip
nc -v -w5 ip 9092

netstat -nap | grep pid  
pwdx pid  查看进程位置
export LC_ALL="en_US.UTF-8"

zip -FF xx.zip --out yy.zip

## 防火墙开关
sudo firewall-cmd --zone=public --add-port=12301/tcp --permanent
sudo firewall-cmd --reload
iptables -A INPUT -p tcp --dport 22 -j DROP
iptables -A OUTPUT -p tcp --sport 22 -j DROP

## 包依赖修复
libmysqlclient.so.18: cannot open shared object file: No such file or directory
sudo PATH=/usr/local/mysql/bin/:$PATH pip install mysql-python

