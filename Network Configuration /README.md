                                                Network Configuration 

# Overview

This lab explores Linux networking concepts by comparing Virtual Machine (VM) network configurations in NAT Mode and Bridged Mode. Various networking commands were used to examine IP addressing, routing, DNS resolution, connectivity, and hostname configuration.

Environment: Kali Linux Virtual Machine


## Task A – Explore Network Configurations (NAT Mode)

# Step 1: Display Network Configuration

* Command : ifconfig
  
* IP Address: 192.168.64.2
* MAC Address: fe80::e8f0:2fff:fe00:113a
* Network Mask: 255.255.255.0
  
  <img width="1388" height="784" alt="image" src="https://github.com/user-attachments/assets/0af7cea9-6e0b-46da-9b78-5c7519452c4f" />

# Step 2: Display Routing Table

* Command : route -n

  The routing table shows how network traffic is directed to different destinations and identifies the default gateway used for outbound traffic.

  <img width="1384" height="784" alt="image" src="https://github.com/user-attachments/assets/01047312-abc8-4e6e-af8a-687b1663d78a" />


# Step 3: List Current TCP Connections

* Command : netstat -t

The netstat command displays active TCP connections and provides information about network communication occurring on the system.

<img width="1386" height="784" alt="image" src="https://github.com/user-attachments/assets/67af4b43-5b63-408d-b5f6-54ab28f52f9d" />

# Step 4: Step 4: Test Connectivity to ubuntu.com

* Command : ping -c 10 ubuntu.com

The ping command verifies network connectivity by sending ICMP echo requests to a remote host. Limiting the count to 10 requests allows connectivity testing without continuous transmission.

<img width="1384" height="784" alt="image" src="https://github.com/user-attachments/assets/34089d25-420b-433c-be73-451fe158b021" />

# Step 5: Perform DNS Query

* Command : host www.odu.edu

The host command queries DNS servers to resolve domain names into IP addresses. 

<img width="1388" height="622" alt="image" src="https://github.com/user-attachments/assets/c4e6489e-ce2a-4b53-bd14-2014a3ff3305" />

# Step 6: Display System Hostname

* Command : cat /etc/hostname

The /etc/hostname file contains the permanent hostname assigned to the Linux system.

<img width="1390" height="782" alt="image" src="https://github.com/user-attachments/assets/805bcac3-748c-438e-8718-6310f0708ab8" />

# Step 7: Display DNS Server Configuration
 
* Command : cat /etc/resolv.conf

The /etc/resolv.conf file contains the DNS server information used by the system for name resolution.

<img width="1392" height="588" alt="image" src="https://github.com/user-attachments/assets/4e316196-4c59-4ea6-858f-d08d91693512" />

# Step 8: Change Hostname Permanently

* Command : sudo nano /etc/hostname

Changing the hostname permanently allows the system to identify itself using the specified MIDAS ID after every reboot.

<img width="1392" height="786" alt="image" src="https://github.com/user-attachments/assets/ba75bd83-b4a3-42eb-8267-f280f7b5c2d7" />




## Task B – Different Network Setting (Bridged Mode)

# Step 1: Display Network Configuration

* Command : ifconfig

* IP Address: 192.168.8.102
* MAC Address: fe80::e8f0:2fff:fe00:113a
* Network Mask: 255.255.255.0

The IP address changed because the VM became part of the same physical network as the host computer. In bridged mode, the VM receives an IP address directly from the network's DHCP server rather than from VirtualBox's internal NAT network.

<img width="1396" height="788" alt="image" src="https://github.com/user-attachments/assets/53b5c209-1e5e-4f9e-b498-46ac3ec06a35" />

# Step 2: Display Routing Table

* Command : route -n

The default gateway changed to match the gateway of the physical network.

This confirms that the VM is communicating directly with the local network instead of using the virtual NAT gateway.

<img width="1396" height="790" alt="image" src="https://github.com/user-attachments/assets/04338e76-9bc1-4f73-a13a-40f0335da3e0" />

# Step 3: List Current TCP Connections

* Command : netstat -t

The active TCP connections were generally similar, although network traffic may vary depending on background services and current activity.

TCP connections depend more on running services and applications than on the network mode itself.

<img width="1390" height="662" alt="image" src="https://github.com/user-attachments/assets/d856bea4-5746-4698-a746-e69ba4ce7550" />

# Step 4: Test Connectivity to ubuntu.com

* Command : ping -c 10 ubuntu.com

Both NAT and Bridged modes achieved a 100% success rate with no packet loss.

Both configurations successfully provided Internet connectivity. Minor differences in response times were observed, but overall network performance was similar.

<img width="1388" height="786" alt="image" src="https://github.com/user-attachments/assets/57941a5b-6c26-40e7-a6d8-216658e8d175" />

# Step 5: Perform DNS Query

* Command : host www.odu.edu

The resolved IP address remained the same in both network configurations.

DNS resolution produced identical results because both configurations queried valid DNS servers for the same domain name.

<img width="1392" height="668" alt="image" src="https://github.com/user-attachments/assets/8fb8b9ff-7e81-476a-98b8-5b550ee52309" />

# Step 6: Display System Hostname

* Command : cat /etc/hostname

No differences were observed.

The hostname is a local system configuration and is not affected by the VM network mode.

<img width="1392" height="630" alt="image" src="https://github.com/user-attachments/assets/9c72d1f4-90b0-45ac-9acd-3d1f14085e48" />

# Step 7: Display DNS Server Configuration

* Command : cat /etc/resolv.conf

The DNS server addresses were different from those used in NAT mode.

In bridged mode, the VM receives DNS information directly from the physical network, whereas NAT mode often uses DNS servers provided by the virtualization software.

<img width="1392" height="834" alt="image" src="https://github.com/user-attachments/assets/3a301188-97d8-4c51-9095-dd4466f21e71" />

# Lessons Learned

This lab improved my understanding of Linux networking and virtual machine network configurations. I learned how to use commands such as ifconfig, route, netstat, ping, host, and cat to gather information about network interfaces, routing, DNS resolution, and connectivity. I also learned how to locate and modify important system files such as /etc/hostname and /etc/resolv.conf.

By comparing NAT and Bridged networking modes, I observed that the IP address and default gateway changed when the VM joined the physical network through bridged mode. However, the MAC address and subnet mask remained unchanged. I also learned that DNS server configurations can differ between network modes while still providing successful name resolution. Overall, this lab strengthened my practical understanding of Linux networking concepts and virtual machine network management.
