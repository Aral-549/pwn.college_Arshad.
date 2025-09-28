# Intro to Commands 

**Problem** : The problem is to find flag with help of *grep* and pipe operator(*|*)
## My solve

**Flag:** `pwn.college{ESI5EmvhJxm5r__yGQj9qBXSKWe.0FOxEzNxwSN5gjNzEzW}`

**Thought process** :   Followed the instructions after testing once to get the flag.


the output of the /challenge/run command is directly sent to grep therby creating no temp files


Inputed the command
bash
```bash
/challenge/run | grep -v DECOY
```


## What I learned
> * with adding the argument *-v* to the grep command we can find the lines which do not hace a specific words
> * Format : grep -v SPECIFIC_WORDS 


## References 
Just Read The Instructions and the Resources
