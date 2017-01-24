This is a small app running on Raspberry Pi as s remote switch for garage doors. The RPI is connected to home Wifi that is accessible outside the house as well. Any mobile phone/pc that hasve access to home Wifi can access RPIs website and open / close the garage doors. No more specific garage doors remote control is required :)

# Prerequisities 

* a garage doors motor with connector to manual control like Hormann etc 
* Raspberry Pi with a connection to home wifi
* Relay module to control the doors motor like this one https://www.sparkfun.com/products/13815

# Software used 

* standard Raspberry's Raspian image up to date
* connection to Wifi configured
* WebIOPi from  http://webiopi.trouch.com/INSTALL.html

# Configuration
* connect the relay module to RPI's GPIO pin 2
* Udpate /etc/webiopi/config to direct to custom web page like `doc-root=/home/pi/WebIOPi-0.7.0/mydoors`
* Copy index.html to `/home/pi/WebIOPi-0.7.0/mydoors` and customize IO pin number where is relay connected
* If relay pin connected to an another pin, udpate index.html to right pin number

# Security
* the RPI is conneted to homes Wifi that is considered secure
* if additional security is required, customize RPIs web server to introduce aditional authentication
* cusotmize RPIs transport protocol to use SSL/https to make secure trasfer if possible
* if paranoic with home security, install VPN server to RPI and connect only clients with the VPN setup can access the garage doors

# TBD 
* connect camera to broadcast image of the garage door to check if open / closed
* integartion to an home automation system / dashboard

# Image gallery from my installation

https://goo.gl/photos/6mYRy5UKS8qQs6747


