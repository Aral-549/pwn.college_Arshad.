
# Adding-commands
**Problem** : The problem is to find the path of create a *win* file that *reads* and echoes the flag when /challenge/run is called
## My solve

**Flag:** `pwn.college{4xN24O_ynNxYi1cfjNy6B85fbcK.QX2cjM1wSN5gjNzEzW}`

**Thought process** :  Made a win script using *vim* to read and echo the flag , made the win script executable using *chmod* changed the path so that command */challenge/run* goes to *win* and cat's it
<details><strong> <summary>Click To View Code</summary> 

```bash
hacker@path~adding-commands:~$ cat win
#!/bin/bash
read line < /flag
echo "$line"
hacker@path~adding-commands:~$ chmod +x win
hacker@path~adding-commands:~$ PATH=/home/hacker
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
pwn.college{4xN24O_ynNxYi1cfjNy6B85fbcK.QX2cjM1wSN5gjNzEzW}
 ```

</strong></details>
## What I learned
> * commands like echo , read , cd are independdent of path

## References 
Just the Instructions and Resources




