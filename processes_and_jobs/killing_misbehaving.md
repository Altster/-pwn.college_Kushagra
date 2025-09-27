# Challenge Name
killing misbehaving processes

## My solve
**Flag:** `pwn.college{E5NYv6aBzSKKVCUGYmr1NoMA-h5.0FNzMDOxwCM2gjNzEzW}`

SSH (Ubuntu)
```bash
hacker@processes~killing-misbehaving-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.1  0.0   1056   640 ?        Ss   18:09   0:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-works
root           8  0.1  0.0 231708  2560 ?        S    18:09   0:00 /run/dojo/bin/sleep 6h
root         138  0.0  0.0   4132  1280 ?        S    18:09   0:00 /bin/bash /challenge/.init
root         139  0.0  0.0   4132  1280 ?        S    18:09   0:00 /bin/bash /challenge/.init
root         140  0.0  0.0   5204  3520 ?        S    18:09   0:00 su -c exec /challenge/decoy > /tmp/flag_fifo hacker
root         141  0.0  0.0   2744  1280 ?        S    18:09   0:00 sleep 6h
root         142  0.0  0.0   2744  1600 ?        S    18:09   0:00 sleep 6h
hacker       143  0.1  0.0  13516  9280 ?        Ss   18:09   0:00 /usr/bin/python /challenge/decoy
hacker       145  0.1  0.0 231576  3520 pts/0    Ss   18:09   0:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-inte
hacker       151  0.0  0.0 231972  4160 pts/0    S    18:09   0:00 /run/dojo/bin/bash --login
hacker       161  0.0  0.0 233600  3840 pts/0    R+   18:09   0:00 ps aux
hacker@processes~killing-misbehaving-processes:~$ kill 143
hacker@processes~killing-misbehaving-processes:~$ /challenge/run
Sending the flag to /tmp/flag_fifo!
```

Terminal 
```bash
hacker@processes~killing-misbehaving-processes:~$ cat /tmp/flag_fifo
pwn.college{E5NYv6aBzSKKVCUGYmr1NoMA-h5.0FNzMDOxwCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@processes~killing-misbehaving-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  1 18:09 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-workspace/bin/dojo-i
root           8       1  0 18:09 ?        00:00:00 /run/dojo/bin/sleep 6h
root         138       1  0 18:09 ?        00:00:00 /bin/bash /challenge/.init
root         139       1  0 18:09 ?        00:00:00 /bin/bash /challenge/.init
root         140       1  0 18:09 ?        00:00:00 su -c exec /challenge/decoy > /tmp/flag_fifo hacker
root         141     138  0 18:09 ?        00:00:00 sleep 6h
root         142     139  0 18:09 ?        00:00:00 sleep 6h
hacker       143     140  1 18:09 ?        00:00:00 /usr/bin/python /challenge/decoy
hacker       145       0  1 18:09 pts/0    00:00:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interactive-5.2p37/
hacker       151     145  0 18:09 pts/0    00:00:00 /run/dojo/bin/bash --login
hacker       160     151  0 18:09 pts/0    00:00:00 ps -ef
hacker@processes~killing-misbehaving-processes:~$ kill 140
bash: kill: (140) - Operation not permitted
```

## What I learned
It was a practice exercise

## References 
None
