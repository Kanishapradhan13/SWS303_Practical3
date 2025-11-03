# Evaluate Firewall Rules and IDS Alerts for Simulated Attack Traffic

## Environment Setup

### Create Virtual Networks in VirtualBox

Create Host-Only Network:

![alt text](<assets/Screenshot from 2025-11-03 19-41-12.png>)

#### Ubuntu VM (Victim/IDS/Firewall) 

Network Settings:

Adapter 1: Host-only Adapter → vboxnet0
Adapter 2: Internal Network → Name: intnet

![alt text](<assets/Screenshot from 2025-11-03 19-44-32.png>)

![alt text](<assets/Screenshot from 2025-11-03 19-44-43.png>)

![alt text](assets/image.png)

Configure static IPs using Netplan

```ip a``` Verify IPs are assigned

![alt text](<assets/Screenshot from 2025-11-03 20-59-55.png>)

#### Kali VM (Attacker):

Configure network (Kali uses NetworkManager):

![alt text](<assets/Screenshot from 2025-11-03 21-05-30.png>)

### Install and Configure Tools on Ubuntu

Install iptables-persistent

![alt text](assets/image1.png)

Install Snort 3

Snort 3 requires several dependencies

![alt text](assets/image2.png)

















