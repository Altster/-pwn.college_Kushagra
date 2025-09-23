# Challenge Name
Writing to multiple programs

## My solve
**Flag:** `pwn.college{wAq6n-kNNyc4QNt3Gt3I34iidyq.QXwgDN1wCM2gjNzEzW}`

```bash
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | >(/challenge/the) >(/challenge/planet)
bash: /dev/fd/63: Permission denied
Are you sure you're properly redirecting input into '/challenge/planet'?
Are you sure you're properly redirecting input into '/challenge/the'?
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{wAq6n-kNNyc4QNt3Gt3I34iidyq.QXwgDN1wCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee /challenge/the
WARNING: it looks like you passed the path /challenge/the, instead of the
substituted process, to tee. This will cause tee to try to write to the
/challenge/the file, rather than have the shell launch the /challenge/the
command and redirect tee's output to it.
/usr/bin/tee: /challenge/the: Permission denied
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
2798151293020431521
```
```bash
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >(/challenge/the) >(/challenge/planet)
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
15705156182481412641
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{wAq6n-kNNyc4QNt3Gt3I34iidyq.QXwgDN1wCM2gjNzEzW}
```

## What I learned


## References 
None
