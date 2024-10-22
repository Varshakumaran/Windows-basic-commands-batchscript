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
Create a directory named "MyLab" on the desktop.
~~~
mkdir %userprofile%\Desktop\MyLab
~~~
![image](https://github.com/user-attachments/assets/b15b3fc9-c992-4e2a-a53d-cda2ced244e0)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.



## COMMAND AND OUTPUT

~~~
cd %userprofile%\Desktop\MyLab
~~~

![image](https://github.com/user-attachments/assets/9c38ce98-5234-4757-9ec4-313a6d617be2)

~~~
type nul > MyFile.txt
~~~

![image](https://github.com/user-attachments/assets/3039509e-9129-483d-a64c-94bfc63a9232)

List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT
~~~
dir %userprofile%\Desktop\MyLab
~~~
![image](https://github.com/user-attachments/assets/36d88192-dc90-43b7-8ec4-82264625147b)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

~~~
mkdir %userprofile%\Desktop\Backup
~~~
![image](https://github.com/user-attachments/assets/f632f9d7-7cc2-4177-85d0-bc3d3f0bd16c)

~~~
copy MyFile.txt %userprofile%\Desktop\Backup
~~~
![image](https://github.com/user-attachments/assets/276db5c5-a7cc-466a-93eb-3614fc98b66d)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
~~~
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
~~~
![image](https://github.com/user-attachments/assets/e44bffc3-c91d-4b84-8a37-e7b1bdca9ed4)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

## COMMAND:

~~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
~~~~

![image](https://github.com/user-attachments/assets/5231b876-c674-465b-b4f6-666dbb9db881)

## COMMAND :

~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
~~~

![image](https://github.com/user-attachments/assets/ce47181b-d539-427f-9b3d-c684766671d1)


# RESULT:
The commands/batch files are executed successfully.

