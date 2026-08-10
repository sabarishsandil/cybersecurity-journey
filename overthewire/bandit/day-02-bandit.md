# OverTheWire Bandit - Day 2

## Introduction

During Day 2, I continued practicing Linux and cybersecurity concepts using OverTheWire Bandit.

I completed Levels 6 to 10.

The main concepts I practiced were:

- Advanced `find`
- `grep`
- `sort`
- `uniq`
- `strings`
- Pipes
- Base64 decoding

Passwords are intentionally not included in this repository.

---

# Level 6 - Finding Files

## Objective

Find a file somewhere on the server with specific properties:

- Owned by user `bandit7`
- Owned by group `bandit6`
- Exactly 33 bytes

## Command Used

```bash
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null

# Level 7 - grep
Objective

Find the password inside data.txt.

The required line contains the word:

millionth
Command Used
grep "millionth" data.txt
Concept Learned

grep is used to search text for a specific pattern.

Basic syntax:

grep "pattern" filename

Example:

grep "error" logfile.txt
What I Learned
Text searching
Pattern matching
Using grep
Cybersecurity Connection

grep is useful for searching:

Log files
Configuration files
Error messages
Suspicious strings
Security events
Result

Successfully found the required line and obtained the password for the next level.

# Level 8 - sort and uniq
Objective

Find the only line in data.txt that occurs exactly once.

Command Used
sort data.txt | uniq -u
Command Breakdown
sort data.txt

Sorts all lines in the file.

|

The pipe sends the output of one command to another command.

uniq -u

Displays only lines that occur once.

What I Learned
sort
uniq
Finding duplicate lines
Finding unique lines
Using pipes
Result

Successfully found the unique line and obtained the password for the next level.

# Level 9 - strings
Objective

Find a human-readable string in data.txt that is preceded by several = characters.

Commands Used
strings data.txt

Then:

strings data.txt | grep "=="
Command Breakdown
strings data.txt

Extracts readable text from the file.

|

Passes the output to another command.

grep "=="

Searches for lines containing ==.

What I Learned
Using strings
Extracting readable text
Working with binary or mixed-content files
Using pipes
Combining commands
Cybersecurity Connection

strings can be useful when investigating binary files and malware because readable strings may contain:

URLs
File paths
Commands
Error messages
Configuration information
Result

Successfully found the required string and obtained the password for the next level.

# Level 10 - Base64
Objective

The password was stored in data.txt using Base64 encoding.

Command Used
base64 -d data.txt

Another method:

cat data.txt | base64 -d
Concept Learned

Base64 is an encoding method used to represent data as text.

Base64 is NOT encryption.

It does not require a secret key to decode.

Encode Example
echo "Hello" | base64
Decode Example
echo "SGVsbG8=" | base64 -d
What I Learned
Base64 encoding
Base64 decoding
Using the base64 command
Difference between encoding and encryption
Cybersecurity Connection

Base64-encoded data can appear in:

Scripts
Web requests
Configuration files
Malware
Logs
CTF challenges

Encoded data should not automatically be considered secure.

Result

Successfully decoded the Base64 data and obtained the password for the next level.

Commands Practiced

During Levels 6-10, I practiced:

find
cat
grep
sort
uniq
strings
base64

I also practiced:

Pipes |
Output redirection
File searching
Text searching
Pattern matching
File ownership searching
File size searching
Binary file investigation
Encoding and decoding
Cybersecurity Skills Practiced

Through Levels 6-10, I practiced:

Linux command-line investigation
Advanced file searching
File ownership analysis
Text searching
Pattern matching
Command pipelines
Binary file investigation
Data encoding and decoding
Progress
Level	Status	Main Concept
Level 6	Completed	Advanced find
Level 7	Completed	grep
Level 8	Completed	sort + uniq
Level 9	Completed	strings + grep
Level 10	Completed	Base64
Result

Successfully completed OverTheWire Bandit Levels 6-10.

Passwords are intentionally not included in this repository.
