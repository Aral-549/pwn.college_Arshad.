
# Intro to Commands 

**Problem** : The problem is to redirect '*my flag*' with help of /challenge/run and the errors that came after to *instructions*  to the file '*COLLEGE*'
## My solve

**Flag:** `pwn.college{MFf001kfI6mnyPCIMAdWIxTvzNJ.QX0YTN0wSN5gjNzEzW}`

**Thought process** :   Followed the instructions after testing once to get the flag.

Inputed the command
bash
```bash
 /challenge/run > ~/myflag 2> ~/instructions

 cat myflag 

```


## What I learned
> * with the help of *>* we can redirect files but only the source file will be present at the destinated file
> *  1> - Redirects stdout (default)
> *  2> - Redirects stderr

## References 
Just Read The Instructions and the Resources
