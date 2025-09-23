# Challenge Name
Process substitution for input

## My solve
**Flag:** `< pwn.college{IhWR8I-Acz5XKU5Kr43VwXcpAQq.0lNwMDOxwCM2gjNzEzW}`

```bash
hacker@piping~process-substitution-for-input:~$ diff <(/challenge/print_decoys_and_flag) <(/challenge/print_decoys)
45d44
< pwn.college{IhWR8I-Acz5XKU5Kr43VwXcpAQq.0lNwMDOxwCM2gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
How to pass the output of commands as the input to diff command and compare 2 files

## References 
None
