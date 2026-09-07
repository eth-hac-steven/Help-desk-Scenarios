# Printer Issue V.2 (Printer is offline)

**Subject**: I can't print my files,Printer says offline

**Ticket No**: IT-2026-4453

**Username**: Jonny.Test

**Department**: Admin

**Time Submitted**: 03:40 PM

**Description**: I wanted to print a document but the print says it is offline on my end. I checked with my colleagues on the same printer and it's working fine for them, so it seems to be just my computer.

**Assigned to**: Eth-steve

# Resolving User-Ticket

## Troubleshooting the Issue

- Upon getting to the user workstaion i noticed the user was not connected to the internet, which is exactly why mr Johnny can't print but other can, to Confirm .

- Run

```
ping <printer-ip>
```

-  4 packets sent and 0 received, verifying network path to the printer has the issue.

## Solution

- Check the Ethernet cable and it was not properly seated with the LED light off, 
- Re-seating the cable restored the internet connection,
- ping  the printer again which was a success,
- restoring access back to the printer.

**Status**: Resolved
