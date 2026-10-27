# NETWORKWALKS-B084D-WK1-CYBERSECURITY-LAB-SETUP-SAMPLE

 This project is aimed at creating a virtual machine using  virtual-box  a windows application for creating virtual environments that are used by cybersecurity professionals   to simulate attack's and also test Malwares safely 


 PROJECT OBJECTIVITES 

The following are the objectivates of the project.
1. Download the windows or Mac  set-up files for vitual-box, kali Linux and windows Operating systems
2. install the Virtual-box from the official site
3. configure a private  NAT Network from the Network tab on Virtual-box Application for the cybersecurity-lab
4. Install the Kali on virtual-box
5. configure the Network connectivity for the kali machine ( for set-ups that are 2026 and above )
6. configure the Ip address of the Kali machine 
7. Verify the Network  Connectivity and DNS resolution
8. Take screenshots of the process for recovery
9. Document the complete set-up process
10. Prepare the Set for future Cybersecurity projects



PERPOSE OF THE LAB 
 
The Lab provides the a secure environment  for carrying out Cybersecurity secure testing for the following 

1.  Port scanning
2.  Network Reconance
3.  Malware creation
4.  Packet analysis
5.  Web Security testing  ETC 



LAB ARCHECTURE 


LAB CONFIGURATION 

COMPUTER ----  HP 
HOST OS ----  WINDOWS 10 
HOST RAM ----  16GB 
PROCCESSOR ---- Intel core i5 
Hypervisor----- Virtual-box 
Security OS ---- KALI LINUX 
KALI RAM ------  2048 MB 
VIRTUAL NETWORK --- NAT NETWORK 
NETWORK  ADDRESS ---- 10.0.0.0/24
KALI IP-ADDRESS ---- 10.0.0.2 
DEFLAUT GATEWAY ----- 10.0.0.1
DNS SERVER --- 8.8.8.8
FUTER VM RANGE ---- 10.0.0.3 - 10.0.0.99 



 LAB SET-UP PROCCEDURE 

 1. Download and install 7Zip or WinRAR from their official sites 

 2. Install vitaul-box as your Hypervisor

 3. Create the NAT NETWORK
    Create a edicated  Network   for the virtual-box
    i.e Network Name: NatNetwork IPv4 Prefix: 10.0.0.0/24 DHCP: Enabled IPv6: Disabled

 4. Import Kali Linux
The Kali Linux virtual machine was downloaded from the official Kali Linux website and imported into VirtualBox.

The VM network adapter was configured as follows:

Adapter 1
Attached to: NAT Network    Network:     Nat Network   Adapter Type: Intel PRO/1000 MT Desktop  The VM was allocated:

RAM: 2048 MB

 5. Configure the Kali Linux Network
The Kali Linux network configuration was checked and configured with a consistent IPv4 address.
Example configuration:

IP Address: 10.0.0.2  Subnet Mask: 255.255.255.0   Gateway: 10.0.0.1  DNS: 8.8.8.8



 PROBLEMS ENCOUNTERED DURING THE LAB 

 1. During the installation of the Kali Linux i was expecting  there to be a problem   of network connectivity but suprising'y it was working  perfectly afther the installation
    but incase of the problem occuring please type this code in the terminal.

    sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0
it will solve the problem 
    


 2. Dduring the install of the virtual-box hyper-V  the setup refused to load properly it was due to the fact that my computers Virtualization feature was turn off by default and this is how to fix it in Windows marchines
    1. switch on the windows marchine while pressing the  f10 button
    2. the Bios set-up will load 






    


   
