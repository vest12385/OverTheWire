# Level 15 → Level 16

## Level Goal

The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL encryption.

** Helpful note: Getting “HEARTBEATING” and “Read R BLOCK”? Use -ign_eof and read the “CONNECTED COMMANDS” section in the manpage. Next to ‘R’ and ‘Q’, the ‘B’ command also works in this version of that command… **

## Commands you may need to solve this level

ssh, telnet, nc, openssl, s_client, nmap

## Helpful Reading Material

[Secure Socket Layer/Transport Layer Security on Wikipedia](http://en.wikipedia.org/wiki/Secure_Socket_Layer)
[OpenSSL Cookbook - Testing with OpenSSL](https://www.feistyduck.com/library/openssl-cookbook/online/ch-testing-with-openssl.html)

## Write-up

```
ssh bandit15@bandit.labs.overthewire.org
BfMYroe26WYalil77FoDi9qh59eK5xNr
openssl s_client -connect localhost:30001 -ign_eof
BfMYroe26WYalil77FoDi9qh59eK5xNr
```
Password : `cluFn7wTiGryunymYOu4RcffSxQluehd`