                                      Group and Users Accounts 

This lab focuses on basic Linux user and group management. It covers creating user accounts, managing passwords, assigning groups, and modifying group ownership. The tasks were performed in a Linux virtual machine environment and reflect practical system administration skills.



# Task A: User Account Management

### 1. Display Current User Account information

<img width="1168" height="611" alt="image" src="https://github.com/user-attachments/assets/0aa912ce-d959-4a47-aac9-add3d407dfc1" />

### 2. Display password information for current user

<img width="1012" height="611" alt="image" src="https://github.com/user-attachments/assets/c074e361-a47e-43cd-82c2-c0376b023ff4" />

### 3. Create a new user

<img width="1013" height="611" alt="image" src="https://github.com/user-attachments/assets/d0a708f1-1a0f-426e-8de4-845ef7ab6132" />

### 4. Set password

<img width="1088" height="611" alt="image" src="https://github.com/user-attachments/assets/ff18d001-224d-446a-bb36-f17edaa4894f" />

### 5. Set default shell to bash

<img width="1010" height="611" alt="image" src="https://github.com/user-attachments/assets/4947aa4d-17c1-433d-9150-d171cc25e39d" />

### 6. Display password info for new user

<img width="1088" height="611" alt="image" src="https://github.com/user-attachments/assets/a56485bb-5524-4659-b6cd-7a0d8e70dce7" />

### 7. Add user to sudo group

<img width="1013" height="611" alt="image" src="https://github.com/user-attachments/assets/3920a747-4897-4d52-a5ec-c8662755e3d0" />

### 8. Switch to new user

<img width="1009" height="611" alt="image" src="https://github.com/user-attachments/assets/c4ee238e-14bb-4437-8199-0a361ffc2e26" />


# Task B - Group Account Management 

### 1. Check current shell

<img width="1087" height="611" alt="image" src="https://github.com/user-attachments/assets/d19b2b2d-2171-4b6a-b38e-56c2cd27b516" />

### 2. Display user ID and groups

<img width="1012" height="611" alt="image" src="https://github.com/user-attachments/assets/41414bf6-57f6-44c7-a6f5-5a7f172a8009" />

### 3. Display root group membership

<img width="1012" height="611" alt="image" src="https://github.com/user-attachments/assets/4f4650b1-61bc-46d1-88f5-32cdc79969b1" />

### 4. Check ownership of /etc/group

<img width="1085" height="611" alt="image" src="https://github.com/user-attachments/assets/b4d34931-ce42-406e-827d-c09ad0607813" />

### 5. Create new group

<img width="1009" height="611" alt="image" src="https://github.com/user-attachments/assets/c60c75f2-7ceb-4491-b61c-2b67bd31bb20" />

### 6. Display group info

<img width="1013" height="611" alt="image" src="https://github.com/user-attachments/assets/62e664aa-a3ea-4267-94af-02dd34562bf4" />

### 7. Rename group

<img width="1085" height="611" alt="image" src="https://github.com/user-attachments/assets/3cf0b6fb-11cc-4493-8309-8fe8f44252ff" />

### 8. Add user to group

<img width="1012" height="611" alt="image" src="https://github.com/user-attachments/assets/31bf78d5-c77e-4c42-a7a8-fdf18a0cd6f5" />

### 9. Create file and change group owner

<img width="1013" height="611" alt="image" src="https://github.com/user-attachments/assets/e475176c-0b68-40ff-a418-83a3f4154bea" />

### 10. Verify ownership

<img width="1012" height="611" alt="image" src="https://github.com/user-attachments/assets/a17876fc-03f9-40a2-be60-1759dc69e325" />

### 11. Delete group and observe result

<img width="1246" height="611" alt="image" src="https://github.com/user-attachments/assets/0b5f1174-804e-4d97-bbda-511e645eec3f" />

**Observation: After deleting the group, the file still exists but the group owner is displayed as the old GID instead of a group name**

### 12. Delete user and home directory

<img width="1235" height="611" alt="image" src="https://github.com/user-attachments/assets/b1365270-fe3e-49e4-827c-6947c10d9b3f" />

# Lesson Learned 

I learned that Linux stores user details in /etc/passwd and password hashes in /etc/shadow, both of which require elevated permissions to access. Creating users with useradd -m automatically generates a home directory, while usermod -s allows changing the user’s default shell and affects how they interact with the system. I also learned that group management commands like groupadd, groupmod, and groupdel directly impact file ownership and system permissions. Using -aG is important because it adds users to groups without removing existing memberships. Finally, I understood that deleting a group can leave files with orphaned group information, and that userdel -r properly removes both a user account and their home directory.
