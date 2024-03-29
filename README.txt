webserver prototype

1) unzip the html folder
2) unzip the jsmol folder
3) unzip my_examples folder
4) move the jsmol and my_examples folders into the html folder
5) move contents of this html folder into the html folder in your local apache server

instructions for running this page on your local server goes as follows

#####################################################################################

WELCOME to our summer 2022 webserver project

to test on localserver

http://127.0.0.1
or
http://localhost

after installing local apache server via LAMP or XAMPP stack
instructions for installing LAMP or XXAMP stack is found here
https://www.alphr.com/set-up-local-web-server/

######################################################################################

for Linux Mint simply install LAMP server with the following terminal command

$ sudo apt-get install apache2

NOTE: This webserver will eventually run on our Linux server, so it is simpler to develop and test it on a Linux Mint laptop. If you have an older unused laptop lying around, you should convert its OS to Linux Mint and use it as a machine for code development. You might also try VirtualBox Virtual Machine (VM) with Linux image (IF YOU DONT HAVE ACCESS TO A LINUX OS ANY OTHER WAY), however I find that it can be very difficult to get client-side graphics to appear/function properly over the scaled graphics on a VM desktop.  If you do use Windows or Mac for the project, we recommend setting up a XAMPP server instead of a linux LAMP server.

Instructions for XAMPP server setup
https://www.apachefriends.org/index.html


Instructions for a new 'bare metal' Linux install
https://www.linuxmint.com/


Instructions for VM install (Linux running over existing operating systems)
install Oracle VirtualBox and follow its instructions to build your VM using a Linux Mint .vdi file from osboxes.org
https://www.virtualbox.org/
and
https://www.osboxes.org/

the user and password will both be osboxes.org

###################################################################

After setting up local server: 

Download, unzip and put all the files from this GitHub project repo in your Linux file system at /var/www/html/

You may need to open permissions to copy files there by using this terminal command

$ sudo chmod -R 777 /var/www/html/
or
$ sudo chmod ugo+rwx /var/www/html/

When everything is in place, you open your chrome/firefox browser to the address

https://127.0.0.1

and this will show a functional version of index.html  
If you simply open index.html directly in the browser not all of the supporting code will work (i.e. JSmol viewers will not function)

The plots in this site are using ploty.js running on d3.js  (more information found below)

https://plotly.com/javascript/

Our divergence plots are modified candlestick plots from ploty.js library

#######################################################################

The three 'example' buttons should be workng and open results using plotly and JSmol, but at this stage all the left hand side of the page is not yet built. 



