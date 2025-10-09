
# Finding-sessions
**Problem** : The problem is to run screen command to check multiple screens in which flags are found
## My solve

**Flag:** `pwn.college{QsUILMqlvzRYcDF9pcjk1LG8EEm.01N4IDOxwSN5gjNzEzW}`

**Thought process** :  Sucessfully ran screen command which lead to another window and detached from it with *ctrl + A and the d*
found the flag in similar window


```bash
screen -r 145 # ctrl + A and the d

 ```


## What I learned
> * screen can be resumed using the command *screen -r PID/FILE* 
## References 
Just the Instructions and Resources





