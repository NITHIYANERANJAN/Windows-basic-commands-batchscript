# Windows-basic-commands-batchscript

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
mkdir %userprofile%\Desktop\MyLab
![image](https://github.com/NITHIYANERANJAN/Windows-basic-commands-batchscript/assets/144979351/e4d38925-be6c-437d-b812-9b8a25debeae)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![image](https://github.com/NITHIYANERANJAN/Windows-basic-commands-batchscript/assets/144979351/c3d0a785-f08b-4f88-b5df-b644b02be4aa)
![image](https://github.com/NITHIYANERANJAN/Windows-basic-commands-batchscript/assets/144979351/99140a67-a051-4e5f-9bd2-05f4efeca2c9)



List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/NITHIYANERANJAN/Windows-basic-commands-batchscript/assets/144979351/6960d64d-fa84-42af-a302-68f28518c975)



Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/NITHIYANERANJAN/Windows-basic-commands-batchscript/assets/144979351/4776935a-724a-4308-af91-521b910aec9d)
![image](https://github.com/NITHIYANERANJAN/Windows-basic-commands-batchscript/assets/144979351/3a7f9801-40c7-4f49-a55a-5c78e5473fee)




Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents
![image](https://github.com/NITHIYANERANJAN/Windows-basic-commands-batchscript/assets/144979351/f3a3c913-3d5c-4168-b5ad-3a899d000b37)



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

![image](https://github.com/NITHIYANERANJAN/Windows-basic-commands-batchscript/assets/144979351/f1e02241-ec4b-41e8-9e7d-605195fc7990)





# RESULT:
The commands/batch files are executed successfully.

