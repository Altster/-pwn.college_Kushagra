# Challenge Name
Executable shell scripts

## My solve
**Flag:** `pwn.college{sy2K7pkHC3QjwfVGI7dT3rpyYJm.QX0cjM1wCM2gjNzEzW}`

```bash
hacker@chaining~executable-shell-scripts:~$ touchx.sh
bash: touchx.sh: command not found
hacker@chaining~executable-shell-scripts:~$ touch x.sh
hacker@chaining~executable-shell-scripts:~$ cat > x.sh << 'EOF'
> /challenge/solve
> EOF
hacker@chaining~executable-shell-scripts:~$ chmod +x x.sh
hacker@chaining~executable-shell-scripts:~$ ./x.sh
Congratulations on your shell script execution! Your flag:
pwn.college{sy2K7pkHC3QjwfVGI7dT3rpyYJm.QX0cjM1wCM2gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
It is more convenient to make a shell script executable instead of calling it using bash

## References
None
