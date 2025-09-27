# Challenge Name
Becoming root with su

## My solve
**Flag:** `pwn.college{YBHcHmQzr0Tg51-MFcTG4btDxYi.QX1UDN1wCM2gjNzEzW}`

```bash
hacker@users~becoming-root-with-su:~$ su
Password:
root@users~becoming-root-with-su:/home/hacker# cat /flag
pwn.college{YBHcHmQzr0Tg51-MFcTG4btDxYi.QX1UDN1wCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@users~becoming-root-with-su:~$ su
Password:
root@users~becoming-root-with-su:/home/hacker# cat flag
pwn.college{canhVO7pW10lXDFhMU_WAX1J3tp.QXxcTN0wCM2gjNzEzW}   <--- incorrect flag
```

```bash
hacker@users~becoming-root-with-su:~$ su
Password:
root@users~becoming-root-with-su:/home/hacker# cat flag
pwn.college{canhVO7pW10lXDFhMU_WAX1J3tp.QXxcTN0wCM2gjNzEzW}
root@users~becoming-root-with-su:/home/hacker# cd /challenge/run
bash: cd: /challenge/run: Not a directory
root@users~becoming-root-with-su:/home/hacker# ls
COLLEGE  Desktop  PWN  cmd_output  flag  instructions  link  link_to_flag  myflag  not-the-flag  the-flag
root@users~becoming-root-with-su:/home/hacker# cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{oRye4JYMovYPrWJ84z9XUYs2w6x.QX3YTN0wCM2gjNzEzW}
```

## What I learned
The 2 commands used to access root access of a system, and how the `su` command works, and how outdated it is

## References 
None
