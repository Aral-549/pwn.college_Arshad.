
# Reading-shell-scripts

**Problem** : The problem is to run /challenge/run after running a script which tests if first argument is *pwn* or not 
## My solve

**Flag:** `pwn.college{suHaV1HJj1F_erP9A3GSqAXr1UD.0lMwgDOxwSN5gjNzEzW}`

**Thought process** :  the bash file using cat found out the password
<details> <summary><strong>Code</strong></summary>

```bash
hacker@chaining~reading-shell-scripts:~$ cat /challenge/run
#!/opt/pwn.college/bash

read GUESS
if [ "$GUESS" == "hack the PLANET" ]
then
        echo "CORRECT! Your flag:"
        cat /flag
else
        echo "Read the /challenge/run file to figure out the correct password!"
fi


/challenge/run # gives the flag

 ```
</details>

## What I learned
> * */challenge/run* is a bash script and executable so we were able to use cat to find the flag
## References 
Just the Instructins and Resources






