# Challenge Name
comparing files

## My solve
**Flag:** `> pwn.college{UpOq8ldCht1W2VoYCVpVQCbDZlI.01MwMDOxwCM2gjNzEzW}`

I am wondering why it is `87a88`. Shouldn't it have been `100a101` because there are 100 fakes and 1 real
```bash
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
87a88
> pwn.college{UpOq8ldCht1W2VoYCVpVQCbDZlI.01MwMDOxwCM2gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
The use of `diff` 

## References 
None
