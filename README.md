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

![](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/0963a33103d695a9205395733f17539f7f6947a0/Images/SBE_03.png)

2. configured the LAN network on the firewall through the CLI over the console interface,

![SBE Configured the LAN Network](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/3955adc2f427930985298865819c23472dc5139f/Images/SBE_04.png)

3. added a Win10 workstation to the LAN network,
4. connected to the firewall GUI from the Win10 workstation,
5. and completed the network setup through the firewall GUI.

![SBE Network Setup Firewall GUI](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/7cab93119258ed0c5b261b81c5ba9933e70da87b/Images/SBE_05.png)
### In stage 2 we built a Windows domain on Windows Server 2012r2 as follows:
1. added a Win2012r2 server to the network and linked it up,
2. prepared the Win2012r2 server for the "Active Directory Domain Services" server role,

![SBE Prepared Win2012r2 Server](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/a76e02741b62d6d5f5391688a91c0690180cdb2e/Images/SBE_06.png)

3. installed the "Active Directory Domain Services" server role,
4. created new Active Directory user accounts,

![SBE Created AD Users](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/53474993ac5568dda9dcd59cd504143ed8bc4406/Images/SBE_07.png)

5. prepared the Win10 workstation to join the domain,
6. joined the Win10 workstation to the domain,

![SBE Joined Win10 to the Domain](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/93088cc0d62fee41858fd088e1a2914f7a90a885/Images/SBE_08.png)

7. and set the desktop background on Win10 with the group policy from the Domain Controller.

![SBE Desktop Background](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/c589105101eb736be4de4a9befeb894c73ea46d8/Images/SBE_09.png)
### In stage 3 we built an Internet Information Services (IIS) webserver on a Win2012r2 server and joined the server to the domain as follows:
1. added a Win2012r2 server to the network and linked it up,
2. prepared the Win2012r2 server to join the domain,
3. installed the "IIS" server role,

![SBE IIS Server Role](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/7570a8600b6f0d7844f6f35090818a7298c22576/Images/SBE_10.png)

4. added a test webpage,

![SBE Test Webpage](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/30e78fd6696c7eb3c79d04a83db4282cd8e9b6ee/Images/SBE_11.png)

5. and verified access over the LAN network.

![SBE Verified Access](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/30e78fd6696c7eb3c79d04a83db4282cd8e9b6ee/Images/SBE_11.png)
### In stage 4 we built a LAMP (Linux, Apache, MySQL, PHP/Perl/Python) webserver on Ubuntu server over the DMZ network as follows:
1. added an Ubuntu server to the network and linked it up,
2. prepared the Ubuntu server,

![SBE Prepared Ubuntu Server_01](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/49276f33336505f10d1977e4506c9ccbc840fc3f/Images/SBE_13.png)
![SBE Prepared Ubuntu Server_02](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/2babbdd0f8646d7793106ca4ddf368a020417641/Images/SBE_14.png)

3. installed DokuWiki,

![SBE Installed DokuWiki](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/4f8cce61c751bb82b0473595263d659eb7b047f1/Images/SBE_15.png)

4. configured DokuWiki,

![SBE Configured DokuWiki_01](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/f20d0aa1de61f6926e46abe436f5565dee3ea182/Images/SBE_16.png)
![SBE Configured DokuWiki_02](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/e43d0270bfc65583bbaa049534c530b54b3454b8/Images/SBE_17.png)

5. and setup a Virtual IP (VIP) for the public side of the webserver on the firewall.

![SBE Setup VIP](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/583839e557f73097ce8c757f441a238d7efc03a1/Images/SBE_18.png)
### In stage 5 we built a File Transfer Protocol (FTP) server on a Win2012r2 server on the DMZ network as follows:
1. added a Win2012r2 server to the network and linked it up,
2. prepared the Win2012r2 server,
3. and installed the FTP service.

![SBE Installed FTP_01](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/469b83f9a55e68d6a8a3d666e6b2b48ca2991407/Images/SBE_19.png)
![SBE Installed FTP_02](https://github.com/iamroot-GitHub/Small-Business-Environment-Project/blob/93bfefd499abc13bf371d452eea39cd6d68f2195/Images/SBE_20.png)
![SBE Installed FTP_03]
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
