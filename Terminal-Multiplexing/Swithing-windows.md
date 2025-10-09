
# Detaching-and-attaching
**Problem** : The problem is to run screen command ,detach from it and run /challenge/run
## My solve

**Flag:** `pwn.college{svyj-J_bGURF0HDD08GUNXHAFxI.0FO4IDOxwSN5gjNzEzW}`

**Thought process** :  Sucessfully ran scrren command which lead to another window and used ctrl + A  and press 0 to change to window 0 from window 1


```bash
screen -ls

screen -r 135 # ctrl + A , 0
 ```


## What I learned
> * Ctrl-A c - a new window 
> * Ctrl-A n - moves to next window
> * Ctrl-A p - moves to previous window
> * Ctrl-A 0 through Ctrl-A 9 - moves to window 0-9
> * Ctrl-A " -  moves to selection menu of all of windows
## References 
Just the Instructins and Resources






