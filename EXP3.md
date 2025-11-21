## Experiment 3: Linux File Manipulation and System Manipulation I

### Name: arjun  Roll No.: 590029204   Date: 2025-09-23

### Aim:

* To practice Linux file manipulation commands like `touch`, `cp`, `mv`, `rm`, `cat`, `less`, `head`, `tail`.
* To explore file permissions and ownership with `ls -l`, `chmod`, `chown`, and `chgrp`.
* To search and filter files using `find` and `grep`.
* To understand archiving and compression with `tar`, `gzip`, and `gunzip`.
* To create and manage links (`ln`) for both hard and symbolic links.

### Requirements

* A Linux machine with bash shell (Ubuntu/Fedora/other).
* User privileges to create, modify, and delete files and directories.
* Access to system utilities like `tar`, `gzip`, `grep`, and `find`.

## Theory

Linux file management involves creating, copying, moving, removing, and viewing files. File permissions and ownership ensure secure access control. Searching and filtering tools like `grep` and `find` help locate information efficiently. Archiving with `tar` and compression with `gzip` reduce storage usage and simplify file transfer. Links (`ln`) allow multiple references to the same file data (hard links) or path references (symbolic links).

## Procedure & Observations

## Exercise 1: Creating and Managing Files

### Task Statement:

Create files and manage timestamps using `touch`.

### Command(s):

```bash
touch newfile.txt
touch file1.txt file2.txt file3.txt
touch -t 202401151430 dated_file.txt
```

### Output:

<img width="1483" height="601" alt="image" src="https://github.com/user-attachments/assets/5e96dc99-851a-4136-b002-1e238da322a5" />

---

## Exercise 2: Copying, Moving, and Deleting Files

### Task Statement:

Use `cp`, `mv`, and `rm` to copy, rename, move, and delete files and directories.

### Command(s):

```bash
cp document.txt backup_document.txt
mv oldname.txt newname.txt
rm unwanted_file.txt
rm -r old_directory/
```

### Output:
<img width="1483" height="601" alt="image" src="https://github.com/user-attachments/assets/7767eacd-c9a2-4164-bae2-5ab2becfba65" />


---

## Exercise 3: Viewing File Contents

### Task Statement:

Display file contents using `cat`, `less`, `head`, and `tail`.

### Command(s):

```bash
cat filename.txt
less /var/log/syslog
head -n 5 filename.txt
tail -n 20 filename.txt
tail -f /var/log/syslog
```

### Output:

<img width="1483" height="601" alt="image" src="https://github.com/user-attachments/assets/0cb0f092-13d0-480c-97b9-90c67123d5dd" />


---

## Exercise 4: File Permissions and Ownership

### Task Statement:

Explore file permissions and ownership with `ls -l`, `chmod`, `chown`, and `chgrp`.

### Command(s):

```bash
ls -l
chmod 755 script.sh
chmod u+x script.sh
sudo chown newuser:newgroup file.txt
chgrp developers project.txt
```

### Output:

<p align="center">
<img src="/img/t14.png" width="900">
</p>

---

## Exercise 5: File Searching with `find`

### Task Statement:

Search files by name, type, size, and permissions using `find`.

### Command(s):

```bash
find /home -name "*.txt"
find /home -type f -size +100M
find /etc -name "*conf*"
find /tmp -type f -empty -delete
```

### Output:

<img width="1483" height="601" alt="image" src="https://github.com/user-attachments/assets/b7d31615-a03c-4ed3-b938-f0d05ebc045a" />


---

## Exercise 6: Pattern Searching with `grep`

### Task Statement:

Search for patterns in files using `grep`.

### Command(s):

```bash
grep "error" /var/log/syslog
grep -i "Error" logfile.txt
grep -r "function" ~/code/
grep -n "TODO" *.txt
```

### Output:

<img width="1483" height="601" alt="image" src="https://github.com/user-attachments/assets/18f69c21-c59d-446b-b998-5bfb90477bc8" />


---

## Exercise 7: Archiving and Compression

### Task Statement:

Create and extract archives using `tar`, compress and decompress with `gzip`/`gunzip`.

### Command(s):

```bash
tar -czf backup.tar.gz /home/user/documents
tar -xzf backup.tar.gz -C /restore/
gzip largefile.txt
gunzip largefile.txt.gz
```

### Output:

<img width="1483" height="601" alt="image" src="https://github.com/user-attachments/assets/1829f2e0-f77e-45cf-a53e-b9c8fe89bd6d" />


---

## Exercise 8: Creating Links

### Task Statement:

Create and test hard and symbolic links using `ln`.

### Command(s):

```bash
echo "Hello" > original.txt
ln original.txt hardlink.txt
ln -s original.txt symlink.txt
ls -li original.txt hardlink.txt symlink.txt
```

### Output:

<img width="1483" height="601" alt="image" src="https://github.com/user-attachments/assets/157c1a7d-3314-4717-8455-aa3311d3418e" />


---

## Result

* Successfully created, copied, moved, and deleted files.
* Practiced viewing file contents and monitoring logs.
* Explored file permissions and ownership management.
* Used `find` and `grep` to locate and filter data.
* Created archives and compressed files.
* Demonstrated both hard and symbolic links.

## Challenges Faced & Learning Outcomes

* Challenge 1: Accidentally deleted files with `rm` without `-i`. Learned to use `rm -i` for safety.
* Challenge 2: Remembering numeric vs symbolic permissions in `chmod`. Fixed through repeated practice.

### Learning:

* Gained practical skills with file manipulation and permission commands.
* Learned how to efficiently search files and patterns in Linux.
* Understood how to archive and compress files for better storage management.
* Understood differences between hard and symbolic links.

## Conclusion


This experiment provided hands-on experience with core Linux file management, permissions, searching, archiving, and linking. These are foundational skills for effective Linux system administration and daily usage.
