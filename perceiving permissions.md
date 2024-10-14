# CHANGING FILE OWNERSHIP
Every file is owned by an individual or a group of individuals. And there are some files which can't be accessed by everyone. So in order to access the files we can change the the user from root using the ```chown``` command.
The syntax is ``` chown user filename ```.

```Connected!
hacker@permissions~changing-file-ownership:~$ ls -l
total 44
-rw-r--r-- 1 hacker hacker    4 Oct  8 13:41 COLLEGE
-rw-r--r-- 1 hacker hacker    1 Oct 12 13:30 PWN
drwxr-xr-x 2 hacker hacker 4096 Oct  6 08:46 a
drwxr-xr-x 2 hacker hacker 4096 Oct  3 08:28 cryptos
-rw-r--r-- 1 hacker hacker    0 Oct  8 19:00 error
-rw-r--r-- 1 hacker hacker  757 Oct  8 14:27 errors.log
-rw-r--r-- 1 hacker hacker   58 Oct  6 07:36 f
-rw-r--r-- 1 hacker hacker  829 Oct  8 14:31 instructions
-rw-r--r-- 1 hacker hacker   58 Oct  6 07:39 m
-rw-r--r-- 1 hacker hacker   93 Oct  8 14:31 myflag
lrwxrwxrwx 1 hacker hacker    5 Oct  6 15:44 not-the-flag -> /flag
-rw-r--r-- 1 root   hacker    0 Oct  8 19:37 open
drwxr-xr-x 2 hacker hacker 4096 Oct  6 07:10 sam
-rw-r--r-- 1 hacker hacker  435 Oct  8 14:14 the-flag
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{EJcigy0_zKPofVH2Nqx0hxkFbnC.dFTM2QDL5MTM1czW}
```