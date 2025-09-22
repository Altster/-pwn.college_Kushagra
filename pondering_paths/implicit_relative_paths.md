# Challenge Name
implicit relative paths, from /

## My solve
**Flag:** `pwn.college{kugfm-fqbmSLPSoF7yqyl3KwuK8.QX5QTN0wCM2gjNzEzW}`

I finally understood the meaning of ~
```bash
hacker@paths~implicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{kugfm-fqbmSLPSoF7yqyl3KwuK8.QX5QTN0wCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ /challenge/run
Incorrect...
You invoked this challenge with an absolute path. This challenge needs a relative path!
```

## What I learned
Understood the difference between absolute and relative paths

## References 
None
