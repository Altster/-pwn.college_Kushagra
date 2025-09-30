# Challenge Name
understanding shebangs

## My solve
**Flag:** `pwn.college{oaipcr4aAkqYkLqyvjSKW0_HmdC.0VOzMDOxwCM2gjNzEzW}`

```bash
hacker@chaining~understanding-shebangs:~$ touch solve.sh
hacker@chaining~understanding-shebangs:~$ cat > solve.sh << 'EOF'
> #!/bin/bash
> echo "hack the planet"
> EOF
hacker@chaining~understanding-shebangs:~$ chmod a+x solve.sh
hacker@chaining~understanding-shebangs:~$ /challenge/run
Testing your script...
Perfect! Your flag:
Flag: pwn.college{oaipcr4aAkqYkLqyvjSKW0_HmdC.0VOzMDOxwCM2gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
That the shell script must begin with a `shebang` to set the interpreter

## References
None
