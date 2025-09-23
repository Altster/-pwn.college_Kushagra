# Challenge Name
Reading input

## My solve
**Flag:** `pwn.college{YSXcIy9DFqDIRmhZKstnYPVgFll.QX4cTN0wCM2gjNzEzW}`

```bash
hacker@variables~reading-input:~$ read PWN
COLLEGE
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{YSXcIy9DFqDIRmhZKstnYPVgFll.QX4cTN0wCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@variables~reading-input:~$ PWN=$(read COLLEGE)
You appear to be invoking a subshell. This could be, for example, because you
are doing something like `PWN=$(echo COLLEGE)`. Instead, you must use `read` to
set the PWN variable.
```

## What I learned
How to read input from the user

## References 
None
