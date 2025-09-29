# Challenge Name
Switching windows

## My solve
**Flag:** `pwn.college{oqX42bP4aTKTILgyShShACGZ9m0.0FO4IDOxwCM2gjNzEzW}`

```bash
hacker@terminal-multiplexing~switching-windows:~$ screen -r
```
Window 1
```bash
Welcome to the window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-A 0 to switch to window 0!
MSG
hacker@terminal-multiplexing~switching-windows:~$  cat <<MSG
> Welcome to the window switching challenge!
> You are currently in window 1.
> The flag is hidden in window 0.
> Use Ctrl-A 0 to switch to window 0!
> MSG
Welcome to the window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-A 0 to switch to window 0!
```
Window 0
```bash
hacker@terminal-multiplexing~switching-windows:~$  cat <<MSG
> Excellent work! You found window 0!
> Here is your flag: pwn.college{oqX42bP4aTKTILgyShShACGZ9m0.0FO4IDOxwCM2gjNzEzW}
> MSG
Excellent work! You found window 0!
Here is your flag: pwn.college{oqX42bP4aTKTILgyShShACGZ9m0.0FO4IDOxwCM2gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
How to start windows within a screen session, and how to toggle between them

## References 
None
