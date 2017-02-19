# Level 25 → Level 26

## Level Goal

Logging in to bandit26 from bandit25 should be fairly easy… The shell for user bandit26 is not /bin/bash, but something else. Find out what it is, how it works and how to break out of it.

## Commands you may need to solve this level

ssh, cat, more, vi, ls, id, pwd

## Helpful Reading Material



## Write-up

```
ssh bandit25@bandit.labs.overthewire.org
uNG9O58gUE7snukf3bvZ0rxhtnjzSGzG
ssh -i bandit26.sshkey bandit26@localhost
cat /etc/passwd | grep bandit26
cat /usr/bin/

縮小視窗
ssh -i bandit26.sshkey bandit26@localhosts
input v then get into vi mode
:e /etc/bandit_pass/bandit26
```
Password : `5czgV9L3Xx8JPOyRbXh6lQbmIOWvPT6Z`