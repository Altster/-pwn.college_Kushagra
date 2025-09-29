# Challenge Name
Finding commands

## My solve
**Flag:** `pwn.college{8XEe5M0NXPRM78tNoDutZsH_NmI.01NzEzNxwCM2gjNzEzW}`

I didn't realise that I had only reading access to the flag file, not the execution access
```bash
hacker@path~finding-commands:~$ which win
/challenge/paths/28878/win
hacker@path~finding-commands:~$ cat /challenge/paths/28878/flag
pwn.college{8XEe5M0NXPRM78tNoDutZsH_NmI.01NzEzNxwCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@path~finding-commands:~$ which win
/challenge/paths/28878/win
hacker@path~finding-commands:~$ /challenge/paths/28878/flag
bash: /challenge/paths/28878/flag: Permission denied
```

## What I learned
How to find the path to the directory of a command in PATH

## References 
None
