# Network Issue v4 (Wi-Fi) - MTN ZLT X100M PRO(Personal Device)

**Subject:** I cannot see the Wi-Fi network on my router, while other can.  

**Ticket No:** IT-2026-4425

**Username:** Mr. James  

**Department:** Admin

**Time Submitted:** 03:40 PM

**Description:** I recently purchased the MTN 5G Ultrafast Router (ZLT X100M PRO) but i have not been able to connect to it, i cant even see the name of the wifi, can you help with this? 

**Assigned to:** Eth-steve


### Root Cause
The router is broadcasting in a **Wi-Fi 6 (802.11ax) Exclusive** mode or using a channel width incompatible with the older laptop's Wi-Fi 5 NIC. This setting is located in the **Advanced** wireless menu, not the basic SSID page.

### Step-by-Step Resolution

1.  **Access Router Admin Panel**
    *   Open browser: `http://192.168.1.1` (or check router sticker).
    *   Login with admin credentials.

2.  **Navigate to Advanced Wireless Settings**
    *   **Do NOT** stop at the basic "Wi-Fi Settings" or "SSID" page.
    *   Go to **Advanced** > **Wireless** (or **Wi-Fi Advanced**).
    *   Select the **2.4 GHz** tab (and **5 GHz** if the issue persists there).

3.  **Change Wireless Mode (The Critical Fix)**
    *   Locate **Wireless Mode** (sometimes labeled "Protocol" or "Mode").
    *   **Current Setting:** Likely `802.11ax Only` or `Wi-Fi 6 Only`.
    *   **Action:** Change to **Mixed Mode**.
    *   **Specific Selection:** Select **`802.11b/g/n/ax`**.
        *   *Key:* Ensure **`b/g`** is included in the list. This forces legacy beacons.
    *   *Note:* If `ax` is not an option in the dropdown, select `802.11n/g` to force legacy mode temporarily for testing.

4.  **Adjust Channel Width (If available in Advanced)**
    *   Set **Channel Width** to **20/40 MHz** (Auto) or **20 MHz**.
    *   Avoid **80 MHz** or **160 MHz** on 2.4 GHz.

5.  **Save and Reboot**
    *   Click **Save/Apply**.
    *   **Reboot the Router** (Power cycle) to ensure the radio restarts in the new mode.

6.  **Verify on Laptop**
    *   Toggle Airplane Mode ON/OFF on the laptop.
    *   The SSID should now appear. Connect and test.

### Summary for Ticket Closure
> "The issue was caused by the MTN ZLT X100M PRO router broadcasting in Wi-Fi 6 exclusive mode.

> The fix required navigating to **Advanced > Wireless Settings**, changing the **Wireless Mode** from `802.11ax Only` to **`802.11b/g/n/ax`** (Mixed Mode),

> rebooting the router. The legacy laptop can now detect and connect to the AP."
