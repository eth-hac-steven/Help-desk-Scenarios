# Network Issues V.4 (Proxy Issue)

**Subject:** I have connected to the internet but i can not still browse.

**Ticket No:** IT-2026-4521

**Username:** Oshegun

**Department:** Sales

**Time Submitted:** 08:15 AM

**Description:** I've been connected to the internet for a while now but i have not been able browse anything since morning, the WIFI sign is saying i am connected but nothing yet,and its not just the office wifi but every other one i connect to even my phones hotspot, what is happening??

### Resolving User-Ticket
1. On CMD i checked the IP using
   ```
   ipconfig 
   ```
   It was correct.
   image 
2. Ran
   ```
   ping 8.8.8.8
   ```
   ```
   ping google.com
   ```
   The ping was successful, this rule out DNS as the cause.
3. Tried searching for anything using the browser and got back this error
   image 
4. with the error in mind, open setting
5. select ```Network and internet```
6. select ```proxy```
7. while there i noticed the ```Manual Proxy setup``` was ```on```
8. Click on ```set  up```
9.  Asked Mr.Shegun if he had need of a Proxy server, he said no.
10. Turn it off.
11. Returned back to the browser and refreshed the page
12. Internet Access was restored

**Status**: Resolved
  
