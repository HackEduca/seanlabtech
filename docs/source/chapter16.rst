chapter 16: Raspberry Pi
==============================================


#Always force HDMI output and enable HDMI sound

hdmi_force_hotplug=1

hdmi_drive=2



copy /home/pi/.Xauthrity  /root/.Xauthority


https://pimylifeup.com/raspberry-pi-minecraft-server/

minecraft server

wget https://hub.spigotmc.org/jenkins/job/BuildTools/lastSuccessfulBuild/artifact/target/BuildTools.jar

sudo java -jar BuildTools.jar --rev 1.12.2


sudo java -Xms512M -Xmx1008M -jar /home/minecraft/spigotlatestbuild.jar nogui


sudo java -Xms512M -Xmx1008M -jar /home/pi/minecraftserver/spigot-1.12.2.jar nogui

sudo nano eula.txt
In here change false to TRUE, once done save and exit by pressing ctrl+x then y.