# OverTheWire Bandit - Level 1

## Objective

Find the password stored in a file named `-`.

## Concept Learned

Linux treats `-` specially in many commands. It can represent standard input.

To refer to a file named `-`, I used a path such as:

```bash
./-

Command Used:

cat ./-


What I Learned:

- Linux filenames can contain special characters
- ./ specifies a file in the current directory
- Special filenames can behave differently when passed directly to commands

Result:

Successfully read the file and obtained the next level's password.

Password intentionally not included.
