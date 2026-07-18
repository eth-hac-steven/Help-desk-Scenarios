#  Network issues (V.2-DNS)

 ### Scenario 
 Mr. johnny made a compliant this morning say he cant access  the internet in his cubicle but other around him, please investigate, resolve and close this ticket.

 ### Troubleshooting the Issue 
 - The ticket says he cant access the internet but other can.
 - upon getting to  his system  is the eternet connected sign in the action bar , which seems strange taking the compliant into account
 - i then decided to search for www.google.com and that failed revealing an interesting 
 - i then open the command prompt and ran
````
 ipconfig 
````
(it has an ip)
````
ping 8.8.8.8 
````
(4 packets successfully sent)
````
ping google.com 
````
 (that failed)
 - This reveals that the issue is DNS (Domain name resolution), which is responsible for mapping domain name like google.com, to an ip (8.8.8.8(Google DNS server)/172.217.22.14).

### Solution 
- A simple fix would be to flush the DNS in CMD
    - ipconfig /flushdns
- this clears dns cache that may be broken.
- Another fix would be 
 - hold WIN + R
 - Enter : ncpa.cpl
 - select the interface 
 - right click on it , select properties
 - select ipv4
 - click on properties
 - in the dns either
      - clear and replace the existing ip
      - Enter a new one
 - click apply
 - click on save
 - Then test it by trying to access the internt again
 -  if all have said does not work ,we can always restart the system 😄

 ***with this done the ticket is closed***
 
