# Challenge Name
Process exit codes

## My solve
**Flag:** `pwn.college{4T0yE1PablYDNzVGzfOpYdHKF5B.QX5YDO1wCM2gjNzEzW}`

```bash
hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
168
hacker@processes~process-exit-codes:~$ /challenge/submit-code 168
CORRECT! Here is your flag:
pwn.college{4T0yE1PablYDNzVGzfOpYdHKF5B.QX5YDO1wCM2gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
How to find the exit code of the most recent command

## References 
None
