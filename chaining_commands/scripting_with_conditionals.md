# Challenge Name
Scripting with conditionals

## My solve
**Flag:** `pwn.college{8ehBi8ifBUf1JCdZ121uD3OvQpp.0lNzMDOxwCM2gjNzEzW}`

```bash
hacker@chaining~scripting-with-conditionals:~$ touch solve.sh
hacker@chaining~scripting-with-conditionals:~$ cat > solve.sh << 'EOF'
> #!/bin/bash
> if [ "$1" == "pwn" ]
> then
> echo college
> fi
> EOF
hacker@chaining~scripting-with-conditionals:~$ chmod a+x solve.sh
hacker@chaining~scripting-with-conditionals:~$ /challenge/run
Correct! Your script properly handles all the conditions.
Here's your flag:
pwn.college{8ehBi8ifBUf1JCdZ121uD3OvQpp.0lNzMDOxwCM2gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
How to implement conditionals in shell script

## References
None
