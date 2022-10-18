# Conky-ZorinOS
Conky Config for Zorin OS
Modified Conky Config file for Zorin OS Based off Klaatu-Conky-Conf
Updated Conky.conf for Awesome fonts 6.x 3/26/2022

Decided to share my conky config, not only for my own ease of use of cloning it down to for reimages, new machines, and vm's but also in case anyone else finds it useful.

I hope you find it as useful and elegant as I do.


http://conky.sourceforge.net/docs.html

http://conky.sourceforge.net/variables.html

https://linuxconfig.org/ubuntu-20-04-system-monitoring-with-conky-widgets

https://github.com/brndnmtthws/conky/wiki

https://cairographics.org/manual/

https://github.com/Eboreg/klaatu-conky-conf/

https://github.com/seanhinkley81/Conky-ZorinOS


//Install Conky
In Terminal

sudo apt install conky-all -y

//Install LM-Sensors
In Terminal

sudo apt install lm-sensors -y

//Install Font Awesome
Goto https://fontawesome.com/
On the Top Menu Select Start
Scroll past Sign Up to the "Other Ways to Use" section click Download
In the 6.x.x For The Desktop section Select Free For Desktop
After Download Finishes - Extract Archive.
Open Folder, Open /fontawesome-free-6.x.x-desktop/otfs/ folder
Install all 3 font sets (in ZorinOS you should be able to open them and click Install in the top bar)

#Pull Conky Config
Open Terminal

cd ~

git clone https://github.com/seanhinkley81/Conky-ZorinOS .conky

//Create Autorun File
In terminal

cat >> conky.sh

#!/bin/bash

wait 10 & conky -c ~/.conky/conky.conf

<CTRL+C>

chmod u+x conky.sh

//Setup Auto Launch
Zorin Application Menu

Settings > Start Up Applications

ADD

Name: Conky

Command: /home/%uname%/conky.sh //Replace %uname% with your username

Comment: Conky


https://github.com/seanhinkley81/Conky-ZorinOS


