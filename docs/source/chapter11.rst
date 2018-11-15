chapter 11: Ware house
====================================


1. python pip install
  python path에 scripts도 추가

D:\SEANLAB2\IoT\aWareHouse\aWareHouse\Server

pip install -r requirements.txt

2. install influxdb

ubuntu
wget https://dl.influxdata.com/influxdb/releases/influxdb_1.4.3_amd64.deb
sudo dpkg -i influxdb_1.4.3_amd64.deb

influxd -config /etc/influxdb/influxdb.conf

$ sudo apt-get install python-pip python-dev build-essential
$ sudo pip install --upgrade pip
$ sudo pip install --upgrade virtualenv



veyon



X displays are protected by a "key" which you need to give in order to be able to connect. That key will generally be stored in the user's ~/.Xauthority file.

To allow someone else's application (like x11vnc) to connect to his DISPLAY, a user has to give him that key or grant him access to his ~/.Xauthority file. You can retrive the key of your display by doing.

xauth list "$DISPLAY"

You can grant access to your ~/.Xauthority by changing its permissions (group ownership or ACLs).

The other user can specify which authority file to use via the XAUTHORITY environment variable, or add a key to a specific display to his own ~/.Xauthority using xauth add.
