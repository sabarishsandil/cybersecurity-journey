# Day 2 - Linux

## 1. File Permissions

Linux uses file permissions to control who can access a file or directory.

There are three basic permissions:

- `r` - Read
- `w` - Write
- `x` - Execute

There are three categories of users:

- User - Owner of the file
- Group - Users belonging to the file's group
- Others - Everyone else

To view file permissions:

```bash
ls -l

this can be divided into:

- | rwx | r-x | r--
    |     |     |
  User  Group  Others

first character represents the file type:

- = Regular file
d = Directory
l = Symbolic link


## 2.Permission Numbers

- Linux permissions can also be represented using numbers.

Read    = 4
Write   = 2
Execute = 1

- Combining them:

7 = rwx
6 = rw-
5 = r-x
4 = r--
3 = -wx
2 = -w-
1 = --x
0 = ---

- Common permissions:

600 = rw-------
644 = rw-r--r--
700 = rwx------
755 = rwxr-xr-x

## 3.chmod

chmod means "change mode".

It is used to change the permissions of files and directories.

View permissions:
ls -l test.txt

Add execute permission:
chmod +x script.sh

Set permissions using numbers:
chmod 755 script.sh

Example:

chmod 644 notes.txt

This gives:

Owner  → Read + Write
Group  → Read
Others → Read

Practice:

touch test.txt
ls -l test.txt
chmod 600 test.txt
ls -l test.txt
chmod 644 test.txt
ls -l test.txt

The permissions change after using chmod.

## 4.chown

chown means "change owner".

It is used to change the owner of a file or directory.

Basic syntax:
chown username filename

Example:

sudo chown user test.txt

To change both owner and group:

sudo chown user:group test.txt

Check ownership using:

ls -l

Important:

Do not randomly change ownership of system files.

## 5.cat

cat displays the contents of a file.

Example:

cat notes.txt

Create a file and write some text:

echo "Linux Day 2" > notes.txt

Then:

cat notes.txt

Output:

Linux Day 2

cat is especially useful for reading small text files.

I also used cat during OverTheWire Bandit.

# 6.less

less is used to read files one screen at a time.

less notes.txt

It is useful for reading large files.

Important keys:

Space → Next page
b     → Previous page
↑     → Move up
↓     → Move down
q     → Quit

For example:

less /var/log/syslog

less can be useful during cybersecurity investigations when examining large log files.

## 7.head

head displays the beginning of a file.

head notes.txt

By default, it displays the first 10 lines.

To display the first 5 lines:

head -n 5 notes.txt

Example:

head -n 20 /var/log/syslog

This displays the first 20 lines.

## 8.tail

tail displays the end of a file.

tail notes.txt

By default, it displays the last 10 lines.

To display the last 5 lines:

tail -n 5 notes.txt
tail -f

The -f option follows a file as new content is added.

tail -f logfile.txt

This is useful for monitoring live log files.

Press:

Ctrl + C

to stop following the file.

