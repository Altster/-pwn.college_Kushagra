# Challenge Name
Exporting variables

## My solve
**Flag:** `pwn.college{wk8-SrHU5ke2eD5iJe2LH3uyivl.QXyYTN0wCM2gjNzEzW}`

```bash
hacker@variables~exporting-variables:~$ PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ export PWN
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run PWN
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{wk8-SrHU5ke2eD5iJe2LH3uyivl.QXyYTN0wCM2gjNzEzW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
```

## Incorrect tangents I went on
None

## What I learned
The fact that variables are "local", can how to export them to make them "global"

## References 
None
