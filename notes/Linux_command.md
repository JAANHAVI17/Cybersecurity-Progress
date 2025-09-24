# Cybersecurity Learning Progress 🚀

This repository contains my notes and progress in learning *Linux commands* and *basic cybersecurity concepts*. I’m documenting my journey step by step, and this will serve as both a personal reference and a way to share my progress with others.

---

## 📌 Topics Covered

### 🔹 Linux Commands
- *System Information*
  - ifconfig → Know IP address  
  - uname → Basic hardware/software information  

- *File & Directory Management*
  - ls → List all available files & folders  
  - ls -a → Show hidden files  
  - pwd → Print current directory  
  - cd → Change directory  
  - cd .. → Go back to previous directory  
  - mkdir → Create directory  
  - rmdir → Remove directory  

- *File Operations*
  - touch file → Create empty file  
  - cat file → Read file contents  
  - rm file → Remove file  
  - cp file destination/ → Copy file  
  - mv file destination/ → Move file / Rename file  

- *Other Useful Commands*
  - date → Show system date & time  
  - clear → Clear terminal  
  - zip/unzip → Compress/Extract files  
  - locate → Find file location  

---

### 🔹 File Permissions
Linux file permissions control *who can read, write, or execute files and directories*.  
Each file/directory has 3 types of users and 3 types of permissions.

#### *User Types*
- *u (user/owner)* → The person who created the file  
- *g (group)* → Users in the file’s group  
- *o (others)* → Everyone else  
- *a (all)* → Combination of user, group, and others  

#### *Permission Types*
- r → Read (4) : View the contents of a file or list a directory  
- w → Write (2) : Modify a file or add/delete files in a directory  
- x → Execute (1) : Run a file as a program or enter a directory  

#### *Viewing Permissions*
Use the command:  
```bash
ls -l
```
output:
```bash
-rwxr-xr--  1 user group  4096 Sep 23  file.sh
```

## Breakdown:

- → File type ( - = regular file, d = directory, l = link )

rwx → Owner (user) has read, write, and execute

r-x → Group has read and execute

r-- → Others have only read


### Changing Permissions (chmod)

Numeric method (octal values)

chmod 777 file → rwx for all (user, group, others)

chmod 644 file → rw for owner, r for group & others

chmod 755 file → rwx for owner, rx for group & others


### Symbolic method

chmod u+x file → Add execute for user

chmod g-w file → Remove write for group

chmod o=r file → Give others only read


- Here’s a screenshot explaining Linux file permissions:  

![Permissions Example](notes/Images/permissions.png)

---

### 🔹 Basic Shortcuts
- Ctrl + L → Clear terminal  
- Ctrl + C → Kill process  
- Ctrl + Z → Stop process  
- Ctrl + Shift + C → Copy content  
- Ctrl + Shift + V → Paste content  
- Ctrl + A → Go to beginning of line  
- Ctrl + E → Go to end of line  
- Ctrl + K → Cut text from cursor to end  

---

## ✨ Author
👩‍💻 Janhavi Mestry

