# Challenge Name
Scripting with arguments

## My solve
**Flag:** `pwn.college{QmdZNdzSPK1YfL4dLqv9qZil7qd.0VNzMDOxwCM2gjNzEzW}`

At first, I thought I needed to define firsthand how many arguments the file will take, but then realised that there is no restriction on that, and I can have it take as many arguments as I need while writing the script itself.
```bash
hacker@chaining~scripting-with-arguments:~$ touch solve.sh
hacker@chaining~scripting-with-arguments:~$ cat > solve.sh << 'EOF'
#!/bin/bash
echo "$2 $1"
EOF
hacker@chaining~scripting-with-arguments:~$ /challenge/run
Correct! Your script properly reversed the arguments.
Here's your flag:
pwn.college{QmdZNdzSPK1YfL4dLqv9qZil7qd.0VNzMDOxwCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@chaining~scripting-with-arguments:~$ touch solve.sh
hacker@chaining~scripting-with-arguments:~$ cat > solve.sh a b << 'EOF'
> #!/bin/bash
> echo $2
> echo $1
> EOF
cat: a: No such file or directory
cat: b: No such file or directory
```
```bash
hacker@chaining~scripting-with-arguments:~$ touch solve.sh
hacker@chaining~scripting-with-arguments:~$ cat > solve.sh << 'EOF'
#!/bin/bash
echo $2
echo $1
EOF
hacker@chaining~scripting-with-arguments:~$ /challenge/run
Not quite right!
Expected: college_JY6kRjupUg pwn_u0nAXg7xvs
Got: college_JY6kRjupUg
pwn_u0nAXg7xvs
```

## What I learned
How to have my shell script take arguments, and access these arguments in the script

## References
None
