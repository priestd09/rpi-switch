This is a small app running on Raspberry Pi as s remote switch for garage doors.

# Prerequisities 

* a garage doors motor with connector to manual control like ... 
* Raspberry Pi with a connection to home wifi
* Relay module to control the doors motor like this one https://www.sparkfun.com/products/13815

# Software used 

* standard Raspberry's Raspian image up to date
* connection to Wifi configured
* WebIOPi from  http://webiopi.trouch.com/INSTALL.html
* Udpate /etc/webiopi/config to direct to custom web page like `doc-root=/home/pi/WebIOPi-0.7.0/mydoors`
* Copy index.html to `/home/pi/WebIOPi-0.7.0/mydoors` and customize IO pin number where is relay connected


