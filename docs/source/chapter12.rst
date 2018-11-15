chapter 12: Docker
===========================


*ubuntu14.04
1.remove old version
sudo apt-get remove docker docker-engine docker.io

2. install

sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    software-properties-common

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

sudo apt-key fingerprint 0EBFCD88

sudo apt-get update


sudo apt-get install docker-ce

docker run -d -p 8083:8083 -p 8086:8086 -e ADMIN_USER="root" -e INFLUXDB_INIT_PWD="root" -e PRE_CREATE_DB="warehouse" tutum/influxdb:latest
docker run -d -p 8083:8083 -p 8086:8086 -e ADMIN_USER="admin" -e INFLUXDB_INIT_PWD="admin" -e PRE_CREATE_DB="warehouse" tutum/influxdb:latest


docker run -it -d -p 8061:8061 tislaamo/blockpy


##docker cloud9
docker run -it -d -p  8071:8071 -v /home/sean/docker_workspace:/workspace/ kdelfour/cloud9-docker

docker run -it -d -p  80:80 -v /home/sean/docker_workspace:/workspace/ kdelfour/cloud9-docker

sudo ufw allow 8071/tcp

sudo cat /proc/sys/net/ipv6/conf/all/disable_ipv6

sudo sysctl -p


docker attach mynodered
To stop the container:

docker stop mynodered
To start the container:

docker start mynodered