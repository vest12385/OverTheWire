# Level 11 → Level 12

## Level Goal

The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

## Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

## Helpful Reading Material

[Rot13 on Wikipedia](http://en.wikipedia.org/wiki/Rot13)

## Write-up

```
ssh bandit11@bandit.labs.overthewire.org
IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
cat data.txt | tr 'n-za-mN-ZA-M' 'a-zA-Z'
```
Password : `5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu`