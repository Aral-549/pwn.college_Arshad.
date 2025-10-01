# Data Manipulation

**Problem** : The problem is to find flag by removing a specific column in the /challenge/run output
## My solve

**Flag:** `pwn.college{AAZzfQGCIukDGJAZhdH3PY7mI47.01NxEzNxwSN5gjNzEzW}`

**Thought process** :   Followed the instructions after testing once to get the flag.


Inputed the command
bash
```bash
 /challenge/run | cut -d " " -f 2 | tr -d "\n"
```


## What I learned
> * wth the command *cut*  we can specifically print specific column of a file
> * *-d* is the column delimiter(what separates the fields in each line)
> * *-f* means field specifies which one to be cutdown


## References 
Just Read The Instructions and the Resources
