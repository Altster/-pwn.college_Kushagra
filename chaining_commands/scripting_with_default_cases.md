# Challenge Name
Scripting with default cases

## My solve
**Flag:** `pwn.college{Mt_r3RsFai5YO36Z3jaSD0g22Ua.01NzMDOxwCM2gjNzEzW}`

```bash
hacker@chaining~scripting-with-default-cases:~$ touch solve.sh
hacker@chaining~scripting-with-default-cases:~$ cat > solve.sh << 'EOF'
> #!/bin/bash
> if [ "$1" == "pwn" ]
> then
> echo college
> else
> echo nope
> fi
> EOF
hacker@chaining~scripting-with-default-cases:~$ chmod a+x solve.sh
hacker@chaining~scripting-with-default-cases:~$ /challenge/run
Correct! Your script properly handles the if/else conditions.
Here's your flag:
pwn.college{Mt_r3RsFai5YO36Z3jaSD0g22Ua.01NzMDOxwCM2gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
How to implement `else` case in the if conditional

## References
None
