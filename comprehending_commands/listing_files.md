# Challenge Name
Listing files

## My solve
**Flag:** `pwn.college{helloworld}`

```bash
hacker@commands~listing-files:~$ ls /challenge
8173-renamed-run-14897  DESCRIPTION.md
hacker@commands~listing-files:~$ /challenge/8173-renamed-run-14897
Yahaha, you found me! Here is your flag:
pwn.college{gnk10fSn1TB0efDY7vkmgS7tHIu.QX4IDO0wCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@commands~listing-files:~$ ls /challenge
8173-renamed-run-14897  DESCRIPTION.md
hacker@commands~listing-files:~$ cat /challenge/8173-renamed-run-14897
#!/opt/pwn.college/bash

echo "Yahaha, you found me! Here is your flag:"
cat /flag
hacker@commands~listing-files:~$ cat /flag
cat: /flag: Permission denied
```

## What I learned
use of ls

## References 
None
