# Level 23 → Level 24

## Level Goal

A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

** NOTE: ** This level requires you to create your own first shell-script. This is a very big step and you should be proud of yourself when you beat this level!

** NOTE 2: ** Keep in mind that your shell script is removed once executed, so you may want to keep a copy around…

## Commands you may need to solve this level

cron, crontab, crontab(5) (use “man 5 crontab” to access this)

## Helpful Reading Material



## Write-up

```
ssh bandit23@bandit.labs.overthewire.org
jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n
cat /etc/cron.d/cronjob_bandit24
cat /usr/bin/cronjob_bandit24.sh
mkdir /tmp/gun_bandit23
cd /tmp/gun_bandit23
vim script.sh
	#!/bin/bash
	cat /etc/bandit_pass/bandit24 > /tmp/gun_bandit23/nextpass
chmod 775 ./script.sh
cp script.sh /var/spool/bandit24/
cat nextpass 
```
Password : `UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ`