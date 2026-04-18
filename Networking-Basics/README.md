                                Networking Basics LAB

## Overview
This covers:
  - IP addressing and subnetting
  - Binary conversation
  - Networking calculations
  - Basic Bash looping

## Task A

| Category | IP Address | Binary Format |
|----------|------------|--------------|
| Address | 192.168.100.4 | 11000000.10101000.01100100.00000100 |
| Network (/28) | 255.255.255.240 | 11111111.11111111.11111111.11110000 |
| Network Address | 192.168.100.0 | 11000000.10101000.01100100.00000000 |
| Broadcast Address | 192.168.100.15 | 11000000.10101000.01100100.00001111 |
| First IP | 192.168.100.1 | 11000000.10101000.01100100.00000001 |
| Last IP | 192.168.100.14 | 11000000.10101000.01100100.00001110 |
| Max Hosts | 14 | |

### Explanation
-  Subnet mask /28 → 4 host bits  
- Total IPs = 2⁴ = 16  
- Usable hosts = 16 - 2 = 14

## Task B

| Category | IP Address | Binary Format |
|----------|------------|--------------|
| Address | 170.1.0.0 | 10101010.00000001.00000000.00000000 |
| Network (/26) | 255.255.255.192 | 11111111.11111111.11111111.11000000 |
| Network Address | 170.1.0.0 | 10101010.00000001.00000000.00000000 |
| Broadcast Address | 170.1.0.63 | 10101010.00000001.00000000.00111111 |
| First IP | 170.1.0.1 | 10101010.00000001.00000000.00000001 |
| Last IP | 170.1.0.62 | 10101010.00000001.00000000.00111110 |
| Max Hosts | 62 | |

### Explanation
-  Subnet mask /26 → 6 host bits  
- Total IPs = 2⁶ = 64  
- Usable hosts = 64 - 2 = 62

Using for loop:
0 1 2 3 4 5 6 7 8 9 10

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/b2aa2f6e-716f-40b2-b56f-b5704a4cb1c3" />

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/e34718e3-dccd-48e3-9683-a348dcca37a1" />

Using while loop:
0 1 2 3 4 5 6 7 8 9 10

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/1da2d6da-1f03-4491-8d1f-8bd80523a027" />

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/96226d51-3083-4145-834a-efe1629b1004" />
