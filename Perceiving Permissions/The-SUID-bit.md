# The SUID Bit

**Problem** : The Problem is to use the SUID rights to make the flag readable by user

**Flag:** `pwn.college{kCHq-3r7wlhj1JMw4V9MEaPhQF3.QXzEjN0wSN5gjNzEzW}`

**Thought process** :  Sucessfully completed the command *chmod* in given forat to get the flag rights


 Inputed the commands
    
```bash  
chmod u+xs /challenge/getroot

/challenge/getroot #Changes to Root DIrectory

cat /flag
```

## What I learned
> * Command : *chmod* --> *format*- *chmod [OPTIONS] MODE FILE*.
>   
> * u->User ,r->read, g->group , w->write, x-> execute.
>   
> * *drwxr-xr-x* first character is file type next three are root permissiosns next 3 group permissions and next three are others permissions.
>
> * the SUID gives the same power as root solely for that file
>
> * format: *chmod u+srx [PROGRAM]*
## References 
Just the Instructins and Resources
