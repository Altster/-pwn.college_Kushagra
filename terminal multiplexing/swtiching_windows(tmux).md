# Challenge Name
Switching windows (tmux)

## My solve
**Flag:** `pwn.college{4RRkrx2V6GSO92HfW2KwZZj0oaM.0FM5IDOxwCM2gjNzEzW}`

```bash
hacker@terminal-multiplexing~switching-windows-tmux:~$ tmux ls
challenge_session: 2 windows (created Mon Sep 29 10:45:24 2025)
hacker@terminal-multiplexing~switching-windows-tmux:~$ tmux a
```
Window 1
```bash
hacker@terminal-multiplexing~switching-windows-tmux:~$  cat <<MSG
> Welcome to the tmux window switching challenge!
> You are currently in window 1.
> The flag is hidden in window 0.
> Use Ctrl-B 0 to switch to window 0!
> MSG
Welcome to the tmux window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-B 0 to switch to window 0!
hacker@terminal-multiplexing~switching-windows-tmux:~$ 11;rgb:0c0c/0c0c/0c0c
```
Window 1
```bash
hacker@terminal-multiplexing~switching-windows-tmux:~$  cat <<MSG
> Excellent work! You found window 0!
> Here is your flag: pwn.college{4RRkrx2V6GSO92HfW2KwZZj0oaM.0FM5IDOxwCM2gjNzEzW}
> MSG
Excellent work! You found window 0!
Here is your flag: pwn.college{4RRkrx2V6GSO92HfW2KwZZj0oaM.0FM5IDOxwCM2gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
How to navigate between windows in tmux

## References 
None
