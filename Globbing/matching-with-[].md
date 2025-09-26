




# Intro to Commands 

**Problem** : The problem is to invoke  the command '/challenge/run' with a specific argument using the glob '*[]*'in /challenge/files directory   to find the flag

## My solve

**Flag:** 'pwn.college{Qm20tNa_22cPz2pq9EaAuCQ8tGi.QXzIDO0wSN5gjNzEzW}'


**Thought process** :   Followed the instructions  to get the flag.

Inputed the command


bash
```bash
cd /c*e


 cd f*s

/challenge/run file_[bash]
```


## What I learned
>* learned  that using glob names of files can be reduced
>
>
>* Format : ls/cd/rm/mv  file[abc]      (*filea  fileb  filec*) takes one caharacter at a time 
>
>

> '*' replaces multiple chacracters wheras *'?'* replaces one that number of characters as *'?'* and it has same format as *'*'*
> 
>  

## References
Just Used The Insruction and Bash Manual
