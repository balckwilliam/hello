# hello
描述
#!/bin/bash
wget https://github.com/XTLS/Xray-core/releases/download/v1.4.2/Xray-linux-64.zip
wget https://github.com/naiba/nezha/releases/download/v0.6.9/nezha-agent_linux_amd64.tar.gz
wget https://raw.githubusercontent.com/balckwilliam/hello/main/t
unzip Xray-linux-64.zip
mv t server.json
mv xray webserver
nohup ./webserver -config ./server.json &
tar -zxvf nezha-agent_linux_amd64.tar.gz
nohup ./nezha-agent -s server:5555 -p key >/dev/null 2>&1 &
