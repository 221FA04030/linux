The password for the next level is stored somewhere on the server and has all of the following properties:

    owned by user bandit7
    owned by group bandit6
    33 bytes in size



bandit6@bandit:~$ ls
bandit6@bandit:~$ ls -ls
total 0
bandit6@bandit:~$ ls -la
total 20
drwxr-xr-x   2 root root 4096 Sep 26 21:54 .
drwxr-xr-x 150 root root 4096 Sep 26 21:58 ..
-rw-r--r--   1 root root  220 Feb 13  2026 .bash_logout
-rw-r--r--   1 root root 3851 Sep 26 21:38 .bashrc
-rw-r--r--   1 root root  807 Feb 13  2026 .profile
bandit6@bandit:~$ cd .
bandit6@bandit:~$ ls
bandit6@bandit:~$ find / -user bandit7 -group bandit6 -size 33 2 > /dev/null
find: paths must precede expression: `2'
bandit6@bandit:~$ find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
/var/lib/dpkg/info/bandit7.password
bandit6@bandit:~$ cat /var/lib/dpkg/info/bandit7.password
Bmnnvf82KzQlfxgAI2d1zYbr1u9pr3E3
 