                              Linux User & Permission Management LAB

# Linux User & Permission Management Lab

## Overview
**This Lab demonstates Linux user management, group permissions, SGID, and Sticky Bit concepts.**

## Topics Covered
  - User and group creation
  - File permissions (chmod, umask)
  - Shared directories
  - SGID (Set Group ID)
  - Sticky Bit

## Task A: Get Accounts and Groups Ready

### Step 1: Create Groups

<img width="1085" height="611" alt="image" src="https://github.com/user-attachments/assets/1da2a904-c540-4a5e-a706-49a7c9489857" />

### Step 2: Create Users

<img width="1082" height="611" alt="image" src="https://github.com/user-attachments/assets/b48e18d7-258e-44e9-9b0f-af5cd3ce9989" />

<img width="1080" height="611" alt="image" src="https://github.com/user-attachments/assets/b927732e-d68d-4aa5-9667-2196ada9c8c5" />

### Step 3: Create Shared Group

<img width="1082" height="611" alt="image" src="https://github.com/user-attachments/assets/ee0b7e6d-fd78-4f40-875b-7033275fbdb5" />

### Step 4: Create Shared Directory

<img width="1093" height="611" alt="image" src="https://github.com/user-attachments/assets/2362c148-0717-4e15-88f4-e2913a4556b5" />

### Step 5: Get Permissions

<img width="1085" height="611" alt="image" src="https://github.com/user-attachments/assets/03b6279c-9ba9-482d-bd57-c15493742a3f" />

### Step 6: Set umask for Sophia

<img width="1082" height="611" alt="image" src="https://github.com/user-attachments/assets/8965ce4e-46e9-4332-a2bd-eace545c33f2" />

### Step 7: Create File

<img width="1082" height="611" alt="image" src="https://github.com/user-attachments/assets/c3daf010-7e01-437f-94e6-7427287d77e0" />

### Step 8: Copy File

<img width="1084" height="611" alt="image" src="https://github.com/user-attachments/assets/2a14dd48-c181-4187-ba95-ba6e1b1de294" />

### Step 9: Emma Access Test

<img width="1082" height="611" alt="image" src="https://github.com/user-attachments/assets/66e82137-5dc1-4e54-91bf-7ee04d529934" />

### Step 10: Exit Users

<img width="1082" height="611" alt="image" src="https://github.com/user-attachments/assets/a5ab8a9a-419e-4d4a-9cc3-bc65c6272040" />

## Task B: Set SGID Permission

### Step 1: Enable SGID

<img width="1091" height="611" alt="image" src="https://github.com/user-attachments/assets/e0e63f56-1cbb-4a72-be34-dd72b73f08f8" />

### Step 2: Sophia Copies File

<img width="1079" height="611" alt="image" src="https://github.com/user-attachments/assets/298a27b4-0054-4540-a0b5-5848a0d855a7" />

### Step 3: Emma Reads File

<img width="1085" height="611" alt="image" src="https://github.com/user-attachments/assets/9ea84f38-bef3-4347-a20b-5e9d5b031f50" />

## Task C: Unset SGID

### Step 1: Remove SGID

<img width="1085" height="611" alt="image" src="https://github.com/user-attachments/assets/c4d875fe-d5f1-4ed3-8903-4b334176fe6b" />

### Step 2: Sophia Copies Again

<img width="1090" height="611" alt="image" src="https://github.com/user-attachments/assets/59e333ae-beaa-40b9-b213-86655a916c29" />

### Step 3: Olivia Test

<img width="1087" height="611" alt="image" src="https://github.com/user-attachments/assets/d2ba3581-6abf-4393-812f-d65887896560" />

### Extra Credit: Sticky Bit

### Step 1: Olivia Deletes File

<img width="1087" height="611" alt="image" src="https://github.com/user-attachments/assets/7b1b053a-94e4-4788-a784-8794a1f267dd" />

<img width="1084" height="611" alt="image" src="https://github.com/user-attachments/assets/d8478e8a-812e-43e2-b36a-550dcedbdcc9" />

### Step 2: Set Sticky Bit

<img width="1088" height="611" alt="image" src="https://github.com/user-attachments/assets/e0992a48-f4c3-40c3-85de-4eeea33f3697" />

### Step 3: Olivia Tries Again

<img width="1084" height="611" alt="image" src="https://github.com/user-attachments/assets/0e019e93-9f92-49ad-bb00-1af1d8386556" />

# Lessons Learned

This lab helped me understand how Linux manages users, groups, and file permissions in a multi-user environment. I learned that creating users and groups is important for organizing access and controlling collaboration between different accounts.

I also gained hands-on experience with file permissions using chmod, which showed how read, write, and execute permissions directly affect what users can do with files and directories. Setting up shared directories reinforced how group ownership is essential for controlled collaboration.

The SGID permission helped me understand how files created inside a directory can automatically inherit the group ownership, making teamwork more consistent. In contrast, the Sticky Bit showed how shared directories can be protected so that only file owners can delete their files, even when others have write access.

Finally, adjusting umask helped me see how default file permissions are determined when new files are created. Overall, this lab strengthened my understanding of Linux permission management and how it is used to improve both security and collaboration.
