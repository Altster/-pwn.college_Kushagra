# Challenge Name
Reading shell scripts

## My solve
**Flag:** `pwn.college{0YLLVXSS_1b2Hple7p_5hfa0ed0.0lMwgDOxwCM2gjNzEzW}`

I thought I need to pass "hack the PLANET" as argument, but when I read the `read GUESS`, I realised that I am supposed to pass it to the stdin of `/challenge/run`
```bash
hacker@chaining~reading-shell-scripts:~$ cat /challenge/run
#!/opt/pwn.college/bash

read GUESS
if [ "$GUESS" == "hack the PLANET" ]
then
        echo "CORRECT! Your flag:"
        cat /flag
else
        echo "Read the /challenge/run file to figure out the correct password!"
fi
hacker@chaining~reading-shell-scripts:~$ echo 'hack the PLANET' | /challenge/run
CORRECT! Your flag:
pwn.college{0YLLVXSS_1b2Hple7p_5hfa0ed0.0lMwgDOxwCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@chaining~reading-shell-scripts:~$ cat /challenge/run
#!/opt/pwn.college/bash

read GUESS
if [ "$GUESS" == "hack the PLANET" ]
then
        echo "CORRECT! Your flag:"
        cat /flag
else
        echo "Read the /challenge/run file to figure out the correct password!"
fi
hacker@chaining~reading-shell-scripts:~$ /challenge/run "hack the PLANET"
```

## What I learned
How to read a shell script

## References
None
