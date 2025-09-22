# Challenge Name
Matching with *

## My solve
**Flag:** `pwn.college{A7GTVOg_OXPfQlQv8VSg-zPKRCV.QXxIDO0wCM2gjNzEzW}`

I thought I should write `ch*` isntead of `c*` because I assumed many files would be named starting with c. But I knew that there is only one file starting with r in challenge, so I inputed `r*`
```bash
hacker@globbing~matching-with-:~$ cd /ch*
hacker@globbing~matching-with-:/challenge$ /ch*/r*
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{A7GTVOg_OXPfQlQv8VSg-zPKRCV.QXxIDO0wCM2gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
How to write the file path *, making it much easier

## References 
None
