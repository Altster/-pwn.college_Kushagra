# Challenge Name
Searching for manuals

## My solve
**Flag:** `pwn.college{gq20TnCa5infektskNuZOUS2U2U.QX2EDO0wCM2gjNzEzW}`

The man man database gave me the argument for man that wwould help me find the name of the challenge function. Then `man` on that game the instructions to get the flag
```bash
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -k challenge
gqnainfekt (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man gqnainfekt
hacker@man~searching-for-manuals:~$ /challenge/challenge --gqnain 205
Correct usage! Your flag: pwn.college{gq20TnCa5infektskNuZOUS2U2U.QX2EDO0wCM2gjNzEzW}
```

## Incorrect tangents I went on
I thought I should search for `/flag` or `/challenge/challenge` in the man manpage, but didn't find it. Was stuck on it for 10 minutes, then decided to actually read the documentation, and found the answer
AND
```bash
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -f challenge
challenge: nothing appropriate.
```
AND
```bash
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -k challenge
gqnainfekt (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ /gqnainfekt
bash: /gqnainfekt: No such file or directory
```

## What I learned
How useful documentation can be

## References 
None
