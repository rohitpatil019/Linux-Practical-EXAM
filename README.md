# 🐧 Linux Practical Examination

## 📌 Overview

This project is based on a **Linux Practical Examination** that covers essential Linux system administration and command-line operations.

The practical includes file and directory management, file content operations, user and group management, permissions, package management, Apache web server configuration, networking, and search and text-processing commands.

The main objective of this project is to gain practical knowledge of Linux commands and understand basic Linux system administration tasks.

---

## 🎯 Objectives

* Learn and practice basic Linux commands.
* Understand file and directory management.
* Manage Linux users and groups.
* Configure file and directory permissions.
* Install and manage software packages.
* Configure and manage the Apache Web Server.
* Practice searching and text-processing commands.
* Develop basic Linux system administration skills.

---

# ⭐ Features

* Basic Linux file and directory operations
* File creation, copying, renaming, moving, and deletion
* File content management using Linux commands
* User creation and user information management
* Group creation and user-group management
* File permissions using `chmod`
* File ownership using `chown`
* Directory access control
* Apache Web Server installation and configuration
* Custom Apache webpage creation
* HTTP response testing using `curl`
* Searching files using `find`
* Searching text using `grep`
* Sorting records using `sort`
* Counting lines, words, and characters using `wc`

---

# 🏗️ Project Structure / Architecture

```text
Linux-Practical-EXAM/
│
├── LinuxExam/
│   │
│   ├── student.txt
│   ├── linux_course.txt
│   ├── project.txt
│   ├── students.txt
│   │
│   ├── Documents/
│   │
│   ├── Backups/
│   │   └── student_backup.txt
│   │
│   ├── Scripts/
│   │
│   ├── public/
│   ├── private/
│   └── shared/
│
├── screenshots/
│   ├── Q1.png
│   ├── Q2.png
│   ├── Q3.png
│   ├── Q4.png
│   ├── Q5.png
│   ├── Q6.png
│   ├── Q7.png
│   ├── Q8.png
│   ├── Q9.png
│   ├── Q10.png
│   └── Q11.png
│
└── README.md
```

---

# 🛠️ Technologies Used

| Technology  | Purpose                              |
| ----------- | ------------------------------------ |
| Linux       | Operating System                     |
| Bash Shell  | Command-line operations              |
| Apache      | Web Server                           |
| Git         | Version Control                      |
| GitHub      | Project Repository                   |
| HTML        | Webpage creation                     |
| `systemctl` | Service management                   |
| `chmod`     | Permission management                |
| `chown`     | Ownership management                 |
| `grep`      | Text searching                       |
| `find`      | File searching                       |
| `sort`      | Sorting records                      |
| `wc`        | Counting lines, words and characters |
| `curl`      | HTTP testing                         |

---

# 📚 Practical Tasks

## Q1. Basic File Operations

### Tasks

* Create a directory named `LinuxExam`.
* Navigate into the directory.
* Create:

  * `student.txt`
  * `course.txt`
  * `result.txt`
* Display the current working directory.
* Display the contents of the directory.

### Work Done

Created the `LinuxExam` directory and three files. Verified the current working directory and displayed the files.

### Commands Used

```bash
mkdir
cd
touch
pwd
ls
tree
```

---

## Q2. File Management

### Tasks

* Copy `student.txt` as `student_backup.txt`.
* Rename `course.txt` to `linux_course.txt`.
* Delete `result.txt`.
* Create:

  * `Documents`
  * `Backups`
  * `Scripts`
* Move `student_backup.txt` into `Backups`.
* Display the directory structure.

### Work Done

Performed file copying, renaming, deletion, directory creation, and file movement operations.

### Commands Used

```bash
cp
mv
rm
mkdir
tree
```

---

## Q3. File Content Operations

### Tasks

* Add at least 5 lines of student information to `student.txt`.
* Add at least 5 lines of course information to `linux_course.txt`.
* Display contents using `cat`.
* Display the first 3 lines using `head`.
* Display the last 2 lines using `tail`.
* Count lines, words, and characters using `wc`.

### Work Done

Added student and course information and practiced displaying and analyzing file contents.

### Commands Used

```bash
cat
head
tail
wc -l
wc -w
wc -c
```

---

## Q4. User Management

### Tasks

* Create a user named `student01`.
* Set a password.
* Verify that the user exists.
* Display UID and GID.
* Display the user's home directory.
* Switch to the `student01` account.
* Verify the current username.

### Work Done

Created `student01`, configured the password, verified user information, and switched to the account.

### Commands Used

```bash
useradd
passwd
id
getent
su
whoami
```

---

## Q5. Group Management

### Tasks

* Create a group named `linuxbatch`.
* Add `student01` to `linuxbatch`.
* Verify the groups of `student01`.
* Create another user named `student02`.
* Add `student02` to `linuxbatch`.
* Display all group members.

### Work Done

Created the `linuxbatch` group and added both `student01` and `student02`.

### Commands Used

```bash
groupadd
usermod -aG
groups
getent group
```

---

## Q6. File Permissions

### Tasks

Create `project.txt` and configure:

* Owner → Read, Write, Execute
* Group → Read, Execute
* Others → Read only

Then:

* Change permission to `640`.
* Change owner to `student01`.
* Change group to `linuxbatch`.
* Verify final permissions.

### Work Done

