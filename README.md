
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
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/HareeshrajaR/Windows-basic-commands-batchscript/assets/144870459/cb3eb77e-19eb-4685-8d73-f957d261233b)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/HareeshrajaR/Windows-basic-commands-batchscript/assets/144870459/4d29f61c-0e88-42cf-872e-b1ff09202912)


![image](https://github.com/HareeshrajaR/Windows-basic-commands-batchscript/assets/144870459/637c9afc-cecf-406f-a9ef-dcf61c75f411)



List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/HareeshrajaR/Windows-basic-commands-batchscript/assets/144870459/d4197033-9d04-4550-8513-0248fc20144c)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```

![image](https://github.com/HareeshrajaR/Windows-basic-commands-batchscript/assets/144870459/8bc9e2ac-0919-477b-b025-39a945f7afb2)


![image](https://github.com/HareeshrajaR/Windows-basic-commands-batchscript/assets/144870459/fefdde05-4d84-46ee-9135-d1d3c9b7e77c)


Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/HareeshrajaR/Windows-basic-commands-batchscript/assets/144870459/2cfa13a1-6152-4f01-bbe4-4a310c0409a9)



## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT
![image](https://github.com/HareeshrajaR/Windows-basic-commands-batchscript/assets/144870459/4a712e59-e8ca-47c3-880d-670aa06d9450)

# RESULT:
The commands/batch files are executed successfully.

