

# Intro to Commands 

**Problem** : The problem is to redirect(input) the word  '*COLLEGE*' to the file '*PWN*' and then redirect the PWN file into my standard input
## My solve

**Flag:** `pwn.college{4N5HqIFI_j6ea1r0zwM5cdb4RYa.QXwcTN0wSN5gjNzEzW}`

**Thought process** :   Followed the instructions after testing once to get the flag.

Inputed the command
bash
```bash
echo COLLEGE > PWN


/challenge/run < PWN
```


## What I learned
> * with the help of *<* we can redirect(Input) files from a particular file
>   
> *  1> - Redirects stdin (default)
> 

## References 
Just Read The Instructions and the Resources
