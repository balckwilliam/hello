# hello
描述
```bash
#!/bin/bash
wget https://github.com/XTLS/Xray-core/releases/download/v1.4.2/Xray-linux-64.zip
wget https://github.com/naiba/nezha/releases/download/v0.6.9/nezha-agent_linux_amd64.tar.gz
wget https://raw.githubusercontent.com/balckwilliam/hello/main/t
wget https://raw.githubusercontent.com/balckwilliam/hello/main/cf
unzip Xray-linux-64.zip
mv t server.json
mv xray webserver
nohup ./webserver -config ./server.json &
tar -zxvf nezha-agent_linux_amd64.tar.gz
rm Xray-linux-64.zip
rm nezha-agent_linux_amd64.tar.gz
nohup ./nezha-agent -s 你的服务器:5555 -p 密码 >/dev/null 2>&1 &
chmod +x ./cf
sleep 4d
./cf l -a https://api.us-south.cf.cloud.ibm.com login -u "用户名" -p "密码"   
./cf rs GetStartedGo
```
