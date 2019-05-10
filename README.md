# CmdsToRemember
Commands which are usually helpful. Sort of a cheat sheet for everything life working with *nix systems. :)

## Linux general bash commands:
Check kernel version:
```
uname -r
```

Check release information:
```
cat /etc/*release
```

Grep for text on each line of file1 in file2.
```
#!/bin/bash
INPUT=$1
INPUT2=$2
for i in $(< $INPUT)
do
echo "grep $i $INPUT2 >> badSyscall.list"
grep "$i" "$INPUT2" >> badSyscall.list
done
```
Great and simple tool to track all fork/execs:
```
sudo apt-get install forkstat
forkstat -e exec
```
Reference: https://stackoverflow.com/questions/26852228/detect-new-process-creation-instantly-in-linux
