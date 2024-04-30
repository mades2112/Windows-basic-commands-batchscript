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
```
mkdir %userprofile%\Desktop\MyLab
```
![326683013-f1f83410-e659-40ff-bee3-e079d93c7736](https://github.com/mades2112/Windows-basic-commands-batchscript/assets/152461996/b374a8e3-513c-4e2a-b9c1-f5cbace1f8af)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![326683213-4de1b4bd-f842-485a-bf0d-90def6eaf1e9](https://github.com/mades2112/Windows-basic-commands-batchscript/assets/152461996/199eea44-cbf2-4238-bc23-6e7806f26f4a)

![326683200-60ef83ad-950a-4bf7-ae70-7ccd4fae7aa7](https://github.com/mades2112/Windows-basic-commands-batchscript/assets/152461996/cb0a6f84-8352-46a9-89f7-614b9b1442cf)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![326683303-a28afee5-4fc8-4720-a29b-ae4c9819f177](https://github.com/mades2112/Windows-basic-commands-batchscript/assets/152461996/8fa4f5a8-c15b-4e4c-ac8d-f3e6dde2a3a3)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```



## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![326683386-0fe73689-4d9b-4494-8ce8-d940fc9b9606](https://github.com/mades2112/Windows-basic-commands-batchscript/assets/152461996/2e34584e-0c0f-4d55-a79f-a7b6eda303e2)


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


![326683409-f8257a6d-6fa4-4e1a-bc73-063fad3c5508](https://github.com/mades2112/Windows-basic-commands-batchscript/assets/152461996/e19f90bd-402d-4033-9b40-31c1bd296253)



# RESULT:
The commands/batch files are executed successfully.

