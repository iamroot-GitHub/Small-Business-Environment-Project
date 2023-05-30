# Small Business Environment Project
## In this project I worked together with a team to build a small business environment using GNS3 via FortiClient VPN.
### Starting Topology
![Starting Topology](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/9f21529a752862ab05b4f8d11650d52c04a7ffb4/Images/SBE%20Starting%20Topology.png)
### Our team setup the client's network to include a LAN, Guest, and DMZ network (these networks were built on a FortiNet firewall (a FortiGate)).
### We added the following devices to the lab workspace:
1. a FortiNet firewall,
2. two Ethernet switches,
3. and a Win10 workstation.
---
### Device Topology
![SBE Stage 1 Topology Step 1](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/f09713de194f6ce78cd05a4669a69451c6fcffd3/Images/SBE%20Stage%201%20Topology%20Step%201.png)
---
### We linked the following devices in the lab workspace:
![SBE Stage 1 Topology Step 2](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/b5c86f7061868929e135293a00e20a7762f0ea6f/Images/SBE%20Stage%201%20Topology%20Step%202.png)
1. WAN port on the firewall to the WAN-SWITCH,
![SBE Stage 1 Topology Step 3](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/e166ee5785f8f657e7185f423668d92b579fe597/Images/SBE%20Stage%201%20Topology%20Step%203.png)
2. LAN port on the firewall to the LAN-SWITCH,
3. DMZ port on the firewall to the DMZ-SWITCH,
4. and the Win10 workstation to the LAN-SWITCH.
![SBE Stage 1 Topology Step 4](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/a54342c71a3c0cd70210251f5d978146b54bd81a/Images/SBE%20Stage%201%20Topology%20Step%204.png)
---
### After setting up the client's network our team worked together to configure the LAN network by:
1. Configuring the LAN interface,
![SBE Stage 1 Topology Step 4](Images/SBE configured the LAN interface.png)
3. verifying the configuration is correct,
4. configuring the DHCP server for the LAN interface,
5. and verifying the configuration is correct.
