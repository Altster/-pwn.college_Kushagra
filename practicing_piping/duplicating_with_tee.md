# Challenge Name
Duplicating piped data with tee

## My solve
**Flag:** `pwn.college{QU8hxhymdVSgXIvDRA-C4amMSBm.QXxITO0wCM2gjNzEzW}`

```bash
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee cmd_output | /challenge/college
Processing...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat cmd_output
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "QU8hxhym"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret QU8hxhym | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{QU8hxhymdVSgXIvDRA-C4amMSBm.QXxITO0wCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee /challenge/college
Processing...
You are trying to use 'tee' *instead* of /challenge/college. Use it *between*
/challenge/pwn and /challenge/college!
You must pipe the output of /challenge/pwn into /challenge/college (or 'tee'
for debugging).
```
```bash
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | /challenge/college
Processing...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat pwn
cat: pwn: No such file or directory
hacker@piping~duplicating-piped-data-with-tee:~$ pwn
usage: pwn [-h]
           {asm,checksec,constgrep,cyclic,debug,disasm,disablenx,elfdiff,elfpatch,errno,hex,libcdb,phd,pwnstrip,scramble,shellcraft,template,unhex,update,version}
```

## What I learned

## References 
None
