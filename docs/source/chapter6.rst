chapter 6: mblock
==================================

* windows

1.visual studio community 2017 install
2.windows- dev- dev command line 관리자 권한으로 실행
3.>npm install

npm install --production windows-build-tools

VC community 2017 install & C++ check


electron install
>npm install electron
npm install electron --save-dev --save-exact

D:\SEANLAB2\mBlock2   ==>> OK
npm install
npm run rebuild-serialport
npm run rebuild-hid
npm run rebuild-bluetooth
npm start

mblock  ===> 연결 OK
D:\SEANLAB2\mBlock2\Firmware\baseboard_firmware_uno_minitank ==>Motor OK





hex file
D:\SEANLAB2\mBlock2\mBlock\tools\hex\uno.hex
down

connect -com12-

board -uno



LED OK

mBlock 도 OK



protocol

서보모터 6-9 port 초기 이니셜때만 됨



mblock
Bluetooth  ==> OK
Bluetooth 연결 - Serial 8번 선택  ==>OK   ( BT 패스워드가 바뀌어 등록 안되어 안되었음)
 BTSerial.write("AT+PIN1234"); 바로 삽입


apt-get install libbluetooth-dev

sudo vim /usr/lib/systemd/system/bluetooth.service

and adding the --compat flag to the ExecStart value:

ExecStart=/usr/lib/bluetooth/bluetoothd--compat

Finally, restart the service:

systemctl daemon-reload systemctl restart bluetooth



sudo apt-get install libusb-1.0-0-dev

npm install electron


x-11 proxy
mcookie
c29ee074c51368664c164e7c5c0a747d
xauth add localhost/unix:14 MIT-MAGIC-COOKIE-1 c29ee074c51368664c164e7c5c0a747d
08e4af70e0fcf25e927ff7683ab9ddb3

xauth add localhost/unix:14 MIT-MAGIC-COOKIE-1 08e4af70e0fcf25e927ff7683ab9ddb3






On my client PC I'm running Windows 10 and I have installed XMing and Xming Fonts.

I am running Putty and I have configured it to enable X11 Forwarding. I have tried leaving the X display location blank (as default) and also with the value :0.0.

On my server I'm running Ubuntu on AWS. I edited the /etc/ssh/ssh_config file to include the following two lines:

ForwardX11 yes
ForwardX11Trusted yes

I also installed xauth using sudo apt-get install xauth

Whenever I try to run an application, like xterm & or xclock I get the same error:

PuTTY X11 proxy: Unsupported authorisation protocol
Error: Can't open display: localhost:10.0

windown mblock
관리자 권한으로 실행

npm install --global --production windows-build-tools


