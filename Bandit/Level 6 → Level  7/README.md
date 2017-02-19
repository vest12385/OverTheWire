# Level 6 → Level  7

## Level Goal

The password for the next level is stored somewhere on the server and has all of the following properties: - owned by user bandit7 - owned by group bandit6 - 33 bytes in size

## Commands you may need to solve this level

ls, cd, cat, file, du, find, grep

## Helpful Reading Material



## Write-up

```
ssh bandit6@bandit.labs.overthewire.org
DXjZPULLxYr17uwoI01bNLQbtFemEgo7
cd /
find -group bandit6 -user bandit7 -size 33c
cat ./var/lib/dpkg/info/bandit7.password
```
Password : `HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs`