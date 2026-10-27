#Cybersecurity Lab Environment SetupBuilding an isolated virtual lab for penetration testing and ethical hacking practice

**Project Overview**
This project focuses on setting up a virtual cybersecurity and penetration-testing laboratory using VirtualBox and Kali Linux. The purpose of the lab is to create a controlled environment where cybersecurity tools, network scanning, reconnaissance, vulnerability assessment, and other security-testing activities can be performed safely and repeatedly. The lab is configured on a private virtual network so that additional machines can be added later and used as targets for authorized security testing.  

**Lab Configuration Steps**
1. Virtual Network: Created a VirtualBox NATNetwork using the 10.0.0.0/24 subnet.   
2. Kali Linux Installation: Imported the pre-built Kali Linux virtual machine and attached its network adapter to the new NATNetwork.   
3. VM Settings: Enabled Promiscuous Mode, bidirectional shared clipboard, and file drag/drop.   
4. Shared Folders: Linked the host machine's /downloads folder with full access and auto-mount enabled.   
5. IP Configuration: Manually assigned the Kali Linux IP address to 10.0.0.2/24 with a gateway of 10.0.0.1 and DNS set to 8.8.8.8.  
6. Finalization: Tested external internet connectivity and took a baseline snapshot of the virtual machine.  
