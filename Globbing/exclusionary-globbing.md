




# Intro to Commands 

**Problem** : The problem is to invoke  the command '/challenge/run' in /challenge/files directory with *'*[!]'* argument to find the flag

## My solve

**Flag:** 'pwn.college{omDuHvaqo0G4-XGxuUSVRazbdFh.QX2IDO0wSN5gjNzEzW}'


**Thought process** :   Followed the instructions  to get the flag.
since i need to find files which are not starting with p,w,n  
Inputed the command


bash
```bash
cd /challenge/files


/challenge/run [!pwn]*
```


## What I learned
>* learned  that using glob i can find specific type of files easily
>
>
>* Format : ls/cd/rm/mv  [!xyz]     (*files which are not starting with x or y or z*)
>
>

> 
>  

## References
Just Used The Insruction and Bash Manual
