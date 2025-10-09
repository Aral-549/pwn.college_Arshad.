
# Setting-PATH
**Problem** : The problem is to run /challenge/run such that it won't destroy the flag but runs the win command.
## My solve

**Flag:** `pwn.college{kBYkJXkyz8g6ocCSKj3BOgCUjE3.QX1cjM1wSN5gjNzEzW}`

**Thought process** :  overwrote the usual path by /challenge/more_commands/ so that */challenge/run* runs win command 


```bash
PATH=/challenge/more_commands/

/challenge/run
 ```


## What I learned
> * *PATH=''* will make it so that the program won't look anyhere for the commands
## References 
Just the Instructions and Resources





