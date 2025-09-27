# Challenge Name
Listing processes

## My solve
**Flag:** `pwn.college{QQCsM7mq3id5Odlim4Lp4RPiooZ.QX4MDO0wCM2gjNzEzW}`

```bash
hacker@processes~listing-processes:~$ ps -efww
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 18:01 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-workspace/bin/dojo-init /run/dojo/bin/sleep 6h
root           7       1  0 18:01 ?        00:00:00 /run/dojo/bin/sleep 6h
root         132       1  0 18:01 ?        00:00:00 /challenge/31869-run-2465
root         135     132  0 18:01 ?        00:00:00 sleep 6h
hacker       137       0  0 18:01 pts/0    00:00:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interactive-5.2p37/bin/bash /run/dojo/bin/ssh-entrypoint
hacker       143     137  0 18:01 pts/0    00:00:00 /run/dojo/bin/bash --login
hacker       152     143  0 18:02 pts/0    00:00:00 ps -efww
hacker@processes~listing-processes:~$ /challenge/31869-run-2465
Yahaha, you found me! Here is your flag:
pwn.college{QQCsM7mq3id5Odlim4Lp4RPiooZ.QX4MDO0wCM2gjNzEzW}
Now I will sleep for a while (so that you could find me with 'ps').
```
## Incorrect tangents I went on
None

## What I learned
How to view all the ongoing processes and 2 different ways to represent it

## References 
None
