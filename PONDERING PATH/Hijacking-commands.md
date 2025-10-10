
# Reading-shell-scripts
**Problem** : The problem is to make sure /challenge/run does not run the remove flag command and also to make sure to print the flag
## My solve

**Flag:** `pwn.college{URjNTqXB1mQe0iurF87c4wDtWkP.QX3cjM1wSN5gjNzEzW}`

**Thought process** : created a sym link to the bash so that instead of it executes *bash /flag* instead *rm /flag* Added /home/hacker/ as path and ran /challenge/run


```bash
ln -s /usr/bin/bash ./rm

PATH=/home/hacker/:$PATH

/challenge/run
 ```


## What I learned
> * Better understood the concepts of the Path , symlinks. 
## References 
Just the Instructions and Resources




