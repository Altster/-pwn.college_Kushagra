# Challenge Name
Fun with group names

## My solve
**Flag:** `pwn.college{YeCCuDjXduHsRfQT1f-k0Cgcw3j.QXycjM1wCM2gjNzEzW}`

```bash
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp21534) groups=1000(grp21534)
hacker@permissions~fun-with-groups-names:~$ chgrp grp21534 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{YeCCuDjXduHsRfQT1f-k0Cgcw3j.QXycjM1wCM2gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
The fact that every user has their own group in the system

## References 
None
