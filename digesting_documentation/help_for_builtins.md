# Challenge Name
Help for builtins

## My solve
**Flag:** `pwn.college{A5oDDnZccpZRRnJEEdYEqFYX2wR.QX0ETO0wCM2gjNzEzW}`

```bash
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "A5oDDnZc".
hacker@man~help-for-builtins:~$ challenge --secret A5oDDnZc
Correct! Here is your flag!
pwn.college{A5oDDnZccpZRRnJEEdYEqFYX2wR.QX0ETO0wCM2gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
How to get builtin commands and how to get help about them

## References 
None
