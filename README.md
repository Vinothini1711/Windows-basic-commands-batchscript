# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT

![Screenshot 2024-10-30 105545](https://github.com/user-attachments/assets/90bc7e00-650b-45ba-a09c-00164a1f15fd)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

![Screenshot 2024-10-30 105613](https://github.com/user-attachments/assets/11a81009-6642-4577-accb-7878405f03ce)

![Screenshot 2024-10-30 105622](https://github.com/user-attachments/assets/cd13d4f7-7b1c-4eab-bf4c-986ebffff312)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT

![Screenshot 2024-10-30 105642](https://github.com/user-attachments/assets/5b4c6e56-cf95-4553-b6ed-61ec0ea167e2)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

![Screenshot 2024-10-30 105719](https://github.com/user-attachments/assets/ff4b08d6-5acd-4e3d-94c4-9e6610124271)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT

![Screenshot 2024-10-30 105802](https://github.com/user-attachments/assets/8b837efa-119b-4167-a357-a6b476647be8)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup. If *.docx file are not available in the Documents folder you can use “.pdf” files to copy. 

Open a notepad file named BackupScript.bat and enter the following:

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\DocBackup\*.docx
echo Backup and deletion completed successfully!
```
Save the file and come back to command prompt.
Now execute as
BackupScript.bat

## OUTPUT:

![image](https://github.com/user-attachments/assets/09699605-160c-41d5-82f0-33ea6af8403d)


# RESULT:
The commands/batch files are executed successfully.

