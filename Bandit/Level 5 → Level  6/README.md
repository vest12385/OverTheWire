# Level 5 → Level  6

## Level Goal

The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties: - human-readable - 1033 bytes in size - not executable

## Commands you may need to solve this level

ls, cd, cat, file, du, find

## Helpful Reading Material



## Write-up

```
ssh bandit5@bandit.labs.overthewire.org
koReBOKuIDDepwhWk7jZC0RTdopnAYKh
cd inhere/
find -size 1033c -readable ! -executable
cat ./maybehere07/.file2
```
Password : `DXjZPULLxYr17uwoI01bNLQbtFemEgo7`