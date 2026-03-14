# VM Could Not Reach the Internet

## Problem
A virtual machine had an IP address but could not access external websites or ping outside hosts.

## Investigation
- Verified VM IP configuration using `ipconfig`.  
- Checked host machine’s internet connectivity.  
- Inspected VM network adapter settings in the virtualization software.  
- Tried pinging the default gateway and DNS servers.

## Solution
The VM network adapter was set to **“Host-Only” mode** instead of **NAT**. Changing it to NAT allowed the VM to access the internet.

## What I Learned
- Always check virtualization network mode before troubleshooting higher network layers.  
- IP addresses alone don’t guarantee connectivity; adapter mode matters.  
- Keeping virtualization software updated prevents unexpected network bugs.

## What Tools Helped
- `ipconfig` / `ifconfig`  
- VM network adapter settings  
- Ping command  
