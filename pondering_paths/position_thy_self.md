# Challenge Name
It requires the use of cd to first find the path leading to the correct file, and then find the flag in that file

## My solve
**Flag:** `pwn.college{0JdutnenHhEUjuCydfbJdAtRJmT.QX2QTN0wCM2gjNzEzW}`

```bash
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /var/log directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd /var/log directory
bash: cd: too many arguments
hacker@paths~position-thy-self:~$ cd /var/log
hacker@paths~position-thy-self:/var/log$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{0JdutnenHhEUjuCydfbJdAtRJmT.QX2QTN0wCM2gjNzEzW}
```

## What I learned
The function of 'cd', and that it takes only 1 argument

## References 
None
