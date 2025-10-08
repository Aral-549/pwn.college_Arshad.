
# Changing-permissions

**Problem** : The problem is to change the permissind of the flag file using *chmod*
## My solve

**Flag:** `pwn.college{4Qw2tXOaegeGYkF7rls9Z-Zr-o2.QXzcjM1wSN5gjNzEzW}`

**Thought process** :   cd'ed to the */* Directory and changed the the permissions of group nad others on flag to read 

Inputed the command
bash
```bash
cd /

chmod go+r flag

cat flag

```


## What I learned
> * Command : *chmod* --> *format*- *chmod [OPTIONS] MODE FILE*.
>   
> * u->User ,r->read, g->group , w->write, x-> execute.
>   
> * *drwxr-xr-x* first character is file type next three are root permissiosns next 3 group permissions and next three are others permissions.
## References 
Just the Instructins and Resources.
