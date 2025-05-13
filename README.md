# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

Name:- V.B.Laksha

Reg.no:- 212224220051

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

~~~
mkdir %userprofile%\Desktop\MyLab

~~~

![image](https://github.com/user-attachments/assets/e4d4d320-6d2b-414b-97a4-d6e79fc7f4aa)



## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

~~~

cd %userprofile%\Desktop\MyLab
type nul > MyFile.txt

~~~

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.

~~~

dir %userprofile%\Desktop\MyLab

~~~

![image](https://github.com/user-attachments/assets/04c42731-1792-4d0b-b3c9-08ff10b18ca1)


## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

~~~
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
~~~
![image](https://github.com/user-attachments/assets/082c4cdf-8f35-4a0d-a897-8bab0e5634fb)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
~~~
move MyLab Documents
~~~
![image](https://github.com/user-attachments/assets/28de3ca8-bcbb-4e67-a728-0e6af2d0a686)



## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup. If *.docx file are not available in the Documents folder you can use “.pdf” files to copy.

Open a notepad file named BackupScript.bat and enter the following:

## Command

~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!

~~~





## OUTPUT

![image](https://github.com/user-attachments/assets/205ea07c-fe6c-4057-bea5-7e448568d0ed)




# RESULT:
The commands/batch files are executed successfully.

