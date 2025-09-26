# Challenge Name
Exctracting specific sections of text

## My solve
**Flag:** `pwn.college{MsH2pwBmSrDdT0vdQ--1XPF7ebc.01NxEzNxwCM2gjNzEzW}`

I first ran `/challenge/run` to see which column no. had the characters of the flag, then proceded with the required command

```bash
hacker@data~extracting-specific-sections-of-text:~$ /challenge/run
5734 p
4968 w
21027 n
10364 .
3903 c
92 o
8070 l
7871 l
16327 e
10713 g
32380 e
11427 {
8797 M
9006 s
9759 H
20220 2
848 p
12806 w
13702 B
5204 m
18765 S
27362 r
9825 D
15217 d
9318 T
22523 0
8290 v
10400 d
10500 Q
17839 -
6808 -
10912 1
9708 X
18646 P
27178 F
9465 7
5300 e
15117 b
2271 c
3558 .
8960 0
22083 1
30641 N
3816 x
13967 E
1468 z
2420 N
14603 x
11993 w
25497 C
29252 M
21200 2
29087 g
6118 j
14297 N
14041 z
1328 E
15174 z
11981 W
17625 }
hacker@data~extracting-specific-sections-of-text:~$ /challenge/run | cut -d " " -f 2 | tr -d "\n"
pwn.college{MsH2pwBmSrDdT0vdQ--1XPF7ebc.01NxEzNxwCM2gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
How to access the elements of a specific column of the given data

## References 
None
