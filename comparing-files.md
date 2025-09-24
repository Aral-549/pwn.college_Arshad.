


# Intro to Commands 

**Problem** : The problem is to invoke  the command 'diff' to find the  'flag'(pwn.college) in two different  said files  

## My solve

**Flag:** 'pwn.college{Q-VfxDp7mmgrJr9YIIKig_gEdA7.01MwMDOxwSN5gjNzEzW}'
**Thought process** :   Followed the instructions  to get the flag.

Inputed the command


bash
```bash
 cd /challenge

 
 diff decoys_only.txt decoys_and_real.txt
```


## What I learned
> * learned what the command 'diff' does and how it can be used.
> 
>
> * format : diff file1 file1.
> 
> 
>* diff command tells the differences b/w two files entered.
> 
>
> * 2c2 means change line 2 of file1 to be line 2 of file2 and 1a2 means "after line 1 of file1, add line 2 of file2".
>
> 
> * 3,5d means delete line 3 to 5 or  3d — delete line(s) 3 from file1 (no right-hand side because you remove them).

## References
Just Used The Insructions.
