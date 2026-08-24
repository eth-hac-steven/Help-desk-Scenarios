**Subject:** I can't print anything but my colleagues can

**Ticket No:** IT-2026-4213

**Username:** ejoseph

**Department:** Admin

**Time Submitted:** 03:40 PM

**Description:** I've been trying to print a document but nothing comes out on my end. I checked with my colleagues on the same printer and it's working fine for them, so it seems to be just my computer.

**Assigned to:** Eth-steve

### Resolving User-Ticket

1. Confirmed the user is connected to the correct company network for the printer.
2. Running
   ```
   ping <printer-ip>
   ```
   - confirmes 4/4 packets sent and received, verifying network path to the printer was fine.
3. Restarted the Print Spooler service (`services.msc` → Print Spooler → Restart) to clear any stuck spooler process the most common single fix.
4. Checked the print queue for a stuck/corrupted job blocking the user's print jobs and cleared it.
   - To check this; 
      - Open setting
      - Click on ``Bluetooth & Device``
      - Click on ``Printer & scanners``
      - Click on the printer
      - Click on the print Queue
      - Clear/delete the previously queued files
      
5. Confirmed the correct printer was set as default on the user's machine.
    - To check this;
        -  in the word/excel 
        - holding ``Ctrl + p`` opens the print menu
        - check which printer the user is actually sending the file to.
          
8. Closed and reopened the document/print dialog to refresh the printer connection.
9. If issue persisted, removed and re-added the printer, reinstalling the driver.
10. Checked physical/USB cable connection if the printer was locally connected, and reseated it.
11. Verified shared printer permissions if applicable.

**Status:** Resolved
