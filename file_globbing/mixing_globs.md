# Challenge Name
Mixing globs

## My solve
**Flag:** `pwn.college{8tZQ6311-pv0ScZWJiqn2EPDYzV.QX1IDO0wCM2gjNzEzW}`

```bash
hacker@globbing~mixing-globs:~$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{8tZQ6311-pv0ScZWJiqn2EPDYzV.QX1IDO0wCM2gjNzEzW}
```

## Incorrect tangents I went on
```bash
hacker@globbing~mixing-globs:~$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run *i*n*
Error: you did not use a square bracket glob...
```
```bash
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run *[nw]?
Your expansion did not expand to the requested files (challenging, educational,
pwning). Instead, it expanded to:
amazing challenging kind laughing pwning radiant thrilling uplifting
```
```bash
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run *[na]?
Your expansion did not expand to the requested files (challenging, educational,
pwning). Instead, it expanded to:
amazing challenging educational great jovial kind laughing magical pwning radiant thrilling uplifting xenial
```
```bash
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run *[uw]*
Your expansion did not expand to the requested files (challenging, educational,
pwning). Instead, it expanded to:
beautiful delightful educational laughing pwning queenly uplifting victorious wonderful youthful
```
```bash
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run *[g?]
Your expansion did not expand to the requested files (challenging, educational,
pwning). Instead, it expanded to:
amazing challenging laughing pwning thrilling uplifting
```
```bash
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run ?[g]
Your expansion did not expand to the requested files (challenging, educational,
pwning). Instead, it expanded to:
?[g]
```

## What I learned
How hard it can be to come up with a proper glob combination

## References 
None
