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

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
mkdir %userprofile%\Desktop\MyLab

```
![image](https://github.com/Gokkul-M/Windows-basic-commands-batchscript/assets/144870543/cc81479e-59ca-4b6f-a3da-3c33d470a78f)

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/Gokkul-M/Windows-basic-commands-batchscript/assets/144870543/bea6d2ed-9103-4f36-ae77-272b86af74e2)
![image](https://github.com/Gokkul-M/Windows-basic-commands-batchscript/assets/144870543/dfe71971-b491-4e40-a423-a3cd986d982a)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/Gokkul-M/Windows-basic-commands-batchscript/assets/144870543/5fe03d7d-8908-4f7b-9249-e3457351e886)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/Gokkul-M/Windows-basic-commands-batchscript/assets/144870543/94b231fe-9fcb-46af-8791-00302d494965)

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/Gokkul-M/Windows-basic-commands-batchscript/assets/144870543/1a3d1e73-e435-4120-bbb5-cb9fa105db88)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT
![image](https://github.com/Gokkul-M/Windows-basic-commands-batchscript/assets/144870543/38d334a6-27e6-48d0-921a-fe84c30eb275)

# RESULT:
The commands/batch files are executed successfully.
