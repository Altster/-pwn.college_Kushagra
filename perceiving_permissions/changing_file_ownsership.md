# Challenge Name
Changing file ownsership

## My solve
**Flag:** `pwn.college{I43ionva2mVHDayYPwb9nL1DPyy.QXxEjN0wCM2gjNzEzW}`

```bash
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{I43ionva2mVHDayYPwb9nL1DPyy.QXxEjN0wCM2gjNzEzW}
```
## Incorrect tangents I went on
```bash
hacker@permissions~changing-file-ownership:~$ chown hacker flag
hacker@permissions~changing-file-ownership:~$ cat /flag
cat: /flag: Permission denied
```

## What I learned
How to change the ownership of a file

## References 
None
