# auto-macchanger
step i
script for auto macchager 
"#!/bin/sh
macchanger -e eth0
macchanger -e eth0
macchanger -e eth0
exit"

step 2 
make this file exicutable by using "chmod +x ......sh

step 3 
fire the command crontab -e and add following tax in first line 
@reboot /home/kali/Documents/mac.sh
Note: """you have to mention path and file name what you use in you shell script"""

step 4 
systemctl enable cron.service
systemctl start cron.service

step 5 
update-rc.d cron defaults





