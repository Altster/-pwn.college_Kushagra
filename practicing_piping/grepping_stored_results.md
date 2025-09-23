# Challenge Name
Grepping stored result

## My solve
**Flag:** `pwn.college{ApMCKKockBqJlzIyegmBvQrybVg.QX4EDO0wCM2gjNzEzW}`

```bash
hacker@piping~grepping-stored-results:~$ /challenge/run > /tmp/data.txt
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : /tmp/data.txt
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to a file called /tmp/data.txt. Checking...

[HINT] File descriptors are inherited from the parent, unless the FD_CLOEXEC is set by the parent on the file descriptor.
[HINT] For security reasons, some programs, such as python, do this by default in certain cases. Be careful if you are
[HINT] creating and trying to pass in FDs in python.

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~grepping-stored-results:~$ grep pwn.college /tmp/data.txt
pwn.college{ApMCKKockBqJlzIyegmBvQrybVg.QX4EDO0wCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@piping~grepping-stored-results:~$ grep flag /tmp/data.txt
[FLAG] Here is your flag:
conflagration
flags
flagstaffs
camouflage
flagrantly
camouflaged
camouflages
flagellums
flagellates
flag
flagellating
persiflage's
flagstaff
flagella
flagging
flagpole's
flagellation's
flagellum's
flagstaff's
conflagrations
flagstone's
flagship
flagstone
conflagration's
flagellum
flagship's
flagged
flagons
flagellated
flagellate
flagpole
camouflage's
flagpoles
flagships
flagstones
camouflaging
persiflage
flagon's
unflagging
flagon
flag's
flagrant
flagellation
```

## What I learned
It was a practice challenge

## References 
None
