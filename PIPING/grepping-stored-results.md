

# Intro to Commands 

**Problem** : The problem is to redirect the  output of /challenge/run to /tmp/data.txt.
## My solve

**Flag:** `pwn.college{MLI6uHMRVa7zvL9s4h0oZ3GN-TD.QX4EDO0wSN5gjNzEzW}`

**Thought process** :   Followed the instructions after testing once to get the flag.

Inputed the command
bash
```bash
/challenge/run < /tmp/data.txt


grep pwn.college /tmp/data.txt
```


## What I learned
> * with the help of *>* we can redirect files but only the source file will be present at the destinated file
> *  1> - Redirects stdout (default)
> *  2> - Redirects stderr
> * format for grep : *grep Filename /path/to/file*

## References 
Just Read The Instructions and the Resources
