

# Intro to Commands 

**Problem** : The problem is to find flag with help of *grep* and pipe operator(*|*) by redirecting stderr to another process
## My solve

**Flag:** `pwn.college{oMdtyF1I0tyizR8wzFIH7PZ21vQ.QX1ATO0wSN5gjNzEzW}`

**Thought process** :   Followed the instructions after testing once to get the flag.


the output(stderr) of the /challenge/run command is  sent to stdout followed by grep therby creating no temp files


Inputed the command
bash
```bash
 /challenge/run 2>& 1 |grep pwn.college
```


## What I learned
> * with the help of *|* operator we can stack and use multiple commands
> * with the help of >& operator we can redirect b/w processes
> * 2>& redirects stderr(file descriptor) to another process. 



## References 
Just Read The Instructions and the Resources
