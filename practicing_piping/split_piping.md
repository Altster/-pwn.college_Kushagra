# Challenge Name
Split-piping stderr and stdout

## My solve
**Flag:** `pwn.college{AyKOq_ePrLmzgYKHF--fa_jCPUo.QXxQDM2wCM2gjNzEzW}`

```bash
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack 2> >( /challenge/the ) | /challenge/planet
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{AyKOq_ePrLmzgYKHF--fa_jCPUo.QXxQDM2wCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack | 2>/challenge/the >(/challenge/planet)
bash: /challenge/the: Permission denied
Are you sure you're properly redirecting /challenge/hack's standard output into
'/challenge/planet'?
You must redirect my standard error into '/challenge/the'!
```
```bash
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack | 2>& 1 | /challenge/the >(/challenge/planet)
Are you sure you're properly redirecting /challenge/hack's standard error into
'/challenge/the'?
You must redirect my standard error into '/challenge/the'!
Are you sure you're properly redirecting /challenge/hack's standard output into
'/challenge/planet'?
```

## What I learned
A way to keep the stderr and stdout streams separate, i.e., split piping

## References 
None
