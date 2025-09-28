# Challenge Name
Changing permissions

## My solve
**Flag:** `pwn.college{8UAF5N2IOqsKy7Z1nihkRW9bzss.QXzcjM1wCM2gjNzEzW}`

```bash
hacker@permissions~changing-permissions:~$ chmod o+r /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{8UAF5N2IOqsKy7Z1nihkRW9bzss.QXzcjM1wCM2gjNzEzW}
```
## Incorrect tangents I went on
```bash
hacker@permissions~changing-permissions:~$ chmod u+r flag
hacker@permissions~changing-permissions:~$ cat /flag
cat: /flag: Permission denied
```

## What I learned
How to change the permissions of a file

## References 
None
