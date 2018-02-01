# FishLine
Fishline is an SMS based application that allows users to advertise through the SayCel / PearlCel Network.  It was originally developed for fisherman who come from the sea with their latest catch.  It was broadened to shop owners and business in Pearl Lagoon. 

Fishline requires Rhizomatica Community Cellular Network (RCCN).  SayCel has a fork of RCCN, but Rhizomatica's has the latest updates.
RCCN Puppet Installation: https://github.com/Rhizomatica/puppet

Fishline Consists of two files:
- sms.py 
- fishline.py

Installation: 

1. Put the fishline.py file in "/var/rhizomatica/rccn/modules/" folder in bsc
2. Replace the older sms.py file in "/var/rhizomatica/rccn/modules/" folder with the attached file  
3. Run the command 'ps aux|grep rapi.py'. You will see a process, you have to kill that process. Don't worry it will automatically restart once you kill it. 
4. You are done installing fishline in your bsc 


How to use the application:

You have to subscribe a user before he can start advertising. You subscribe by sending an "subscribe TA" to 20000. Instead of TA use the initials of the fisherman. Now he can advertise. 

If he sends a text message to 2000 he will get a response back saying please confirm. If he replies yes his add will be sent to everyone. 


Pamphlet of instructions used in PearlCel pilot:

![Fishline Pamphlet](https://github.com/saycel/FishLine/blob/master/images-for-readme/Fishline%20Pamphlet%20(1).jpg)
