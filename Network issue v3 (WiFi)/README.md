# Network Issue v3 (Wi-Fi)

**Ticket No:** IT-2026-4318

**Username:** tokoro

**Department:** Sales

**Time Submitted:** 11:05 AM

**Description:** I have not been able connect to the wifi to make use the internet today at all.

**Assigned to:** Eth-steve


### Troubleshooting Guide

It is critical to ask user clarifying questions before assuming a hardware failure.

| Possible Issue | Solution / Action |
| :--- | :--- |
| **Wi-Fi adapter is not on** | Put on the Wi-Fi via the Windows Action Center. |
| **AP is set to "Wi-Fi 6 Only" mode** | The laptop (Wi-Fi 5) cannot see the AP if the AP is configured to reject legacy devices. <br> **Fix:** Log into the AP and enable **"Mixed Mode"** (802.11ax/n/ac) or create a separate SSID for legacy devices. |
| **Driver or Power Management Glitch** | Update the Wi-Fi driver from the manufacturer's site. <br> **Fix:** In Device Manager > Network Adapters, disable "Allow the computer to turn off this device to save power." |
| **Hardware Incompatibility (Rare)** | If the AP is strictly 6 GHz (Wi-Fi 6E) and the laptop lacks a 6 GHz radio, it will not see the network. <br> **Fix:** Connect via Ethernet or connect to the 2.4 GHz/5 GHz band of the AP. |


