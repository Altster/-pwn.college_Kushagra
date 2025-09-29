# Challenge Name
Detaching and attaching

## My solve
**Flag:** `pwn.college{kDePBmQo7qvP6xLHY26PUevVpaT.0lN4IDOxwCM2gjNzEzW}`

```bash
hacker@terminal-multiplexing~detaching-and-attaching:~$ screen
```
```bash
[detached from 139.pts-0.terminal-multiplexing~detaching-and-attaching]
hacker@terminal-multiplexing~detaching-and-attaching:~$ /challenge/run
Found detached screen session: 139.pts-0.terminal-multiplexing~detaching-and-attaching
Sending flag to your screen session...

Flag sent! Now reattach to your screen session with:

  screen -r

You'll find the flag waiting for you there!
hacker@terminal-multiplexing~detaching-and-attaching:~$ screen -r
```
```bash
hacker@terminal-multiplexing~detaching-and-attaching:~$ echo Yes! Flag is: pwn.college{kDePBmQo7qvP6xLHY26PUevVpaT.0lN4IDOxwCM2gjNzEzW}
Yes! Flag is: pwn.college{kDePBmQo7qvP6xLHY26PUevVpaT.0lN4IDOxwCM2gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
How to detach from a screen session, returning to the normal terminal, and also how to reattach the screen

## References 
None
