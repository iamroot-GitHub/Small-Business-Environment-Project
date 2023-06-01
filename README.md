# Small Business Environment Project
## In this project I worked together with a team of five personnel and a senior engineer to build a small business environment using GNS3 via FortiClient VPN.
### Beginning Network Topology
![SBE Beginning Network Topology](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/a2fc6ae6a7627953cb600a328a8982f625fc734c/Images/SBE_01.png)
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
![SBE Complete Network Topology](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/919126fd464dd7e5116256a2d025e637d6a9d3d4/Images/SBE_02.png)
---
### The team completed the small business environment in stages.
### In stage 1 we built out the network infrastructure as follows:
1. added a LAN, GUEST, and DMZ network, and linked them up,
2. configured the LAN network on the firewall through the CLI over the console interface,
![SBE Configured the LAN Network](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/3955adc2f427930985298865819c23472dc5139f/Images/SBE_04.png)
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
### In stage 6 we researched vendor and other industry sources on hardening our network and documented our findings via a wiki page as follows:
1. added a page for notes in the wiki,
2. researched hardening a FortiGate firewall,
3. researched hardening a Windows 10 workstation,
4. researched hardening a Windows Server 2012r2,
5. researched hardening a Ubuntu Server 18.04,
6. documented our research in the wiki notes page,
![SBE Widget.localdomain Wiki Hardening Notes](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/9a05abc427101c8d40e51c0a1c3c148dfc488959/Images/SBE%20Widgets.localdomain%20Wiki%20Hardening%20Notes.png)
7. and presented our findings to the senior engineer.
### As a bonus we scanned our wide area network (WAN) interface and documented our findings via a wiki page as follows:
1. added a page for notes in the wiki,
2. connected to our group's Greenbone server,
![SBE Greenbone Security Assistant Dashboards](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/93dea35e732abb7dcfda3a5e277f8f53deadddec/Images/SBE%20Greenbone%20Security%20Assistant%20Dashboards.png)
3. created a target of the WAN interface IP for the firewall,
4. scanned the target,
![SBE Greenbone Security Assistant Vulnerabilities](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/ff3a110369ed3918289d393bf4d77421f95ca592/Images/SBE%20Greenbone%20Security%20Assistant%20Vulnerabilities.png)
5. documented our scan in the wiki notes page,
![SBE Widgets.localdomain Wiki Greenbone Results](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/ab67fbd3444ab36550fd599aa69ba67c31eb237d/Images/SBE%20Widgets.localdomain%20Wiki%20Greenbone%20Results.png)
6. and presented our findings to the senior engineer.
