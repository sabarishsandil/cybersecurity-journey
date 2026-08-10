# OverTheWire Bandit - Level 4

## Objective

Find the only human-readable file inside the `inhere` directory.

## Concept Learned

The `file` command can identify the type of data contained in a file.

## Commands Used

```bash
cd inhere
ls -la
file ./*

I looked for the file identified as human-readable text.

then i used:

cat <filename>

What I Learned:

- How to identify file types
- The file command
- Wildcards such as *
- How file extensions do not always tell you the actual file type
- Cybersecurity Connection

- The file command can be useful during investigations because a filename or extension may not accurately describe the content of a file.

Result:

Successfully identified the human-readable file and obtained the next level's password.

Password intentionally not included.
