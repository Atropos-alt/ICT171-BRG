# ICT171-BRG

Student Name: Rachel Lee Jiaying

Kaplan Student ID: CT0390460

Murdoch Student ID: 36007211


# 28th March 2026 - Session 1
### 1) Setting up GitHub Account  
   ➜ Created a GitHub account and created a repository for this module, for documentation.
   
### 2) Installing Virtual Machine (VM)  
  ➜ Downloaded and installed Oracle VirtualBox on my laptop. It is used to set up Ubuntu VM for the lab exercises.
   - OS - Ubuntu (64-bit)
   - RAM - 2GB
   - Storage - 10GB
  
### 3) Linux commands learnt in class

| Terminal Commands | What does it do? |
| :---     | :----   |
| sudo apt update    | Check for software updates  |
| sudo apt upgrade -y    | Updates softwares if any |
| pwd   | Show current path (Print Working Directory) |
| ls    | List contents of a directory |
| cd    | Change directory |
| cd ..   | Moves one level up to directory |
| cd /    | Moves to root directory |
| cd -    | Moves to previous directory |
| ip a    | returns the ip address of your own machine |
| ping "link"    | pings the website |
| hostname    | display and change host name |
| df    | To see free space on disk |
| free   | To see used and free memory |
| exit   | End terminal session |
| top   | Real time usage |
| man   | Manual for the commands |
| man ls  | Manual for ls |
| mkdir "directory name" | Make new directory |
| mkdir -p project/src/main | `-p` stands for parents in `mkdir` |

### 4) Checking Linux services
➜ This uses `systemctl list-units --type=service` to check the services running
<img width="1295" height="815" alt="image" src="https://github.com/user-attachments/assets/2661d1fc-07f0-4efa-88b8-c1a5fcaaa7f4" />

➜ This uses `systemctl status snapd` to check the status of snapd.
`snapd` manages, installs, and updates snap packages on Linux.
<img width="1292" height="813" alt="image" src="https://github.com/user-attachments/assets/f973d832-6b1e-4f43-8f5e-385bfccdd528" />

### 5) File Permissions
➜ This creates an empty file called `testing.sh`.  
➜ `ls -l` is used to list the contents of a directory in a long listing format. But in this case it is used to check the file permission. This is before.  
1/2
<img width="1296" height="815" alt="image" src="https://github.com/user-attachments/assets/531645af-8e15-4613-b52c-182493385911" />

➜ `chmod 755 testing.sh`changes the file permission.  
➜ `ls -l` here confirms that the file permission has been changed successfully.  
2/2
<img width="1294" height="816" alt="image" src="https://github.com/user-attachments/assets/2a954b35-ca1c-4b18-b751-d40395e276a2" />
➜ `755` means:  
    Owner `7` = Read `4`, Write `2`, Execute `1` ➜ _rwx_  
    Group `5` = Read `4`, No Write `0`, Execute `1` ➜ _r-x_  
    Others `5` = Read `4`, No Write `0`, Execute `1` ➜ _r-x_  

### 6) Searching in the file, Searching for a file
➜ Here we use `echo "testing" > notes.txt` to write `testing` into `notes.txt`  
➜ Next, we use `find . -name "testing.sh"` to search for a file with the exact name  
➜ Finally, we use `grep -r "testing" .` to search in all subdirectory. (Typo in screenshot)
<img width="1291" height="814" alt="image" src="https://github.com/user-attachments/assets/d5726558-0e61-49ed-8080-1adbc1c5060f" />
