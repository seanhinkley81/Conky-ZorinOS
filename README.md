# Conky-ZorinOS
Conky Config for Zorin OS
Modified Conky Config file for Zorin OS Based off Klaatu-Conky-Conf

http://conky.sourceforge.net/docs.html

http://conky.sourceforge.net/variables.html

https://linuxconfig.org/ubuntu-20-04-system-monitoring-with-conky-widgets

https://github.com/brndnmtthws/conky/wiki

https://cairographics.org/manual/

https://github.com/Eboreg/klaatu-conky-conf/


//Install Conky
sudo apt install conky-all

//Install Sensors
sudo apt install lmsensors

//Install Awesome font

https://fontawesome.com/

Goto Home folder create directory .conky

Copy Project files to
~./conky

launch with command conky - c ~/.conky/conky.conf

//Create Auto Launch File
in Home directory right-click create new text file
add the following line

wait 10 & conky -c ~/.conky/conky.conf

save as conky.sh

right click conky.sh Properties > Permissions > Check 'allow executing file as program' 

// Setup Auto Launch

in Zorin Application Menu 

Settings > Start Up Applications
ADD
Name: Conky
Command: /home/%uname%/conky.sh    //Replace %uname% with you username
Comment: Conky