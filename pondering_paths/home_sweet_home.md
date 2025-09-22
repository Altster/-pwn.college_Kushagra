# Challenge Name
Home sweet home

## My solve
**Flag:** `pwn.college{MehP-VQowqtE4pWoAU0BWMoEbJ3.QXzMDO0wCM2gjNzEzW}`

I was wondering whether a solve with less than 3 characters would be possible, which led me down a tangent
```bash
hacker@paths~home-sweet-home:~$ /challenge/run ~/f
Writing the file to /home/hacker/f!
... and reading it back to you:
pwn.college{MehP-VQowqtE4pWoAU0BWMoEbJ3.QXzMDO0wCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@paths~home-sweet-home:~$ /challenge/run ~/
Writing the file to /home/hacker/!
/challenge/run: line 29: /home/hacker/: Is a directory
... and reading it back to you:
cat: /home/hacker/: Is a directory
```

## What I learned
~ refers to home directory `home/hacker`

## References 
None
