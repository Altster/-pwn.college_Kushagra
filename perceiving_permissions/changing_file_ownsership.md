# Challenge Name
Changing file ownership

## My solve
**Flag:** `pwn.college{I43ionva2mVHDayYPwb9nL1DPyy.QXxEjN0wCM2gjNzEzW}`

I thought the file is mentioned as flag in `ls -l`, so I should do `chown` to it, but instead, it should have been `/flag` since the path is to be provided
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
