# **Bandit**

## **Level 0**
```
ssh bandit0@bandit.labs.overthewire.org

pass: bandit0

ls

cat readme

boJ9jbbUNNfktd78OOpsqOltutMc3MY1

logout
```
## **Level 1**

```
ssh bandit1@bandit.labs.overthewire.org

pass: boJ9jbbUNNfktd78OOpsqOltutMc3MY1

ls

cat ./-

CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

logout
```

## Level 2

```
ssh bandit2@bandit.labs.overthewire.org

pass: CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

ls

cat spaces\ in\ this\ filename

UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

logout
```

## Level 3

```
ssh bandit3@bandit.labs.overthewire.org

pass: UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

ls

cd inhere

ls -la

cat .hidden

pIwrPrtPN36QITSp3EQaw936yaFoFgAB
```

## Level 4

```
ssh bandit3@bandit.labs.overthewire.org

pass: pIwrPrtPN36QITSp3EQaw936yaFoFgAB

bandit4@melinda:~$ ls
inhere
bandit4@melinda:~$ cd inhere/
bandit4@melinda:~/inhere$ ls
-file00  -file02  -file04  -file06  -file08
-file01  -file03  -file05  -file07  -file09
bandit4@melinda:~/inhere$ file ./-file00
./-file00: data
bandit4@melinda:~/inhere$ file ./-file01
./-file01: data
bandit4@melinda:~/inhere$ file ./-file02
./-file02: data
bandit4@melinda:~/inhere$ file ./-file03
./-file03: data
bandit4@melinda:~/inhere$ file ./-file04
./-file04: data
bandit4@melinda:~/inhere$ file ./-file05
./-file05: data
bandit4@melinda:~/inhere$ file ./-file06
./-file06: data
bandit4@melinda:~/inhere$ file ./-file07
./-file07: ASCII text

bandit4@melinda:~/inhere$ cat ./-file07
koReBOKuIDDepwhWk7jZC0RTdopnAYKh

logout
```

## Level 5

```
ssh bandit5@bandit.labs.overthewire.org

pass: koReBOKuIDDepwhWk7jZC0RTdopnAYKh

andit5@melinda:~/inhere$ find ./ -size 1033c
./maybehere07/.file2

bandit5@melinda:~/inhere$ cd maybehere07
bandit5@melinda:~/inhere/maybehere07$ cat .file2
DXjZPULLxYr17uwoI01bNLQbtFemEgo7

logout
```

## Level 6

```
ssh bandit6@bandit.labs.overthewire.org

pass: koReBOKuIDDepwhWk7jZC0RTdopnAYKh

find / -size 33c -user bandit7 -group bandit6 2>/dev/null

/var/lib/dpkg/info/bandit7.password

cat /var/lib/dpkg/info/bandit7.password

HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
```

## Level 7

```
ssh bandit7@bandit.labs.overthewire.org

pass: koReBOKuIDDepwhWk7jZC0RTdopnAYKh
```
