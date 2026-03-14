# What Happens When a Device Connects to Wi-Fi

## Overview
Connecting to Wi-Fi allows a device to communicate with a wireless network and access the internet. 
This process involves scanning for networks, authenticating, and establishing a secure connection so data can be transmitted safely.

## Steps
1. **Device scans for available networks** – The Wi-Fi adapter searches for nearby access points and lists them.  
2. **User selects a network** – The device chooses the SSID (network name) to connect to.  
3. **Authentication and encryption negotiation** – Device and router exchange credentials (password or enterprise authentication) and agree on encryption protocols (WPA2/WPA3).  
4. **DHCP request** – Device requests an IP address from the network’s DHCP server.  
5. **IP address assigned** – DHCP server assigns an IP address, subnet mask, and gateway.  
6. **Device joins the network** – Network parameters are applied, and the device is now connected.  
7. **Network readiness check** – Device tests connectivity, often by pinging a server or checking for internet access.  

## Operational/Security Considerations
- **Strong Wi-Fi password** prevents unauthorized access.  
- **WPA2/WPA3 encryption** protects data in transit.  
- **MAC filtering** or network segmentation improves security.  
- **Auto-connect settings** can be a risk if devices connect to rogue networks.  

## How This Breaks or Gets Attacked
- **Incorrect password** or misconfigured security settings prevent connection.  
- **DHCP failure** can block network access.  
- **Rogue access points** could trick devices into connecting (evil twin attacks).  
- **Packet sniffing** could capture unencrypted traffic if security is weak.  
