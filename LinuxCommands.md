1.  touch song{1..10}.mp3 mkdir Music\_Directory mv song\*
    Music\_Directory ln -s Music\_Directory Audio\_Directory

2.  sudo adduser bob sudo adduser rob sudo adduser max sudo usermod -a G
    sysadmin,manager bob sudo usermod -g sysadmin bob sudo usermod -a G
    sysadmin,manager rob sudo usermod -g sysadmin rob sudo usermod -a G
    sysadmin max sudo usermod -g sysadmin max

3.  Open etc/passwd with an editor and change
    max:x:1001:1001:,,,:/home/max:/bin/bash to
    max:x:1001:1001:,,,:/home/max:/bin/false

sudo chage -E `date -d "30 days" +"%Y-%m-%d"` max

sudo passwd -e Bob

​4. mkdir manager (from home dir) sudo chgrp -R manager manager sudo
chmod -R 2770 manager

​5. sudo useradd -u 4223 gabriel

​6. mkdir /tmp/var tar -cvjf /tmp/var/archive.tar.bz2 /etc/hosts

​7. grep -i "udp" /etc/services \> udp\_services.txt

​8. top shift+f select &cpu and press s Esc

​9. sudo gedit \~/.bashrc add a line there - alias bup='/usr/bin/uptime'

​10. vim hello.txt press i for insert mode and esc to go back to command
mode In insert mode we can type like regular text editor In command mode
x - del :q! - quit without saving :wq - save and quit

​11. sudo apt-get install firewalld sudo firewall-cmd --get-default-zone
sudo firewall-cmd --set-default-zone=dmz sudo firewall-cmd --get-zones
\> zones.txt

​12. firewall-cmd --zone=public --add-port=8080/tcp --permanent sudo
netstat -ntlp | grep LISTEN \> zones.txt

​13. sudo iptables -t nat -A PREROUTING -i eth0 -p tcp --dport 80 -j
REDIRECT --to-port 8080
