# ARP-Attack-and-Network-Sniffing
# Explore Network Sniffing and ARP Attacks

# AIM:

To explore network sniffing and ARP Attacks

## STEPS:

### Step 1:

Install Parrot Security OS either in a partition, VirtualBox or in live mode.



### Step 2:

Investigate the various categories of network security tools available in Parrot OS, such as:

arpspoof
dsniff
Metasploit Framework
Wireshark
Ettercap
tcpdump


### Step 3:
Open the terminal and execute some Parrot OS commands.
```
cat /etc/os-release
ip addr
ip route
ip neigh
ifconfig
```

## ARP Attacks:  
ARP spoofing: A hacker sends fake ARP packets that link an attacker's MAC address with an IP of a computer already on the LAN. 
Boot kali and Windows7 virtual machines.
In windows 7 give the command arp -a
```
ipconfig
arp -a
```
## OUTPUT:
<img width="800" height="600" alt="VirtualBox_WIN7_25_11_2026_10_26_18" src="https://github.com/user-attachments/assets/fdede015-dbee-4b5c-b159-5eef240d493b" />


From Parrot OS, identify the active network interface using:
```
ifconfig

```
## OUTPUT:

<img width="955" height="533" alt="image" src="https://github.com/user-attachments/assets/06231e45-4709-4194-a496-706212a24171" />


Examine the ARP neighbor table using:
```
ip neigh
```

## OUTPUT:
<img width="461" height="89" alt="image" src="https://github.com/user-attachments/assets/c55bcce4-d919-4ed1-9ecc-cc6533c850c8" />


Check the routing information using:
```
ip route
```
## OUTPUT:

<img width="404" height="76" alt="image" src="https://github.com/user-attachments/assets/59363fee-4d14-4115-87ed-a5e9e7a280dc" />

ARP spoofing concepts and their effects on IP-to-MAC address mappings were studied in an isolated virtual network.


 dsniff:
 
dsniff is a collection of network auditing and traffic analysis tools used to examine network traffic.

Install dsniff using:
```
sudo apt update
sudo apt install dsniff -y
```
Check the available utilities using:
```
dsniff -h
dpkg -L dsniff
```
## OUTPUT:

<img width="610" height="434" alt="image" src="https://github.com/user-attachments/assets/17511c61-3f83-4d85-a391-f3f1543ca9df" />

Metasploit Framework:
Metasploit is a penetration-testing framework used for security testing and vulnerability assessment.

Open Metasploit using:
```
msfconsole
```
## OUTPUT:
<img width="577" height="485" alt="image" src="https://github.com/user-attachments/assets/c2a555db-0d10-48f1-b909-0731d9889cf5" />


Search for FTP-related auxiliary modules using:
```
search type:auxiliary ftp
```
## OUTPUT:
<img width="959" height="539" alt="image" src="https://github.com/user-attachments/assets/7a5e9d02-4d44-418a-b4f0-8a883ec65e43" />

Examine FTP service identification modules.


Wireshark:
Wireshark is a network protocol analyzer used to capture and examine network packets.

Invoke Wireshark using:
```
sudo wireshark
```
## OUTPUT:

<img width="959" height="501" alt="image" src="https://github.com/user-attachments/assets/609080bb-520f-4aae-8a04-6e09964c5346" />


Examine the various menus, controls, packet details and protocol information available in Wireshark.

## OUTPUT:
<img width="872" height="399" alt="image" src="https://github.com/user-attachments/assets/1774194f-db7b-4a81-b11a-65f32f9dfa23" />


ARP packet:
<img width="959" height="539" alt="image" src="https://github.com/user-attachments/assets/95fc3ae9-a688-411c-a2f0-c93d6ccd52b0" />


Ettercap:
Ettercap is a network security tool that supports active and passive network analysis and host discovery.

Open Ettercap using:
```
sudo ettercap -G
```
Explore the following menus:

Sniff
Hosts
Targets
View
Plugins
Examine the graphical interface and network analysis features.

## OUTPUT:
<img width="956" height="539" alt="image" src="https://github.com/user-attachments/assets/af18897e-7f9a-4d9a-9f1d-de3a7c2c3173" />

tcpdump:
tcpdump is a command-line network packet analyzer used to capture and examine network traffic.

Check the installed version using:
```
tcpdump --version
```
Examine the available network interfaces using:
```
sudo tcpdump -D
```
## OUTPUT:

<img width="516" height="384" alt="image" src="https://github.com/user-attachments/assets/eb5d40f3-d15f-4ed5-a884-a3c36755ca0e" />

Capture ARP packets on the active interface using:
```
sudo tcpdump -i enp0s3 arp
```
Stop packet capturing using Ctrl + C.

## OUTPUT:
<img width="619" height="405" alt="image" src="https://github.com/user-attachments/assets/d4be3c85-b16c-4ea7-b96d-54818cbd7351" />



## RESULT:
Thus, the network security and network sniffing tools available in Parrot OS, including arpspoof, dsniff, Metasploit, Wireshark, Ettercap and tcpdump, were explored successfully. The concepts of ARP attacks, ARP tables, network interfaces and packet analysis were studied.
