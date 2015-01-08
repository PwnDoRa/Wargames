Bandit Level 7 �� Level 8
========================

### <font color="grey">Level Goal</font>

The password for the next level is stored in the file data.txt next to the word millionth

### <font color="grey">Commands you may need to solve this level</ont>

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

### <font color="grey">Helpful Reading Material</ont>
The unix commandline: pipes and redirects

### <font color="grey">Solution</font>

Account: bandit7
Password: HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
Host: bandit.labs.overthewire.org

�ϥΤW�z�b���K�X�z�L SSH �n�J�ĤC���C

```
$ ssh bandit7@bandit.labs.overthewire.org -p 22
...
bandit7@bandit.labs.overthewire.org's password:
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
...
```

�ˬd�a�ؿ��A�T�{�s�b data.txt �ɮסC

```
bandit7@melinda:~$ ls -al
total 4112
drwxr-xr-x   2 root    root       4096 Jun  6  2013 .
drwxr-xr-x 160 root    root       4096 Jul 28 17:05 ..
-rw-r--r--   1 root    root        220 Apr  3  2012 .bash_logout
-rw-r--r--   1 root    root       3486 Apr  3  2012 .bashrc
-rw-r--r--   1 root    root        675 Apr  3  2012 .profile
-rw-r-----   1 bandit8 bandit7 4184396 Jun  6  2013 data.txt
```

�ڭ̨ϥ� grep ���O�w�� data.txt �ɮסA��X���d�ؼЩҴ��Ѫ��r�� ��millionth�� �A����N�O�U�@�����K�X�C

```
bandit7@melinda:~$ grep millionth data.txt
millionth   cvX2JJa4CFALtqS87jk27qwqGhBM9plV
```

�e�i�U�@���I