Configured file permissions and ownership using Linux permission and ownership commands.

### Commands Used

```bash
touch
chmod
chown
ls -l
```

### Final Permission

```text
640
```

Meaning:

```text
Owner  → Read + Write
Group  → Read
Others → No permission
```

---

## Q7. Permission Challenge

### Directory Structure

```text
LinuxExam/
├── public/
├── private/
└── shared/
```

### Tasks

* `public` → Accessible by everyone
* `private` → Accessible only by owner
* `shared` → Accessible by owner and group members
* Verify permissions using `ls -ld`

### Work Done

Created the required directories and configured permissions according to the access requirements.

### Commands Used

```bash
mkdir
chmod
ls -ld
```

---

## Q8. Package Management

### Tasks

* Update package repository.
* Install Apache Web Server.
* Verify Apache installation.
* Display Apache version.
* Start Apache.
* Check Apache status.
* Enable Apache at boot.

### Work Done

Installed and configured the Apache Web Server and verified that the service was running.

### Commands Used

```bash
apt update
apt install
apache2 -v
systemctl start
systemctl status
systemctl enable
```

> **Note:** The exact package command can vary depending on the Linux distribution. For Amazon Linux, Apache is commonly installed using `httpd` and `dnf`/`yum`.

---

## Q9. Apache Web Server Configuration

### Tasks

* Find Apache document root.
* Create a custom `index.html`.
* Add:

  * Student Name
  * Roll Number
  * Course Name
  * "Linux Practical Examination"
* Restart Apache.
* Access webpage using browser or `curl`.
* Display HTTP response using `curl`.

### Work Done

Configured the Apache document root and created a custom webpage containing student and examination information.

### Commands Used

```bash
find
nano
systemctl restart
curl
curl -I
```

---

## Q10. Linux Networking

### Tasks

The networking practical focuses on basic Linux networking and connectivity verification.

### Work Done

Practiced identifying network information, checking connectivity, viewing IP configuration and testing network communication.

### Common Commands

```bash
ip addr
ip route
hostname
ping
curl
ss
```

These commands help administrators troubleshoot basic Linux network connectivity and services.

---

## Q11. Search and Text Processing

### Tasks

Inside `LinuxExam`:

* Create `students.txt` containing at least 10 student records.
* Search students using `grep`.
* Perform case-insensitive searching.
* Count matching records.
* Sort student records.
* Search for files using `find`.
* Find students whose name contains the letter `a`.
* Find all `.txt` files inside `LinuxExam`.

### Work Done

Created student records and practiced searching, filtering, counting, sorting, and file searching.

### Commands Used

```bash
grep
grep -i
sort
wc -l
find
```

---

# 🏛️ Architecture / Workflow

```text
                 Linux Operating System
                         │
                         ▼
                  Bash Terminal
                         │
          ┌──────────────┼──────────────┐
          ▼              ▼              ▼
       Files &         Users &       Permissions
     Directories        Groups         & Ownership
          │              │              │
          └──────────────┼──────────────┘
                         ▼
                 Package Management
                         │
                         ▼
                  Apache Web Server
                         │
                         ▼
                  Custom Web Page
                         │
                         ▼
               Browser / curl Testing
                         │
                         ▼
               Search & Text Processing
```

---

# 🔗 GitHub Repository

The complete project and practical documentation are available on GitHub:

**GitHub Repository:**
https://github.com/rohitpatil019/Linux-Practical-EXAM

---

# 📸 Screenshots

Screenshots are included to demonstrate the execution and results of the practical tasks.

Example:

```text

# 🎓 Learning Outcomes

After completing this practical examination, I gained hands-on knowledge of:

* Linux command-line operations
* File and directory management
* Linux users and groups
* File permissions and ownership
* Basic system administration
* Package installation and management
* Apache Web Server management
* Basic web server configuration
* Linux networking commands
* File and text searching
* Text processing
* Service management using `systemctl`
* Basic troubleshooting
* Git and GitHub repository management

---

# 🚀 Future Enhancements

The project can be enhanced in the future by:

* Adding advanced Linux networking tasks
* Adding shell scripting automation
* Creating automated system administration scripts
* Adding Linux monitoring commands
* Adding CPU, memory and disk monitoring
* Configuring Apache Virtual Hosts
* Implementing HTTPS using SSL/TLS
* Adding firewall configuration using `firewalld`
* Automating server setup using Bash scripts
* Integrating AWS EC2 deployment
* Adding CI/CD automation using GitHub Actions

---

# 👨‍💻 Author

**Rohit Pradip Patil**

### Skills Practiced

* Linux
* AWS
* Networking
* Apache
* Bash
* Git
* GitHub
* System Administration
* Troubleshooting

### GitHub

https://github.com/rohitpatil019

---

# 📝 Conclusion

This Linux Practical Examination provided hands-on experience with essential Linux system administration concepts.

During this practical, I worked with files, directories, users, groups, permissions, packages, Apache Web Server, networking commands, and text-processing utilities.

The practical helped me understand how Linux commands are used in real-world system administration and troubleshooting environments. It also improved my confidence in working with the Linux command line and managing basic server operations.

Overall, this project provided a strong foundation for further learning in **Linux System Administration, Cloud Computing, AWS, Networking, and Technical Support**.

---

## ⭐ Project Status

**Completed ✅**

This project was created as part of Linux practical and system administration learning.





