# OverTheWire Bandit - Level 3

## Objective

Find a hidden file inside the `inhere` directory.

## Concept Learned

Linux files beginning with `.` are hidden by default.

## Commands Used

```bash
cd inhere
ls
ls -la

The -a option allows hidden files to be displayed.

After finding the hidden file:

cat <hidden-file>

What I Learned:

- Hidden files in Linux
- The meaning of . at the beginning of filenames
- Using ls -a
- Navigating directories with cd

Result:

Successfully found the hidden file and obtained the next level's password.

Password intentionally not included.
