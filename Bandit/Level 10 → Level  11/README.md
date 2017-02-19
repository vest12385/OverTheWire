# Level 10 → Level 11

## Level Goal

The password for the next level is stored in the file data.txt, which contains base64 encoded data

## Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

## Helpful Reading Material

[Base64 on Wikipedia](http://en.wikipedia.org/wiki/Base64s)

## Write-up

```
ssh bandit10@bandit.labs.overthewire.org
truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
base64 -d data.txt 
```
Password : `IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR`