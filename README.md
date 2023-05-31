# Small Business Environment Project
## In this project I worked together with a team of five personnel and a senior engineer to build a small business environment using GNS3 via FortiClient VPN.
### Beginning Network Topology
![SBE Beginning Network Topology](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/9f21529a752862ab05b4f8d11650d52c04a7ffb4/Images/SBE%20Starting%20Topology.png)
### The client that our Managed Service Provider (MSP) was hired by requested the following:
1. a secure network,
2. an internal Windows Domain,
3. an internal Microsoft IIS webserver,
4. an internal Windows 10 workstation,
5. a public webserver,
6. a public FTP server,
7. a LAN network on a specified IP address,
8. a DMZ network on a specified IP address,
9. and a GUEST network on a specified IP address.
### Complete Network Topology
![SBE Complete Network Topology](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/3a4b818e3857098b965f8ec363e8480c1daf7d3f/Images/SBE%20Complete%20Network%20Topology.png)
---
### The team completed the small business environment in stages.
### In stage 1 we built out the network infrastructure as follows:
1. added a LAN, GUEST, and DMZ network, and linked them up,
2. configured the LAN network on the firewall through the CLI over the console interface,
3. added a Win10 workstation to the LAN network,
4. connected to the firewall GUI from the Win10 workstation,
5. and completed the network setup through the firewall GUI.
### In stage 2 we built a Windows domain on Windows Server 2012r2 as follows:
1. added a Win2012r2 server to the network and linked it up,
2. prepared the Win2012r2 server for the "Active Directory Domain Services" server role,
3. installed the "Active Directory Domain Services" server role,
4. created new Active Directory user accounts,
5. prepared the Win10 workstation to join the domain,
6. joined the Win10 workstation to the domain,
7. and set the desktop background on Win10 with the group policy from the Domain Controller.
### In stage 3 we built an Internet Information Services (IIS) webserver on a Win2012r2 server and joined the server to the domain as follows:
1. added a Win2012r2 server to the network and linked it up,
2. prepared the Win2012r2 server to join the domain,
3. installed the "IIS" server role,
4. added a test webpage,
5. and verified access over the LAN network.
### In stage 4 we built a LAMP (Linux, Apache, MySQL, PHP/Perl/Python) webserver on Ubuntu server over the DMZ network as follows:
1. added an Ubuntu server to the network and linked it up,
2. prepared the Ubuntu server,
3. installed DokuWiki,
4. configured DokuWiki,
5. and setup a Virtual IP (VIP) for the public side of the webserver on the firewall.
### In stage 5 we built a File Transfer Protocol (FTP) server on a Win2012r2 server on the DMZ network as follows:
1. added a Win2012r2 server to the network and linked it up,
2. prepared the Win2012r2 server,
3. and installed the FTP service.
### In stage 6 we researched vendor and other industry sources on hardening or network and documented our findings via a wiki page as follows:
1. added a page for notes in the wiki,
2. researched hardening a FortiGate firewall,
3. researched hardening a Windows 10 workstation,
4. researched hardening a Windows Server 2012r2,
5. researched hardening a Ubuntu Server 18.04,
6. documented our research in the wiki notes page,
7. and presented our findings to the senior engineer.
