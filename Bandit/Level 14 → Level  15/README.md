# Level 14 → Level 15

## Level Goal

The password for the next level can be retrieved by submitting the password of the current level to port 30000 on localhost.

## Commands you may need to solve this level

ssh, telnet, nc, openssl, s_client, nmap

## Helpful Reading Material

[How the Internet works in 5 minutes (YouTube)](https://www.youtube.com/watch?v=7_LPdttKXPc) (Not completely accurate, but good enough for beginners)
[IP Addresses](http://computer.howstuffworks.com/web-server5.htm)
[IP Address on Wikipedia](http://en.wikipedia.org/wiki/IP_address)
[Localhost on Wikipedia](http://en.wikipedia.org/wiki/Localhost)
[Ports](http://computer.howstuffworks.com/web-server8.htm)
[Port (computer networking) on Wikipedia](http://en.wikipedia.org/wiki/Port_(computer_networking))

## Write-up

```
ssh bandit14@bandit.labs.overthewire.org
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
nc localhost 30000
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
```
Password : `BfMYroe26WYalil77FoDi9qh59eK5xNr`