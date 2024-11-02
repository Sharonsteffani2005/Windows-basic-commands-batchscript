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

mkdir %sec%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/755849ef-817d-49dc-a1cc-908131a16732)


## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```

cd %sec%\Desktop\MyLab
touch MyFile.txt
```
![image](https://github.com/user-attachments/assets/c395f3c3-5517-40e1-9953-0db095b9913b)

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
dir %sec%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/f64f403d-3f6e-45e6-9527-b196e9ca4603)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```

mkdir %sec%\Desktop\Backup
cp MyFile.txt %sec%\Desktop\Backup

```
![image](https://github.com/user-attachments/assets/a364f430-04ba-499f-974a-451671955492)
![image](https://github.com/user-attachments/assets/613b27ef-3d0b-4640-897a-ac468e1305db)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mv MyFile.txt MyLab\Documents
```
![image](https://github.com/user-attachments/assets/cdf773a9-9ba7-4e8f-961d-f3ffd22a2fe8)

## COMMAND AND OUTPUT


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

### BackupScript.bat
```

@echo off
mkdir %sec%\Desktop\DocBackup
copy %sec%\Documents\*.docx %sec%\Desktop\DocBackup
del %sec%\Documents\DocBackup\*.docx
echo Backup and deletion completed successfully!
```




## OUTPUT
![image](https://github.com/user-attachments/assets/9d71f17e-12b1-4687-b2bc-fa46619d7a9a)


# RESULT:
The commands/batch files are executed successfully.

