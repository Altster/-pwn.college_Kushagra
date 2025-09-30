# Challenge Name
Adding commands

## My solve
**Flag:** `pwn.college{4Gn7OxAxKYsbwqaO4lONfD6dy4C.QX2cjM1wCM2gjNzEzW}`

I thought I could directly add win to the PATH, but later realised that I needed to create a directory, and have win within it, and then set that directory as PATH
```bash
hacker@path~adding-commands:~$ mkdir ./script
hacker@path~adding-commands:~$ cat > ~/script/win << 'EOF'
> #!/bin/bash
> /bin/cat /flag
> EOF
hacker@path~adding-commands:~$ chmod a+x ~/script/win
hacker@path~adding-commands:~$ PATH=~/script
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
pwn.college{4Gn7OxAxKYsbwqaO4lONfD6dy4C.QX2cjM1wCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@path~adding-commands:~$ touch win
hacker@path~adding-commands:~$ cat > win << 'EOF'
> #!/bin/bash
> /flag
> EOF
hacker@path~adding-commands:~$ PATH=/home/hacker/win
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
/challenge/run: line 4: win: command not found
It looks like that did not work... Did you set PATH correctly?
```

## What I learned
How to add my own command to the PATH, allowing me to make my own easily accessible commands

## References
None
