# Challenge Name
Linking files

## My solve
**Flag:** `pwn.college{IM7NC335GKWd2lzZE4F7YtZFNz8.QX5ETN1wCM2gjNzEzW}`

I first tried to create a link to `/flag` using an entirely new variable `link_to_flag`, but it denied access. Then I thought, if `/challenge/catfish` already links to `/home/hocker/not-the-flag`, why don't I change that itself
```bash
hacker@commands~linking-files:~$ ln -s /flag /home/hacker/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{IM7NC335GKWd2lzZE4F7YtZFNz8.QX5ETN1wCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@commands~linking-files:~$ ln -s /challenge/catflag link_to_flag
hacker@commands~linking-files:~$ cat link_to_flag
#!/opt/pwn.college/bash

fold -s <<< "About to read out the /home/hacker/not-the-flag file!"
cat /home/hacker/not-the-flag
```

## What I learned
Meaning of hard a soft links, and how to execute soft link

## References 
None
