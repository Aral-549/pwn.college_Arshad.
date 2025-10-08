
# Executable-files

**Problem** : The problem is to matke /challenge/run progeam executable by user 
## My solve

**Flag:** `pwn.college{weKDchxjjkqs2F3hvak1yzsqWuw.QXyEjN0wSN5gjNzEzW}`

**Thought process** :   Followed the instructions  get the flag.
used chmod to make the /challenge/run program  executable by user

Inputed the command
bash
```bash
chmod ugo+rx /challenge/run

/challenge/run
```


## What I learned
> * Command : chmod --> format- chmod [OPTIONS] MODE FILE.

> * u->User ,r->read, g->group , w->write, x-> execute.

> * drwxr-xr-x first character is file type next three are root permissiosns next 3 group permissions and next three are others permissions.
## References 
Just Read the Instructins and Resources
