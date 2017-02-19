# Level 12 → Level 13

## Level Goal

The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)

## Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd, mkdir, cp, mv

## Helpful Reading Material

[Hex dump on Wikipedia](http://en.wikipedia.org/wiki/Hex_dump)

## Write-up

```
ssh bandit13@bandit.labs.overthewire.org
5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu
mkdir /tmp/gun_bandit12
cd /tmp/gun_bandit12
cp ~/data.txt ./data
xxd -r data > binary
file binary
mv binary binary.gz
gzip -d binary.gz
file binary
bzip2 -d binary
file binary.out
mv binary.out binary.gz
gzip -d binary.gz
file binary
tar -xvf binary
file data5.bin
tar -xvf data5.bin
file data6.bin
bzip2 -d data6.bin
file data6.bin.out
tar -xvf data6.bin.out
file data8.bin
mv data8.bin data8.gz
gzip -d data8.gz
file data8
cat data8
```
Password : `8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL`
