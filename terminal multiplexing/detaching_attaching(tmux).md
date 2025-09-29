# Challenge Name
Detaching attaching (tmux)

## My solve
**Flag:** `pwn.college{0rz9mAIwSA_aBS8SZKg51M4EHfZ.0VO4IDOxwCM2gjNzEzW}`

```bash
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ tmux
[detached (from session 0)]
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ /challenge/run
Found detached tmux session: 0
Sending flag to your tmux session...

Flag sent! Now reattach to your tmux session with:
  tmux attach

You'll find the flag waiting for you there!
```
Window
```
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$  echo Congratulations, here is your flag: pwn.college{0rz9mAIwSA_aBS8SZKg51M4EHfZ.0VO4IDOxwCM2gjNzEzW}
Congratulations, here is your flag: pwn.college{0rz9mAIwSA_aBS8SZKg51M4EHfZ.0VO4IDOxwCM2gjNzEzW}
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ 10;rgb:cccc/cccc/cccc
```
## Incorrect tangents I went on
None

## What I learned
I learned about another form of screens, called tmux

## References 
None
