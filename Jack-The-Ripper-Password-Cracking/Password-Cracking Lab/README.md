                              Password Cracking LAB (John the Ripper)

# Password Cracking Lab (John the Ripper)

## Overview
This lab demonstrates password crackig using John the Ripper in a Linux environment.

## Tools used
  - Linux (Ubuntu/Kali)
  - John the Ripper
  - rockyou.txt wordlist

## Tasks
  - Create users and passwords
  - Extract password hashes
  - crack hashes using John the Ripper
  - Analyze results

## Task A
### 1. Create users

    **Six users were created:**

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/718f5b7f-0369-49d0-b063-e45e18e1c245" />

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/f365a3ed-19ef-409e-aa7a-af742d423ced" />

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/828c8925-ead7-4416-8660-a28f61c33eaf" />

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/18d4bb86-47d7-4df0-9317-aa129afaf91a" />

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/15f84657-3759-4078-8cc2-95103e609f33" />

### 2. Extract hashes

**Password hashes were extracted**

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/125b33a1-c92a-4aab-8b35-c25cecc14f57" />

### 3. Run John

**John the Ripper was executed in wordlist mode (use rockyou.txt)**

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/8f9a3faf-448f-4ead-8a2f-9beead35cf24" />

### 4. Show Results

**John the Ripper ran for 10 more mins and cracked no passwords**

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/7f41d37a-2d8f-4d0c-ae03-00f1904229a4" />

#### Results: 
    - Number of passwprds cracked: X/6
    - Cracked passwords: 0

#### Observation:
**Afer re-running John the Ripper, no additional passwords were cracked. This indicates that:**
 - Either the remaining passwords are not in the wordlist.
 - Or they are too complex for wordlist-based attacks.

### 5. Extra Credit

#### MD5 Hash Cracking

### step 1: Save hashes

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/17a08be2-dde1-478d-95c2-1e0b05632678" />

### Step 2: Run John with correct format

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/b44cf7fb-bc71-4c7e-af18-67c7597aae73" />

