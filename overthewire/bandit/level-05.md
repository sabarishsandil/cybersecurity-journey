# OverTheWire Bandit - Level 5

## Objective

Find a file inside the `inhere` directory with specific properties:

- Human-readable
- Exactly 1033 bytes
- Not executable

## Concept Learned

The `find` command can search for files using different conditions.

## Command Used

```bash
find . -type f -size 1033c ! -executable

command breakdown:

find

Search for files and directories.

.

Start searching from the current directory.

-type f

Search only for regular files.

-size 1033c

Find files exactly 1033 bytes in size.

! -executable

Exclude executable files.

What I Learned:

- Recursive file searching
- Searching by file type
- Searching by file size
- Checking executable status
- Combining multiple find conditions
- Cybersecurity Connection

- find is useful when investigating Linux systems and searching for suspicious or specific files.

Result:

Successfully found the required file and obtained the next level's password.

Password intentionally not included.
