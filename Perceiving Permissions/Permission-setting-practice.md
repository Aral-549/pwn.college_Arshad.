
# Permission-setting-practice

**Problem** : The problem is to continuously and  successfully the command *chmod* successfully to get the permissions for the flags 
## My solve

**Flag:** `pwn.college{4GOe_zmPYs7GxJhwgpPagznZl1W.QXzETO0wSN5gjNzEzW}`

**Thought process** :  Sucessfully completed the command *chmod* in given forat to get the flag rights


 <details> <summary>Inputed the commands</summary>
    
```bash  

chmod u=-,g=rx,o=-  /challenge/pwn

chmod u=rw,g=wx,o=rw  /challenge/pwn

chmod u=r,g=wr,o=r  /challenge/pwn

chmod u=-,g=w,o=wxr  /challenge/pwn

chmod u=r,g=rx,o=wr  /challenge/pwn

chmod u=rwx,g=x,o=r  /challenge/pwn

chmod u=rwx,g=r,o=wx  /challenge/pwn

chmod u=w,g=rwx,o=rwx  /challenge/pwn

chmod u+r /flag

cat /flag

```
 </details>

## What I learned
> * Command : *chmod* --> *format*- *chmod [OPTIONS] MODE FILE*.
>   
> * u->User ,r->read, g->group , w->write, x-> execute.
>   
> * *drwxr-xr-x* first character is file type next three are root permissiosns next 3 group permissions and next three are others permissions.
>
> * Another format: *chmod u=rwx, g=r, o=- FILE* 
## References 
Just the Instructins and Resources
