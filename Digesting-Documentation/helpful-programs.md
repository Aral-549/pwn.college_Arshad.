



# Intro to Commands 

**Problem** : The problem is to invoke  the command '/challenge/challenge' and a suitable argument  to find the flag

## My solve

**Flag:** 'pwn.college{sjQ5eYhbi2b9B86gjSye0LkWKs1.QX3IDO0wSN5gjNzEzW}'


**Thought process** :   Followed the instructions  to get the flag.

used --help/-h command to find the commands to invoke the flag
after a few trial and error using the commands , found the flag


bash
```bash
/challenge/challeneg --help


/challenge/challenge --g  #to get the commands


/challenge/challenge --p  #to get the secret value

/challenge/challenge --p 529

```


## What I learned
>* learned that --help command can be used to run commands which don't have man pages
>  
> 
>* Format : *commnand --help*  or *command -h* 
> 
> 
>  

## References
Just Used The Insructions
