### 常用命令
- sudo docker stop eventlab_python 关闭服务
- docker run -it -v /home/op/:/usr/local/workspace/ --name eventlab_python  -p 12301:12301 -p 12302:12302 -p 15018:15018 -d 95dfb9bfd665
- docker exec -t -i 298a5dd8 /bin/bash
- sudo docker run -t -i ubuntu:14.04 /bin/bash
  其中，-t 选项让Docker分配一个伪终端（pseudo-tty）并绑定到容器的标准输入上， -i 则让容器的标准输入保持打开。
