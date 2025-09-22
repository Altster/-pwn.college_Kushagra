# Challenge Name
Explicit relative paths, from /

## My solve
**Flag:** `pwn.college{omiswH0qo2YBkRcX71pEE3z-t8o.QXwUTN0wCM2gjNzEzW}`

I thought I had to use cd, but later realised that it was not needed to access the explicit relative path
```bash
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ cd ./challenge/run
bash: cd: ./challenge/run: Not a directory
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{omiswH0qo2YBkRcX71pEE3z-t8o.QXwUTN0wCM2gjNzEzW}
```

#Incorrect tangents I went on
I tried the `cd ./challenge/run`, but it didnt work. I believed cd was a must in this challenge, so I tried a lot of variations like `cd /challenge/run` and more. I finally asked my mentor about this and he helped me out

## What I learned
The difference between absolute and relative paths, what a checker is, and when cd needs to be used

## References 
Mentor
