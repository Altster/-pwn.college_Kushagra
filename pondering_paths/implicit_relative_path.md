# Challenge Name
implicit relative path

## My solve
**Flag:** `pwn.college{Eps0bMDm1ZCx3WaKrXpMaSHxi8C.QXxUTN0wCM2gjNzEzW}`

At first I thought that I could access relative path from another directory, but I needed to be in the subdirectory, and the use the relative path
```bash
hacker@paths~implicit-relative-path:~$ cd /
hacker@paths~implicit-relative-path:/$ cd challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{Eps0bMDm1ZCx3WaKrXpMaSHxi8C.QXxUTN0wCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@paths~implicit-relative-path:~$ cd /
hacker@paths~implicit-relative-path:/$ ./challenge/run
Incorrect...
You are not currently in the /challenge directory.
Please use the `cd` utility to change directory appropriately.
```

## What I learned
That `./challenge/run` is different from `cd challenge`, followed by `./run`

## References 
None
