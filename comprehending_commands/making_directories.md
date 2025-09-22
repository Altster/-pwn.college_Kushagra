# Challenge Name
Making directories

## My solve
**Flag:** `pwn.college{8hzfYCThG3W-1PuiVrIZ5sIAGgo.QXxMDO0wCM2gjNzEzW}`

```bash
hacker@commands~making-directories:~$ mkdir /tmp/pwn
hacker@commands~making-directories:~$ cd /tmp/pwn
hacker@commands~making-directories:/tmp/pwn$ cd college
bash: cd: college: No such file or directory
hacker@commands~making-directories:/tmp/pwn$ touch college
hacker@commands~making-directories:/tmp/pwn$ cd
hacker@commands~making-directories:~$ /challenge/run
Success! Here is your flag:
pwn.college{8hzfYCThG3W-1PuiVrIZ5sIAGgo.QXxMDO0wCM2gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
How to make a directory

## References 
None
