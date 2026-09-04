# Linux-Practical-EXAM
 Q1. Basic File Operations  Create a directory named LinuxExam.   Navigate into the directory.   Create:  o student.txt  o course.txt  o result.txt   Display the current working directory.   Display the contents of the directory.  
 -Created the `LinuxExam` directory and three files: `student.txt`, `course.txt`, and `result.txt`. Verified the current directory and listed the files using basic Linux commands.
**Commands used:** `mkdir`, `cd`, `touch`, `pwd`, `tree`

Q2. File Management Inside LinuxExam:  Copy student.txt as student_backup.txt.   Rename course.txt to linux_course.txt.   Delete result.txt.   Create directories:  o Documents  o Backups  o Scripts   Move student_backup.txt into Backups.   Display the directory structure
 -Performed file copy, rename, delete, directory creation, and file movement operations inside `LinuxExam`. Created `Documents`, `Backups`, and `Scripts` directories and verified the final directory structure.
**Commands used:** `cp`, `mv`, `rm`, `mkdir`, `tree`

Q3. File Content Operations  Add at least 5 lines of student information to student.txt.   Add at least 5 lines of course information to linux_course.txt.   Display the contents using cat.   Display the first 3 lines using head.   Display the last 2 lines using tail.   Count the number of lines, words, and characters in student.txt
 -Added student and course information to text files and practiced viewing and analyzing file contents using `cat`, `head`, `tail`, and `wc`.
**Commands used:** `cat`, `head`, `tail`, `wc -l`, `wc -w`, `wc -c`

Q4. User Management  Create a user named student01.   Set a password.   Verify that the user exists.   Display the user's UID and GID.   Display the user's home directory.   Switch to the student01 account and verify the current username.  
 -Created the `student01` user, configured a password, and verified the user details including UID, GID, and home directory. Switched to the `student01` account and confirmed the current username.
**Commands used:** `useradd`, `passwd`, `id`, `getent`, `su`, `whoami`

Q5. Group Management  Create a group named linuxbatch.   Add student01 to linuxbatch.   Verify the groups of student01.   Create another user named student02.   Add student02 to linuxbatch.   Display all members of the group
  -Created the `linuxbatch` group and added `student01` and `student02` as group members. Verified the group membership and user-group associations.
**Commands used:** `groupadd`, `usermod -aG`, `groups`, `getent group`

Q6. File Permissions Create project.txt and:  Give owner Read, Write and Execute permission.   Give Group Read and Execute permission.   Give Others Read permission only.   Verify the permissions
  -Created `project.txt` and configured permissions for the owner, group, and others. Verified that the owner has **Read, Write & Execute**, the group has **Read & Execute**, and others have **Read-only** access.
**Commands used:** `touch`, `chmod`, `ls -l`

Then perform the following:  Change the permission to 640.   Change the owner of the file to student01.   Change the group ownership to linuxbatch.   Verify the final ownership and permissions
  -Updated `project.txt` permissions to **640**, changed its owner to `student01`, and assigned the group ownership to `linuxbatch`. Verified the final ownership and permissions.
**Commands used:** `chmod`, `chown`, `ls -l`

Q7. Permission Challenge Create: LinuxExam/ ├── public/ ├── private/ └── shared/ Configure permissions so that:  public can be accessed by everyone.   private can be accessed only by its owner.   shared can be accessed by the owner and group members.   Verify the permissions using ls -ld
  -Created `public`, `private`, and `shared` directories under `LinuxExam` and configured appropriate permissions based on user and group access. Verified the final permissions using `ls -ld`.
**Commands used:** `mkdir`, `chmod`, `ls -ld`

Q8. Package Management  Update the package repository.   Install Apache Web Server.   Verify that Apache is installed.   Display the installed Apache version.   Start the Apache service.   Check the status of Apache.   Configure Apache to start automatically at boot
  -Updated the package repository, installed and verified the Apache Web Server, checked its version, started the Apache service, and configured it to start automatically at system boot.
**Commands used:** `apt update`, `apt install`, `apache2 -v`, `systemctl start`, `systemctl status`, `systemctl enable`

Q9. Apache Web Server Configuration  Find the Apache document root.   Create a custom index.html.   Put the following information on the webpage:  o Student Name  o Roll Number  o Course Name  o "Linux Practical Examination"   Start/restart Apache.   Access the webpage using the browser or curl.   Display the HTTP response using curl
  -Configured the Apache document root and created a custom `index.html` containing student and course details. Restarted Apache and tested the webpage using a browser and `curl`, including verification of the HTTP response.
**Commands used:** `find`, `nano`, `systemctl restart`, `curl`, `curl -I`

Q11. Search and Text Processing Inside LinuxExam:  Create a file named students.txt containing at least 10 student records.   Use grep to find students matching a specified name or pattern.   Use grep with case-insensitive searching.   Count matching records.   Sort the student records.  Search for a particular file using find.  Find all students whose name contains the letter a. or: Find all .txt files inside the LinuxExam directory
  -Created `students.txt` with student records and practiced searching, case-insensitive filtering, counting matches, sorting records, and finding files within the `LinuxExam` directory.
**Commands used:** `grep`, `grep -i`, `sort`, `wc -l`, `find`







