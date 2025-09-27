# Challenge Name
Cracking passwords

## My solve
**Flag:** `pwn.college{YYyxPL5MJ8FFrWCSStEHKhLgIpZ.QX3UDN1wCM2gjNzEzW}`

```bash
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
aardvark         (zardus)
1g 0:00:00:20 100% 2/3 0.04878g/s 284.0p/s 284.0c/s 284.0C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{YYyxPL5MJ8FFrWCSStEHKhLgIpZ.QX3UDN1wCM2gjNzEzW}
```
## Incorrect tangents I went on
```bash
hacker@users~cracking-passwords:~$ cat /challenge/shadow-leak
root:*:20182:0:99999:7:::
daemon:*:20182:0:99999:7:::
bin:*:20182:0:99999:7:::
sys:*:20182:0:99999:7:::
sync:*:20182:0:99999:7:::
games:*:20182:0:99999:7:::
man:*:20182:0:99999:7:::
lp:*:20182:0:99999:7:::
mail:*:20182:0:99999:7:::
news:*:20182:0:99999:7:::
uucp:*:20182:0:99999:7:::
proxy:*:20182:0:99999:7:::
www-data:*:20182:0:99999:7:::
backup:*:20182:0:99999:7:::
list:*:20182:0:99999:7:::
irc:*:20182:0:99999:7:::
gnats:*:20182:0:99999:7:::
nobody:*:20182:0:99999:7:::
_apt:*:20182:0:99999:7:::
systemd-timesync:*:20357:0:99999:7:::
systemd-network:*:20357:0:99999:7:::
systemd-resolve:*:20357:0:99999:7:::
mysql:!:20357:0:99999:7:::
messagebus:*:20357:0:99999:7:::
sshd:*:20357:0:99999:7:::
hacker::20357:0:99999:7:::
zardus:$6$Vg6xU6i1MgHKiDvJ$6j8YwiPZopJMIY0uJEEaO7yDHj7ZkPkE6o6OcqECefprDjgqeP5XQjKWUD7xAL7Dlx9bSXA09/ccH6dDlxJu//:20358:0:99999:7:::
```

## What I learned
How the leak of any passwords hash value can be fatal

## References 
None
