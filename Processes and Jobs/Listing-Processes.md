
# Listing-Processes 

**Problem** : The problem is to invoke  command  the absolute path "/challenge/run" in a specific directory

## My solve

**Flag:** `pwn.college{QrnBmK9nCAcu4JA_RTW5FQARuUo.QX4MDO0wSN5gjNzEzW}`

**Thought process** :   Followed the instructions after testing once to get the flag.

Inputed the command
bash
```bash
ps aux

/challenge/18614-run-13437

```


## What I learned
> * learned the commands *ps aux* and *ps -ef*
> * *ps aux* gives out processes that are running and aren't in a user readable format
> * *ps -ef* is similar to *pa aux* to disable the truncatation in the terminal use *ps auxww* and *ps -efww*

## References 
[PWN college Youtube Video](https://youtu.be/b67Jq6IZ3U8?list=PL-ymxv0nOtqqRAz1x90vxNbhmSkeYxHVC)
