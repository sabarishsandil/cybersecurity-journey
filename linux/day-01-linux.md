# Day 1 - Linux

## 1. What is Linux?

Linux is an open-source operating system kernel. Linux distributions such as Ubuntu, Debian and Kali Linux use the Linux kernel along with system software and applications.

Linux is widely used in:
- Servers
- Cloud computing
- Cybersecurity
- Networking
- Development
- Embedded systems

## 2. Linux File System

Linux uses a hierarchical file system that starts from the root directory `/`.

Important directories:

- `/` - Root directory
- `/home` - Personal directories of normal users
- `/root` - Home directory of the root user
- `/etc` - System configuration files
- `/var` - Logs and changing data
- `/tmp` - Temporary files
- `/usr` - Programs and system resources
- `/dev` - Device files

## 3. pwd

`pwd` means Present Working Directory.

It shows the current directory.

```bash
pwd

## 4.ls

`ls` lists files and directories.

```bash
ls

Useful options:

```bash
ls -l
ls -a
ls -la

- `-l` - Detailed information
- `-a` - Shows hidden files

## 5.cd

`cd` means Change Directory.cd means Change Directory.

```bash
cd Documents

Go back:

```bash
cd ..

Go to home:

```bash
cd ~

Go to root:

```bash
cd /

## 6.mkdir

`mkdir` means Make Directory.

```bash

mkdir project

Creates a new directory.

## 7.touch

Creates an empty file.

```bash

touch notes.txt

## 8.rm

Removes files or directories.

rm notes.txt

Remove a directory:

rm -r project

Be careful with:

rm -rf

It can permanently delete files and directories.

## 9.cp

cp copies files or directories.

Copy a file:

cp notes.txt backup.txt

Copy a directory:

cp -r project project_backup

## 10.mv

mv moves or renames files and directories.

Move:

mv notes.txt Documents/

Rename:

mv old.txt new.txt

## 11.cat

Displays the contents of a file.

cat notes.txt

## 12.file

Identifies the type of a file.

file filename

## 13.Hidden Files

Files beginning with . are hidden by default.

Example:

.config
.ssh

Show hidden files:

ls -a

## 14.find

Searches for files and directories.

find .

Find regular files:

find . -type f

Find directories:

find . -type d

Find files by size:

find . -type f -size 1033c

## 15.Linux Permissions - Introduction


Linux uses permissions to control access to files.

Three basic permissions:

r - Read
w - Write
x - Execute

Permission categories:

User
Group
Others



