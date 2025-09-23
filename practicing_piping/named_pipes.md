# Challenge Name
Named pipes

## My solve
**Flag:** `pwn.college{EguBo0Zws3Oih3Yo6TefuZsYfFm.01MzMDOxwCM2gjNzEzW}`

SSH:-
```bash
hacker@piping~named-pipes:~$ mkfifo /tmp/flag_fifo
hacker@piping~named-pipes:~$ /challenge/run > /tmp/flag_fifo
You're successfully redirecting /challenge/run to a FIFO at /tmp/flag_fifo!
Bash will now try to open the FIFO for writing, to pass it as the stdout of
/challenge/run. Recall that operations on FIFOs will *block* until both the
read side and the write side is open, so /challenge/run will not actually be
launched until you start reading from the FIFO!
```

Terminal:-
```bash
hacker@piping~named-pipes:~$ cat /tmp/flag_fifo
You've correctly redirected /challenge/run's stdout to a FIFO at 
/tmp/flag_fifo! Here is your flag:
pwn.college{EguBo0Zws3Oih3Yo6TefuZsYfFm.01MzMDOxwCM2gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
The concept of named pipes (FIFOs)

## References 
None
