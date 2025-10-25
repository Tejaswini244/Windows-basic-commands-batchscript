# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file . Save each script in a file with a .bat extension. Ensure you have the necessary permissions to perform the operations. Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\MyLab
```
<img width="1246" height="146" alt="image" src="https://github.com/user-attachments/assets/f5bfea82-7f76-4254-a518-0d169f4d12d2" />


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

```
cd %userprofile%\Desktop\MyLab
```
<img width="1026" height="148" alt="image" src="https://github.com/user-attachments/assets/3532e4d7-b046-4f5b-a3ff-4b0b7befe0f6" />


type nul > MyFile.txt

<img width="978" height="131" alt="image" src="https://github.com/user-attachments/assets/3244306a-dcef-4090-9c86-d7de42efa6ed" />


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT

```
dir %userprofile%\Desktop\MyLab
```
<img width="1205" height="422" alt="image" src="https://github.com/user-attachments/assets/96aa8d14-c09e-43a7-a41d-02d920e78018" />

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\Backup
```
<img width="1180" height="135" alt="image" src="https://github.com/user-attachments/assets/2c711b8f-1869-4dbc-9e25-9716c32752de" />

copy MyFile.txt %userprofile%\Desktop\Backup

<img width="1196" height="155" alt="image" src="https://github.com/user-attachments/assets/e92f35f2-0cd4-436b-97a8-6e164df78757" />

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\Documents
```
move MyLab Documents

<img width="1155" height="210" alt="image" src="https://github.com/user-attachments/assets/cfa3eac8-ce52-4ef7-be3e-b63f49c6e5f0" />

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

## COMMAND

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

## OUTPUT

<img width="1191" height="322" alt="image" src="https://github.com/user-attachments/assets/7dba02c5-ac6b-480e-9109-bfc1106127ae" />

## COMMAND
```
  @echo off
  mkdir %userprofile%\Desktop\DocBackup
  copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
  del %userprofile%\Documents\*.docx
  echo Backup and deletion completed successfully!
```
## OUTPUT

<img width="1260" height="292" alt="image" src="https://github.com/user-attachments/assets/7285b9e2-5106-43b3-917c-059fcf9cb2e9" />

# RESULT:
The commands/batch files are executed successfully.

