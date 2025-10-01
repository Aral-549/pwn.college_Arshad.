
# Killing-Misbehaving-Processes 

**Problem** : The problem is to find and kill a decoy file and run the command /challenge/run

## My solve

**Flag:** `pwn.college{QrnBmK9nCAcu4JA_RTW5FQARuUo.QX4MDO0wSN5gjNzEzW}`

**Thought process** :   Followed the instructions after testing once to get the flag.


Inputed the commands 
bash
```bash
ps auxww

kill 142

/challenge/run

cat /tmp/flag_fifo #In another Terminal

```


## What I learned
> * compiled the concepts of *kill* *ps auww* and *FIFO* to find the flag
## References 
Just Read the Instructins and Resources
