Bandit Level 9 → Level 10
Level Goal

The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.
Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

bandit9@bandit:~$ ls
data.txt
bandit9@bandit:~$ grep data.txt | = *
=: command not found
^C
bandit9@bandit:~$ string data.txt |"==="
===: command not found
Command 'string' not found, did you mean:
  command 'spring' from deb ruby-spring (2.1.1-2)
  command 'spring' from deb spring (106.0+dfsg-4)
  command 'strings' from deb binutils (2.46-3ubuntu2)
Try: apt install <deb name>
bandit9@bandit:~$ strings data.txt |"==="
===: command not found
bandit9@bandit:~$ strings data.txt |"=="
==: command not found
bandit9@bandit:~$ strings data.txt | "=="
==: command not found
bandit9@bandit:~$ strings data.txt | grep "=="
\========== the
========== password
<u*========== is
lp>IoY-b==ld
========== B0s2khmbT9u0geKuOoVGW3JZKhndE3BG
bandit9@bandit:~$ 