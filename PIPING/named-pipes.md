

# Intro to Commands 

**Problem** : The problem is to make a FIFO file and use it to read the flag
## My solve

**Flag:** `pwn.college{YOtz8glZ6P20ewzS4iTHOKd90tL.01MzMDOxwSN5gjNzEzW}`

**Thought process** :   Followed the instructions after testing once to get the flag.

redirected thee output of /challenge/run to /tmp/flag_fifo while doing so catted the output in another terminal thereby using no storage(IN aand Out)

Inputed the command
bash
```bash
 /challenge/run > /tmp/flag_fifo

cat /tmp/flag_fifo
```


## What I learned
> * with the help of FIFO(First In and First Out) files can be made which (EPHEMERALFLOW) won't take any space
> * the data is blocked until other side is ready
> * Its a first in and out type u cant change once written
## References 
Just Read The Instructions and the Resources
