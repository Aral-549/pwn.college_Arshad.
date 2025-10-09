
# Scripting-with-default-conditionals

**Problem** : The problem is to run /challenge/run after running a script which tests if first argument is *pwn* or not 
## My solve

**Flag:** `pwn.college{sUlo99kJU6Qb01k2pVmc-mduu_Z.01NzMDOxwSN5gjNzEzW}`

**Thought process** :  Sucessfully created *solve.sh* file using the shebangs * #!/bin/bash* wrote a bash program to check if the first argument is *pwn* or not if not it will return *nope* instead of nothing
<details> <summary><strong>Code</strong></summary>

```bash
hacker@chaining~scripting-with-default-cases:~$ vim solve.sh
hacker@chaining~scripting-with-default-cases:~$ bash ~/solve.sh pwn
college
hacker@chaining~scripting-with-default-cases:~$ bash ~/solve.sh pwo
nope
hacker@chaining~scripting-with-default-cases:~$ /challenge/run
Correct! Your script properly handles the if/else conditions.
Here's your flag:
pwn.college{sUlo99kJU6Qb01k2pVmc-mduu_Z.01NzMDOxwSN5gjNzEzW} 

 ```
</details>

## What I learned
> * learned how to use if ,then ,else and fi in bash to write Scripts.
> * FILE1 -ef FILE2  True if file1 is a hard link to file2
## References 
Just the Instructins and Resources






