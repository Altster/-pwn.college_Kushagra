# Challenge Name
Scripting with multiple conditions

## My solve
**Flag:** `pwn.college{QWmufhjHkmVoY3O0hFcm42kpPs2.0FOzMDOxwCM2gjNzEzW}`

```bash
hacker@chaining~scripting-with-multiple-conditions:~$ touch solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ cat > solve.sh << 'EOF'
> #!/bin/bash
> if [ "$1" == "hack" ]
> then
> echo "the planet"
> elif [ "$1" == "pwn" ]
> then
> echo college
> elif [ "$1" == "learn" ]
> then
> echo linux
> else
> echo unknown
> fi
> EOF
hacker@chaining~scripting-with-multiple-conditions:~$ chmod a+x solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ /challenge/run
Correct! Your script properly handles all the conditions with elif.
Here's your flag:
pwn.college{QWmufhjHkmVoY3O0hFcm42kpPs2.0FOzMDOxwCM2gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
How to implement multiple conditionals

## References
None
