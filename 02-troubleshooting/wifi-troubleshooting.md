# Wi-Fi Could Not Connect to Network

## Problem
My laptop could see the Wi-Fi network but kept failing to connect. It would prompt for the password repeatedly and never establish a connection.

## Investigation
- Verified that the password was correct.  
- Restarted the laptop and the router to eliminate temporary issues.  
- Checked network adapter settings and drivers.  
- Used `ipconfig` (Windows) / `ifconfig` (Mac/Linux) to inspect IP configuration.  
- Pings to the router failed, indicating a local connectivity issue.  

## Solution
The Wi-Fi adapter was set to **static IP mode** with incorrect gateway information. Switching it to **automatic (DHCP) mode** restored connectivity immediately.

## What I Learned
- Always check whether the adapter is using DHCP or a static IP first.  
- Restarting devices early can save time but may not fix configuration issues.  
- System logs and command-line network tools are invaluable for troubleshooting.  

## What Tools Helped
- `ipconfig` / `ifconfig` to check IP settings  
- Ping to test connectivity  
- Router management interface to verify network configuration  
