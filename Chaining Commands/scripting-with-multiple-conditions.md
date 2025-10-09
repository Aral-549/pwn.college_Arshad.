
# Scripting-with-multiple-conditions

**Problem** : The problem is to run /challenge/run after running a script which tests if first argument is *pwn* or not 
## My solve

**Flag:** `pwn.college{YsAGCTaCwOI03izoJV-1brywkaV.0FOzMDOxwSN5gjNzEzW}`

**Thought process** :  Sucessfully created *solve.sh* file using the shebangs * #!/bin/bash* wrot a bash program to check if the first argument is *pwn* or not
similarly If the argument is "hack", output "the planet" if the argument is "learn", output "linux"for any other input, output "unknown"


<details> <summary><strong>Code</strong></summary>

```bash
hacker@chaining~scripting-with-multiple-conditions:~$ vim solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ cat solve.sh
#!/bin/bash
if [ "$1" == "hack" ]
then
        echo "the planet"
elif [ "$1" == "pwn" ]
then
        echo "college"
elif [ $1 == "learn" ]
then
        echo "linux"
else
        echo "unknown"
fi
hacker@chaining~scripting-with-multiple-conditions:~$ /challenge/run
Correct! Your script properly handles all the conditions with elif.
Here's your flag:
pwn.college{YsAGCTaCwOI03izoJV-1brywkaV.0FOzMDOxwSN5gjNzEzW}

 ```
</details>

## What I learned
> * learned how to use if ,then,else ,elif and fi in bash to write Scripts.
> * FILE1 -ef FILE2  True if file1 is a hard link to file2
## References 
Just the Instructins and Resources






