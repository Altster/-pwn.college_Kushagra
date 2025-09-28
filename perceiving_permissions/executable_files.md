# Challenge Name
Executable files

## My solve
**Flag:** `pwn.college{482X_h6divMPkBFljH6kXk_8fe3.QXyEjN0wCM2gjNzEzW}`

```bash
hacker@permissions~executable-files:~$ cd /challenge
hacker@permissions~executable-files:/challenge$ chmod u+x run
hacker@permissions~executable-files:/challenge$ ./run
Successful execution! Here is your flag:
pwn.college{482X_h6divMPkBFljH6kXk_8fe3.QXyEjN0wCM2gjNzEzW}
```
## Incorrect tangents I went on
```bash
hacker@permissions~executable-files:~$ ls -l
total 40
-rw-r--r-- 1 hacker hacker   4 Sep 22 19:29 COLLEGE
drwxr-xr-x 1 hacker hacker   0 Sep 21 11:02 Desktop
-rw-r--r-- 1 hacker hacker   8 Sep 23 13:29 PWN
-rw-r--r-- 1 root   hacker  77 Sep 23 14:00 cmd_output
-rwxrwxrwx 1 hacker root    60 Sep 27 10:46 flag
-rw-r--r-- 1 hacker hacker 829 Sep 22 20:35 instructions
lrwxrwxrwx 1 hacker hacker   5 Sep 22 14:34 link -> /flag
lrwxrwxrwx 1 hacker hacker   5 Sep 22 14:24 link_to_flag -> /flag
-rw-r--r-- 1 hacker hacker  95 Sep 22 20:35 myflag
lrwxrwxrwx 1 hacker hacker   5 Sep 22 14:38 not-the-flag -> /flag
-rw-r--r-- 1 hacker hacker 437 Sep 22 20:14 the-flag
hacker@permissions~executable-files:~$ cat /flag
cat: /flag: Permission denied
hacker@permissions~executable-files:~$ cd /challenge
hacker@permissions~executable-files:/challenge$ ls -l
total 8
-rwsr-xr-x 1 root   root   1221 Jun  4 14:01 DESCRIPTION.md
-r--r--r-- 1 hacker hacker   32 Jan 14  2025 run
hacker@permissions~executable-files:/challenge$ chmod u+w run
hacker@permissions~executable-files:/challenge$ /run
bash: /run: Is a directory
hacker@permissions~executable-files:/challenge$ /challenge/run
bash: /challenge/run: Permission denied
```

## What I learned
Nothinf  much

## References 
None
