

# Intro to Commands 

**Problem** : The problem is to specify an argument whis is an absolute path to  "challenge/run" , it should be <4 characters and present in home directory
hacker@dojo:~$ /challenge/run YOUR_PATH_HERE
## My solve

**Flag:** `pwn.college{EsWQ064O9Ty6xN6_EKaNh1iWlNZ.QXzMDO0wSN5gjNzEzW}`

**Thought process** :   Followed the instructions after testing few times to get the flag.
since no file in home directory has characters less than 4 . I just used the home directory '~' + '!'or ':' 
thereby creating a file hackers! or hackers: using less than 4 characters  
Inputed the command and argument


bash
```bash
  /challenge/run ~!

```


## What I learned
> learn what '~' is and how can it be used 
>
> 
> learned the use of 'ls' command to check exsisting directories 

## References 
[PWN college Youtube Video](https://youtu.be/b67Jq6IZ3U8?list=PL-ymxv0nOtqqRAz1x90vxNbhmSkeYxHVC)


[Geeks For Geeks](https://www.geeksforgeeks.org/linux-unix/cd-command-in-linux-with-examples/)
