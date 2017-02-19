# Level 17 → Level 18

## Level Goal

There are 2 files in the homedirectory: passwords.old and passwords.new. The password for the next level is in passwords.new and is the only line that has been changed between passwords.old and passwords.new

NOTE: if you have solved this level and see ‘Byebye!’ when trying to log into bandit18, this is related to the next level, bandit19

## Commands you may need to solve this level

cat, grep, ls, diff

## Helpful Reading Material



## Write-up

```
ssh bandit17@bandit.labs.overthewire.org
xLYVMN9WE5zQ5vHacb0sZEVqbrp7nBTn
diff passwords.new passwords.old
```
Password : `kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd`