

# Intro to Commands 

**Problem** : The problem is to pipe a secret value from /challenge/pwn to /challenge/college
## My solve

**Flag:** `pwn.college{02d7W5MM6is5ayVuMRAzclqMOyW.QXxITO0wSN5gjNzEzW}`

**Thought process** :   Followed the instructions after testing once to get the flag.

i used the *tee* command to find out the secret value and directed it from /challenge/pwn to /challenge/college
with the help of pipe

Inputed the command
bash
```bash
 /challenge/pwn | tee xyz | /challenge/college

/challenge/pwn --secret 02d7W5MM|tee uvw | /challenge/college

```


## What I learned
> * with the help of *tee* command (Tee splitter) we can make  copies of the output form stdout also pipe them out if necessary


## References 
Just Read The Instructions and the Resources
