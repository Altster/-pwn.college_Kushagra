# Challenge Name
An epic filesystem quest

## My solve
**Flag:** `pwn.college{Ab6Kqf6qdmP66tUV5YMXLXWNut1.QX5IDO0wCM2gjNzEzW}`

```bash
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls -a
.   .dockerenv  bin   challenge  etc   home  lib32  libx32  mnt  opt   root  sbin  sys  usr
..  DOSSIER     boot  dev        flag  lib   lib64  media   nix  proc  run   srv   tmp  var
hacker@commands~an-epic-filesystem-quest:/$ cat DOSSIER
Tubular find!
The next clue is in: /usr/lib/jvm/java-11-openjdk-amd64/legal/java.naming

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/lib/jvm/java-11-openjdk-amd64/legal/java.naming
ASSEMBLY_EXCEPTION  MESSAGE-TRAPPED
hacker@commands~an-epic-filesystem-quest:/$ cat MESSAGE-TRAPPED
cat: MESSAGE-TRAPPED: No such file or directory
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/lib/jvm/java-11-openjdk-amd64/legal/java.naming/MESSAGE-TRAPPED
Yahaha, you found me!
The next clue is in: /usr/share/doc/libasound2
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/share/doc/libasound2
cat: /usr/share/doc/libasound2: Is a directory
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/share/doc/libasound2
NEWS.Debian.gz  NOTE  changelog.Debian.gz  copyright  examples
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/share/doc/libasound2/NOTE
Yahaha, you found me!
The next clue is in: /usr/share/racket/pkgs/net-lib/net

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/share/racket/pkgs/net-lib/net
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/net-lib/net$ ls
SNIPPET   cookie.rkt  imap.rkt       nntp.rkt  qp.rkt        smtp.rkt          tcp-sig.rkt
cgi.rkt   dns.rkt     mime-util.rkt  pop3.rkt  sendmail.rkt  ssl-tcp-unit.rkt  tcp-unit.rkt
compiled  ftp.rkt     mime.rkt       private   sendurl.rkt   tcp-redirect.rkt  unihead.rkt
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/net-lib/net$ cat SNIPPET
Great sleuthing!
The next clue is in: /usr/share/racket/pkgs/gui-lib/hierlist/compiled

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/net-lib/net$ ls -a /usr/share/racket/pkgs/gui-lib/hierlist/compiled
.  ..  .TRACE  hierlist_rkt.dep  hierlist_rkt.zo
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/net-lib/net$ cat .TRACE
cat: .TRACE: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/net-lib/net$ cat /usr/share/racket/pkgs/gui-lib/hierlist/compiled/.TRACE
Great sleuthing!
The next clue is in: /opt/linux/linux-5.4/arch/hexagon/include/uapi/asm

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/net-lib/net$ ls -a /opt/linux/linux-5.4/arch/hexagon/include/uapi/asm
.   .CLUE   bitsperlong.h  param.h   registers.h  sigcontext.h  swab.h    user.h
..  Kbuild  byteorder.h    ptrace.h  setup.h      signal.h      unistd.h
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/net-lib/net$ cat /opt/linux/linux-5.4/arch/hexagon/include/uapi/asm/.CLUE
Yahaha, you found me!
The next clue is in: /usr/share/racket/pkgs/redex-pict-lib/redex/private/compiled

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/net-lib/net$ ls -a /usr/share/racket/pkgs/redex-pict-lib/redex/private/compiled
.         arrow_rkt.dep        core-layout_rkt.zo       derivations-layout_rkt.dep  pict_rkt.zo
..        arrow_rkt.zo         derivation-pict_rkt.dep  derivations-layout_rkt.zo
.SPOILER  core-layout_rkt.dep  derivation-pict_rkt.zo   pict_rkt.dep
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/net-lib/net$ cat /usr/share/racket/pkgs/redex-pict-lib/redex/private/compiled/.SPOILER
Great sleuthing!
The next clue is in: /opt/linux/linux-5.4/include/config/dmi
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/net-lib/net$ ls /opt/linux/linux-5.4/include/config/dmi
POINTER  scan
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/net-lib/net$ cat /opt/linux/linux-5.4/include/config/dmi/POINTER
Tubular find!
The next clue is in: /usr/local/lib/python3.8/dist-packages/pip/_vendor/truststore

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/net-lib/net$ cd /usr/local/lib/python3.8/dist-packages/pip/_vendor/truststore
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/pip/_vendor/truststore$ ls
REVELATION  __init__.py  __pycache__  _api.py  _macos.py  _openssl.py  _ssl_constants.py  _windows.py  py.typed
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/pip/_vendor/truststore$ cat REVELATION
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{Ab6Kqf6qdmP66tUV5YMXLXWNut1.QX5IDO0wCM2gjNzEzW}
```

## Incorrect tangents I went on
None

## What I learned
Built an instinct on the difference between the way to access a directory and a file

## References 
Mentor
