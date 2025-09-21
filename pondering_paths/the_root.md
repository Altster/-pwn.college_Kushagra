# Challenge Name
Access a file named "pwn" using its absolute path

## My solve
**Flag:** `pwn.college{ItNGgLRC9Sy2ne_zbd8yY1hGUe0.QX4cTO0wCM2gjNzEzW}`

While solving, I was wondering whether I should use "cat" command or not.
It wasn't needed to be used, so now I wonder why that is, because cat is the command needed to display the contents of a file. Then why is /pwn displaying the flag?

```bash
hacker@paths~the-root:~$ /pwn
BOOM!!!
Here is your flag:
pwn.college{ItNGgLRC9Sy2ne_zbd8yY1hGUe0.QX4cTO0wCM2gjNzEzW}
hacker@paths~the-root:~$ cat /pwn
#!/bin/bash

/challenge/.pwn
```

## What I learned
accessing files and the meaning of absolute path

## References 
None
