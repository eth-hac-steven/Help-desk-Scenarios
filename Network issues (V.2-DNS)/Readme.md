#  Network issues (V.2-DNS)

**Subject:** My laptop says I'm connected to Wi-Fi but no websites will open

**Ticket No:** IT-2026-4621

**Username:** jdoe

**Department:** Operations

**Time Submitted:** 09:14 AM

**Description:** My Wi-Fi icon shows I'm connected, but none of the websites I try to open are loading, on any browser. Please help.

**Assigned to:** Eth-steve

### Resolving User-Ticket

1. Confirmed which network the user is connected to (personal hotspot vs. office Wi-Fi vs. an unrecognized open network) to scope the issue.
2. If on the office network,i ran
 ```ipconfig /all```
to check the assigned IP address.
   - Looked for an APIPA address (169.254.x.x), which indicates a failed DHCP request, the device never got valid network settings from the router/DHCP server.
   - If APIPA present: released and renewed the IP with
     
 ```
 ipconfig /release
```
 
 then
 
 ```
 ipconfig /renew
```

so the device can request for a new IP from the DHCP server.
- Then checked the Ethernet cable/AP if the issue persisted.
  
3. If a valid IP was assigned, pinged the default gateway to confirm local network connectivity.
5. Ran
   ```
   ping 8.8.8.8
   ```
   (Google free Domain Name IP address)
   ```
   ping google.com
   ```
   ping the domain name this time to isolate the fault:
   - if the IP ping succeeds, while the domain ping fails → DNS issue.
   - Flushed DNS cache
   ```
   ipconfig /flushdns
   ```
   and/or manually set DNS to 8.8.8.8 / 1.1.1.1 to test.
   To do that i would:
   - hold WIN + R
 - Enter : ncpa.cpl
 - select the interface 
 - right click on it , select properties
 - select ipv4
 - click on properties
 - in the dns either
      - clear and replace the existing ip 
      - Enter a new one(when replacing use an ip that has not been assigned to another Device)
 - click apply
 - click on save
 - Then test it by trying to access the internet again
 
   - Both fail → connectivity/routing issue, escalated to AP/switch/gateway check.
7. If user was on an unrecognized open Wi-Fi, disconnected and reconnected to the correct office network.
8. Confirmed resolution by loading a website in-browser.

**Status:** Resolved
