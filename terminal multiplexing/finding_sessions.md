# Challenge Name
Finding sessions

## My solve
**Flag:** `pwn.college{Y_O0sIEN5IrzTr0r05m0IyQUk7X.01N4IDOxwCM2gjNzEzW}`

Searched each screen one-by-one and detached from each one after looking into them
```bash
hacker@terminal-multiplexing~finding-sessions:~$ screen -ls
There are screens on:
        150.pts-0.terminal-multiplexing~launching-screen        (Remote or dead)
        139.pts-0.terminal-multiplexing~detaching-and-attaching (Remote or dead)
        144.session_b843ff6aef928aaa    (Remote or dead)
        147.session_3fa741c68d4c8bd5    (Remote or dead)
        150.session_2385bc42857aacef    (Remote or dead)
        144.session_20cae7eb4ea72fe9    (Detached)
        147.session_8b23508894e1539d    (Detached)
        150.session_df13773869b206e5    (Detached)
8 Sockets in /home/hacker/.screen.
hacker@terminal-multiplexing~finding-sessions:~$ screen -r 144
Remove dead screens with 'screen -wipe'.
[detached from 144.session_20cae7eb4ea72fe9]
hacker@terminal-multiplexing~finding-sessions:~$ screen -wipe
There are screens on:
        150.pts-0.terminal-multiplexing~launching-screen        (Remote or dead)
        139.pts-0.terminal-multiplexing~detaching-and-attaching (Remote or dead)
        144.session_b843ff6aef928aaa    (Remote or dead)
        147.session_3fa741c68d4c8bd5    (Remote or dead)
        150.session_2385bc42857aacef    (Remote or dead)
        144.session_20cae7eb4ea72fe9    (Detached)
        147.session_8b23508894e1539d    (Detached)
        150.session_df13773869b206e5    (Detached)
8 Sockets in /home/hacker/.screen.
hacker@terminal-multiplexing~finding-sessions:~$ screen -r 147
Remove dead screens with 'screen -wipe'.
[detached from 147.session_8b23508894e1539d]
hacker@terminal-multiplexing~finding-sessions:~$ screen -r 150
Remove dead screens with 'screen -wipe'.
[detached from 150.session_df13773869b206e5]
```
Screen 144
```bash
hacker@terminal-multiplexing~finding-sessions:~$  echo 'Wrong session! Keep looking.'
Wrong session! Keep looking.
```
Screen 147
```bash
hacker@terminal-multiplexing~finding-sessions:~$  echo 'Wrong session! Keep looking.'
Wrong session! Keep looking.
```
Screen 150
```bash
hacker@terminal-multiplexing~finding-sessions:~$  echo 'Congratulations! You found the right session!'
Congratulations! You found the right session!
hacker@terminal-multiplexing~finding-sessions:~$  echo pwn.college{Y_O0sIEN5IrzTr0r05m0IyQUk7X.01N4IDOxwCM2gjNzEzW}
pwn.college{Y_O0sIEN5IrzTr0r05m0IyQUk7X.01N4IDOxwCM2gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
How to see a list of all the screens and reconnect to a particular one 

## References 
None
