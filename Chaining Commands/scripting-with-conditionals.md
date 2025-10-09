
# Scripting-with-conditionals

**Problem** : The problem is to run /challenge/run after running a script which tests if first argument is *pwn* or not 
## My solve

**Flag:** ` pwn.college{sXtPtF86WSHFemZZ3vd4fBsIjo-.0lNzMDOxwSN5gjNzEzW} `

**Thought process** :  Sucessfully created *solve.sh* file using the shebangs * #!/bin/bash* wrote a bash program to check if the first argument is *pwn* or not
<details> <summary><strong>Code</strong></summary>

```bash
hacker@chaining:~$ cat solve.sh
#!/bin/bash

if [ "$1" == "pwn" ]
then
    echo "college"
fi
hacker@chaining:~$ bash ~/solve.sh pwn
college
hacker@chaining:~$ /challenge/run
Correct! Your script properly handles all the conditions.
Here's your flag: pwn.college{sXtPtF86WSHFemZZ3vd4fBsIjo-.0lNzMDOxwSN5gjNzEzW} 

 ```
</details>

## What I learned
> * learned how to use if ,then and fi in bash to write Scripts.
> * FILE1 -ef FILE2  True if file1 is a hard link to file2
## References 
Just the Instructins and Resources







