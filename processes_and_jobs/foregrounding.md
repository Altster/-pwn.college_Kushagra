# Challenge Name
Foregrounding processes

## My solve
**Flag:** `pwn.college{sjQmNVgEMZQAD9cBvoonDolKmwL.QX4QDO0wCM2gjNzEzW}`

```bash
hacker@processes~foregrounding-processes:~$ /challenge/run
To pass this level, you need to suspend me, resume the suspended process in the
background, and *then* foreground it without re-suspending it! You can
background me with Ctrl-Z (and resume me in the background with 'bg') or, if
you're not ready to do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~foregrounding-processes:~$ bg /challenge/run
[1]+ /challenge/run &
hacker@processes~foregrounding-processes:~$


Yay, I'm now running the background! Because of that, this text will probably
overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times
to scroll this text out. After that, resume me into the foreground with 'fg';
I'll wait.

hacker@processes~foregrounding-processes:~$ fg /challenge/run
/challenge/run
YES! Great job! I'm now running in the foreground. Hit Enter for your flag!

pwn.college{sjQmNVgEMZQAD9cBvoonDolKmwL.QX4QDO0wCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@processes~foregrounding-processes:~$ /challenge/run
To pass this level, you need to suspend me, resume the suspended process in the
background, and *then* foreground it without re-suspending it! You can
background me with Ctrl-Z (and resume me in the background with 'bg') or, if
you're not ready to do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~foregrounding-processes:~$ fg /challenge/run
/challenge/run
You resumed me into the foreground from suspension! Please resume me into the
background, and *then* swap me into the foreground directly from there (or
press Enter, and I'll exit).
```

## What I learned
How to foreground a background process

## References 
None
