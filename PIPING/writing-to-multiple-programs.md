

# Intro to Commands 

**Problem** : The problem is to redirect *challenge/hack* output to  /challenge/planet and /challenge/the Simultaneously
## My solve

**Flag:** `pwn.college{QuKI8ZmGVfbZF74T5Tna40kUrHB.QXwgDN1wSN5gjNzEzW}`

**Thought process** :   Followed the instructions after testing once to get the flag.


the output of the /challenge/run command is directly sent to grep therby creating no temp files


Inputed the command
bash
```bash
/challenge/hack | tee >( /challenge/the ) | /challenge/planet

```


## What I learned
> * learned how to beeter use multiple commands in constructive way


## References 
Just Read The Instructions and the Resources
