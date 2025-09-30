# Challenge Name
Redirecting script output

## My solve
**Flag:** `pwn.college{wC_XD0F4M0ICUKYXLY2t4iLBzUG.QX4ETO0wCM2gjNzEzW}`

```bash
hacker@chaining~redirecting-script-output:~$ touch x.sh
hacker@chaining~redirecting-script-output:~$ cat > x.sh << 'EOF'
/challenge/pwn
/challenge/college
EOF
hacker@chaining~redirecting-script-output:~$ bash x.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{wC_XD0F4M0ICUKYXLY2t4iLBzUG.QX4ETO0wCM2gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
The significance of shell scripts as a cluster of commands

## References 
None
