# Challenge Name
The SUID bit

## My solve
**Flag:** `pwn.college{4KJ8k502R77wZoF2Unk9qr4PltI.QXzEjN0wCM2gjNzEzW}`

```bash
hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# cat /flag
pwn.college{4KJ8k502R77wZoF2Unk9qr4PltI.QXzEjN0wCM2gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
What an SUID bit is, and how to set it

## References 
None
