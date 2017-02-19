# Level 6 → Level  7

## Level Goal

The password for the next level is stored in the file data.txt next to the word millionth

## Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

## Helpful Reading Material



## Write-up

```
ssh bandit7@bandit.labs.overthewire.org
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
cat ./data.txt |grep millionth
```
Password : `cvX2JJa4CFALtqS87jk27qwqGhBM9plV`