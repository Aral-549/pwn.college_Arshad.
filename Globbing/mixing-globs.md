
# Intro to Commands 

**Problem** : The problem is to invoke  command  the absolute path "/challenge/run" in a specific directory with a specific argument and using [] glob 

## My solve

**Flag:** `pwn.college{8X7FhRoftzrAVKtOSbijYDRqLnK.QX1IDO0wSN5gjNzEzW}`

**Thought process** :   Followed the instructions after testing nth times got the flag.

every file in the directory starts with a specific alphabet with that in mind using *'[]'* as a separator and *'*'*
to replace the long names making it so everything is less than six digits
Inputed the command
bash
```bash
cd /challenge/files


 /challenge/run [cep]*

```
## What I learned
>* better understood how to use the globs in an effective way
> 

## References 
Just read the Instructions
