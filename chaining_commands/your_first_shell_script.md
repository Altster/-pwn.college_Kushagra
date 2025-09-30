# Challenge Name
Your first shell script

## My solve
**Flag:** `pwn.college{QYqxGY7-yhMfygo2VfdmsoTdaAp.QXxcDO0wCM2gjNzEzW}`

```bash
hacker@chaining~your-first-shell-script:~$ touch x.sh
hacker@chaining~your-first-shell-script:~$ cat > x.sh << 'EOF'
> /challenge/pwn
> /challenge/college
> EOF
hacker@chaining~your-first-shell-script:~$ bash x.sh
Great job, you've written your first shell script! Here is the flag:
pwn.college{QYqxGY7-yhMfygo2VfdmsoTdaAp.QXxcDO0wCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@chaining~your-first-shell-script:~$ /challenge/pwn > x; /challenge/college > x
It looks like you may have chained the pwn command with a pipe or other input
redirection method. In this level, you must script the commands to run one
after the other, without piping or redirection!
```
```bash
hacker@chaining~your-first-shell-script:~$ /challenge/pwn > x.sh; /challenge/college > x.sh; cat x.sh
It looks like you may have chained the pwn command with a pipe or other input
redirection method. In this level, you must script the commands to run one
after the other, without piping or redirection!
```

## What I learned
How to create a shell script

## References 
None
