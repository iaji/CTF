# **Bandit**

## Level 0
```
ssh bandit0@bandit.labs.overthewire.org

pass: bandit0

ls

cat readme

boJ9jbbUNNfktd78OOpsqOltutMc3MY1

logout
```
## Level 1

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

pass: HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

bandit7@melinda:~$ cat data.txt | grep "millionth"
millionth	cvX2JJa4CFALtqS87jk27qwqGhBM9plV

logout
```
## Level 8

```
ssh bandit8@bandit.labs.overthewire.org

pass: cvX2JJa4CFALtqS87jk27qwqGhBM9plV

cat data.txt | sort | uniq -u

UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

logout
```

## Level 9

```
ssh bandit9@bandit.labs.overthewire.org

pass: UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

cat data.txt | strings | grep ".*==="

I========== the6
========== password
========== ism
========== truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk

logout
```

## Level 10

```
ssh bandit10@bandit.labs.overthewire.org

pass: truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk

base64 -d data.txt

The password is IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR

logout
```

## Level 11

```
ssh bandit11@bandit.labs.overthewire.org

pass: IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR

cat data.txt | tr [A-Za-z] [N-ZA-Mn-za-m]

The password is 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu

logout
```

## Level 12

```
ssh bandit12@bandit.labs.overthewire.org

pass: 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu

mkdir /tmp/jack19

cp data.txt step1.txt

mv step1.txt /tmp/jack19

cd /tmp/jack19

xxd -r step1.txt step1.bin

file step1.bin
step1.bin: gzip compressed data, was "data2.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression

mv step1.bin step1.gz

gzip -d step1.gz

file step1

mv step1 step2.bz2

bzip2 -d step2.bz2

file step2

mv step2 step3.gz

gzip -d step3.gz

file step3

mv step3 step4.tar

tar -xf step4.tar

file data5.bin

mv data5.bin step5.tar

tar -xf step5.tar

file data6.bin

mv data6.bin step7.bz2

bzip2 -d step7.bz2

file step7

mv step7 step8.tar

tar -xf step8.tar

file data8.bin

mv data8.bin step9.gz

gzip -d step9.gz

file step9

cat step9

The password is 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

logout
```

## Level 13

```
ssh bandit13@bandit.labs.overthewire.org

pass: 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

ls

ssh -i sshkey.private bandit14@localhost

```

## Level 14

```
cd /etc/bandit_pass/

pass: 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e

nc -v localhost 30000
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
Correct!

BfMYroe26WYalil77FoDi9qh59eK5xNr
```

## Level 15

```
ssh bandit15@bandit.labs.overthewire.org

pass: BfMYroe26WYalil77FoDi9qh59eK5xNr

```
