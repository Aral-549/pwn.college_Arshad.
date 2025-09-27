




# Intro to Commands 

**Problem** : The problem is to invoke  the command '/challenge/catflag' using softlinks to create a shortcut to *flag* the invoke the *flag*

## My solve

**Flag:** 'pwn.college{Q9SCmfYvb-9E2QNiJYhvpmmeVYP.QX5ETN1wSN5gjNzEzW}'


**Thought process** :   Followed the instructions  to get the flag.

since the *not-the-flag* is being invoked insetad of *catflag* i just removed the *not-the-flag* file and created a symlink between 

*not-the-flag* and the actual /flag so that when the command(/challenge/catflag) is invoked the *not-the-flag* will run inturn printing the /flag

Inputed the command


bash
```bash
rm -f /home/hacker/not-the-flag


ln -s /flag /home/hacker/not-the-flag


/challenge/catflag
```


## What I learned
>* learned abt Hard Links: differnt paths/name to the same file. **file command** is *Ln  /file    /hard link to the file*.
>
>

>* learned abt Soft links: A symbolic link/pointer/shortcut to the OG file. **file command** *ln -s /file    /soft link to the file*

>
>

> 
>  

## References
Just Used The Insruction

[Youtube LINK](https://www.youtube.com/watch?list=PL-ymxv0nOtqqRAz1x90vxNbhmSkeYxHVC&v=m55AtwjBXpE)
