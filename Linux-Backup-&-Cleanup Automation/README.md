                                  Backup & Automation (Crontab + Cleanup)



## Overview
This project demonstates: 
  - Automated backups using tar.
  - Task scheduling using cron.
  - System cleanup using Bash scripting

## Features
  - Backup user home directory
  - Scheduled backups using cron
  - Automatic cleanup of old backups

### Task A - System Backup Automation

# Step 1: Create a new user (Alice)

A new user account was created with a home directory:

<img width="1012" height="611" alt="image" src="https://github.com/user-attachments/assets/9fd57f97-cfdd-45f5-8beb-44a78f0ef9fb" />

# Step 2: Backup Shell Script (Alice Home Directory)

<img width="1090" height="611" alt="image" src="https://github.com/user-attachments/assets/6b6eec61-ae07-4c6f-9e50-3fe44a6ec4a1" />

<img width="1090" height="611" alt="image" src="https://github.com/user-attachments/assets/384f086c-e78e-49b1-b588-9fbdc7cc33eb" />

# Step 3: Move and Store Backup in /var/backups

<img width="940" height="529" alt="image" src="https://github.com/user-attachments/assets/f08167bd-2fe7-41e3-8b1f-6e7ad0fbc15e" />

<img width="1010" height="611" alt="image" src="https://github.com/user-attachments/assets/5852da9e-4ec6-4eb6-b13b-ddc23e712ce9" />

# Step 4: Stop Crontab Jobs

<img width="1012" height="611" alt="image" src="https://github.com/user-attachments/assets/6dd133de-e04e-407d-8ed5-735d08a1a262" />

### Task B - Cleanup Script

This script ensures that backup storage remains under control by automatically checking the number of backup files and removing older ones when a defined threshold is exceeded.

* Count the number of backup archives created in Task A
* If the number of backups is less than or equal to 3, do nothing
* If the number of backups is greater than 3, delete the oldest backups until only 3 remain

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/438306ab-47cd-4d87-aa4d-45ddcd5b18d8" />

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/4fd77c85-30a6-4672-8009-681f14453296" />

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/7030b94e-1536-45be-a362-caa641868932" />

# Lessons Learned

This lab reinforced practical Linux system administration skills, particularly in automation and system maintenance. I learned how to create and manage Linux users and how user home directories are structured in /home. I gained hands-on experience writing shell scripts that automate repetitive administrative tasks such as system backups. I also learned how to dynamically generate filenames using user input and timestamps to ensure backups are uniquely identifiable. I improved my understanding of Linux file archiving using tar and compression techniques like gzip, which are essential for reducing storage usage while preserving data integrity. Additionally, I learned how to use crontab to schedule recurring tasks and how scheduled jobs can be used to automate real-world system maintenance workflows.
