# Intro to Commands 

**Problem** : The problem is to find flag by converting lower cases to uppercases and viceversa
## My solve

**Flag:** `pwn.college{Ewzdj_Rx0qBnzmkFgkVstJ9nyak.01MxEzNxwSN5gjNzEzW}`

**Thought process** :   Followed the instructions after testing once to get the flag.


the output of the /challenge/run command is directly sent to grep therby creating no temp files


Inputed the command
bash
```bash
/challenge/run | tr 'ABCDEFGHIJKLMNOPQ
RSTUVWXYZ abcdefghijklmnopqrstuvwxyz' 'abcdefghijklmnopqrstuvwxyz ABCDEFGHIJ
KLMNOPQRSTUVWXYZ'

/challenge/run | tr '[:lower:][:upper:]' '[:upper:][:lower:]'


```


## What I learned
> * wth the command *tr* we can change the casing of specific characters or the whole alpabets if wanted 


## References 
Just Read The Instructions and the Resources
