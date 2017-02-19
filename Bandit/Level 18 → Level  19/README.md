# Level 18 → Level 19

## Level Goal

The password for the next level is stored in a file readme in the homedirectory. Unfortunately, someone has modified .bashrc to log you out when you log in with SSH.

## Commands you may need to solve this level

ssh, ls, cat

## Helpful Reading Material



## Write-up

```
ssh bandit18@bandit.labs.overthewire.org
kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
ssh bandit18@bandit.labs.overthewire.org /bin/sh
kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
cat readme
```
Password : `IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x`