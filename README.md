# Small Business Environment Project
## In this project I worked together with a team to build a small business environment using GNS3 via FortiClient VPN.
### Beginning Network Topology
![SBE Beginning Network Topology](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/9f21529a752862ab05b4f8d11650d52c04a7ffb4/Images/SBE%20Starting%20Topology.png)
### Complete Network Topology
![SBE Complete Network Topology](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/3a4b818e3857098b965f8ec363e8480c1daf7d3f/Images/SBE%20Complete%20Network%20Topology.png)
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
![SBE configured the LAN interface](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/2ed1f4f1115ca96a76dcb47c398877cffe4a4dde/Images/SBE%20configured%20the%20LAN%20interface.png)
2. verifying the configuration is correct,
![SBE verified the correct LAN interface configuration](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/33d112a03bb928ba2af1d0fa924b0d34c9f498b5/Images/SBE%20verified%20the%20correct%20LAN%20interface%20configuration.png)
3. configuring the DHCP server for the LAN interface,
![SBE configured the DHCP server for the LAN interface](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/c27acebb51fc936019e32b15ad8dba75823acb0e/Images/SBE%20configured%20the%20DHCP%20server%20for%20the%20LAN%20interface.png)
4. and verifying the configuration is correct.
![SBE verified the correct DHCP server LAN interface](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/8f7ba1dcc79c3f4710b4d38828b151ab51774e88/Images/SBE%20verified%20the%20correct%20DHCP%20server%20LAN%20interface.png)
