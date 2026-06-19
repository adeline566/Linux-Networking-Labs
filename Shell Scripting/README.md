                              Bash Scripting LAB



## Overview

This lab focused on creating and executing Bash shell scripts in Linux to automate common administrative tasks. The exercises covered conditional statements, file and directory validation, file creation, and displaying directory contents.

## Task A: Conditional Statements

# Objective

Create a shell script that:

* Uses the Bash shebang (#!/bin/bash)
* Reads a number from the user
* Checks whether the number is greater than 10
* Displays the appropriate message based on the condition

# Concepts Used
* User input with read
* Numeric comparison
* if-else statements
  
The script successfully evaluated user input and displayed whether the number entered was greater than 10 or not.

<img width="1087" height="611" alt="image" src="https://github.com/user-attachments/assets/323fa156-a034-4c72-83dd-fc17ac63eda0" />

<img width="1090" height="611" alt="image" src="https://github.com/user-attachments/assets/d1674595-1d5b-4bf2-b486-d57ba9cf4b93" />

## Task B: File and Directory Validation

# Objective

Create a shell script that:

* Reads a filename or directory name from the user
* Determines whether the input exists
* Checks if the input is:
* - A directory
* - A regular file
* Displays file contents if it is a regular file
* Creates a new file if it does not exist

# Concepts Used
* File testing operators:
* - -d (directory)
* - -f (regular file)

* Conditional statements
* File creation
* Displaying file contents using cat

# The script successfully:

* Identified existing directories
* Identified regular files
* Displayed file contents
* Created new files when they did not exist

# Step 1 and 2: Add the Shebang, Read the name of the file to check for a filename that exists.

Create your script using nano or vi and start by adding the shebang line:

<img width="1088" height="611" alt="image" src="https://github.com/user-attachments/assets/9f199e5e-8e68-4ea6-8911-96fa3e129294" />

<img width="1084" height="611" alt="image" src="https://github.com/user-attachments/assets/3e3e68cc-d46f-424e-979b-405008277221" />

# Step 3: Check whether input is a directory or regular file

* -d checks if it is a directory
* -f checks if it is a normal file

<img width="1088" height="611" alt="image" src="https://github.com/user-attachments/assets/57722e8f-08fc-4b37-846f-edebc3bc39e9" />

<img width="1084" height="611" alt="image" src="https://github.com/user-attachments/assets/94e20ae5-f1ce-4a57-8daf-dbcddbb989a9" />


# Step 4: If the input is a directory and exists, then display the message “Directory exists”.

<img width="1085" height="611" alt="image" src="https://github.com/user-attachments/assets/2ed26590-96fb-40e0-ac59-bd4ebf24982a" />

<img width="1087" height="611" alt="image" src="https://github.com/user-attachments/assets/44ba1e32-6b8d-4427-bc40-8716d7aac493" />


# Step 5: If the input is a regular file, then display the message “It is a regular file, and the file exists” and display the contents of the file

<img width="1085" height="611" alt="image" src="https://github.com/user-attachments/assets/5abc1d32-c4df-41d5-a6c9-95d169918454" />

<img width="1085" height="611" alt="image" src="https://github.com/user-attachments/assets/45f73412-c7a9-490e-9dd0-6a5de4233eba" />


# Step 6: If the given input name in step-1 doesn’t exist, then create the new file with the given name in step-1.

<img width="1088" height="611" alt="image" src="https://github.com/user-attachments/assets/531b6ff8-6601-42c4-8cb7-bbc66bbd5f16" />

<img width="1091" height="611" alt="image" src="https://github.com/user-attachments/assets/0e34238b-fd77-4311-9da6-60bca3533c13" />


# Extra Credit: Add your name to the file (using redirection operator ‘>’) and display the contents for the newly created file

# Step 7: Save and exit the editor and remember to make the script executable using the command chmod +x scriptname.sh)

<img width="1087" height="611" alt="image" src="https://github.com/user-attachments/assets/ccdc5123-dc3d-4af9-88b4-10c4a1314b30" />

<img width="1088" height="611" alt="image" src="https://github.com/user-attachments/assets/d928293e-acac-47c2-a180-e273292085ba" />

<img width="1085" height="611" alt="image" src="https://github.com/user-attachments/assets/e4a555df-d2f9-41e5-a26e-4c2688b17c37" />


# Extra Credit(15 points)- Check Directory

# Step 1: Read Two variables- your name and the name of the directory as input.

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/8474898d-59d6-415a-bc87-cbcdd089e25f" />

<img width="940" height="610" alt="image" src="https://github.com/user-attachments/assets/0789ae89-0361-48f7-86c1-14aa08d7688e" />


# Step 2: Your script should check for the validity of the given directory name, if the entered filename is a directory, then display its contents.

<img width="1088" height="611" alt="image" src="https://github.com/user-attachments/assets/33e23c39-f100-45c6-87a0-0d821fd569d8" />

<img width="1090" height="611" alt="image" src="https://github.com/user-attachments/assets/cbe79200-157d-4fe6-806a-67f941fd5c83" />


# Step 3: If the directory doesn’t exist, then print an error message “Sorry, the entered directory name is not a valid directory name.”

<img width="1090" height="611" alt="image" src="https://github.com/user-attachments/assets/82a143bf-cdc1-4583-927a-2f60f57af157" />

<img width="1085" height="611" alt="image" src="https://github.com/user-attachments/assets/57ae68b5-e962-42d3-a0a5-423d62ce6dc6" />



# Step 4: You need to execute your script and test the following directories to test with your script

* • /etc/systemd

<img width="1088" height="611" alt="image" src="https://github.com/user-attachments/assets/8189c907-67cc-426d-b857-2bf7f156f669" />

<img width="1087" height="611" alt="image" src="https://github.com/user-attachments/assets/3ad755a3-de5c-46ed-a6f9-cc2ce567c585" />



* • /home

<img width="1088" height="611" alt="image" src="https://github.com/user-attachments/assets/5a5d7ac8-9672-485b-9096-c950f6334f2e" />

<img width="1087" height="611" alt="image" src="https://github.com/user-attachments/assets/17b4202b-0886-48e8-853e-ac1ed5ac5587" />


* • A directory that does not exist- (desktop)

<img width="1090" height="611" alt="image" src="https://github.com/user-attachments/assets/6be58c99-d12a-4aee-b2c5-b011a5487ea5" />

<img width="1082" height="611" alt="image" src="https://github.com/user-attachments/assets/7fca41fd-16e9-4410-8b69-f6cf7f08cda7" />


# Lessons Learned

I learned how to write and execute Bash scripts using the nano editor and terminal commands. I also understood the importance of the shebang (#!/bin/bash) in defining the script interpreter for proper execution. Through this lab, I gained practical experience using if-else conditional statements in Linux scripting to make decisions based on user input. I also learned how to check file types using -f for regular files and -d for directories, which is essential for handling different filesystem objects correctly.

In addition, I improved my understanding of file creation, reading, and writing using shell redirection operators such as > and commands like cat. I practiced changing file permissions using chmod +x to make scripts executable, which is a necessary step before running any shell script. Finally, I strengthened my debugging skills by testing scripts with multiple inputs and scenarios, which helped ensure that the scripts behave correctly under different conditions.
