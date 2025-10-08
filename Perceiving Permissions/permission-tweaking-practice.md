
# Permission-tweaking-practice

**Problem** : The problem is to continuously and  successfully the command *chmod* successfully to get the permissions for the flags 
## My solve

**Flag:** `pwn.college{MYPTE_5OjdyrxtDFa-ffA4xhYlM.QXwEjN0wSN5gjNzEzW}`

**Thought process** :  Sucessfully completed the command *chmod* in given forat to get the flag rights


 <details> <summary>Inputed the commands</summary>
    
```bash  

chmod g+w /challenge/pwn

chmod uo-rw /challenge/pwn

chmod uo+rx /challenge/pwn

chmod go-wx /challenge/pwn

chmod go+wx /challenge/pwn

chmod go-rx /challenge/pwn

chmod go+r /challenge/pwn

chmod o+x /challenge/pwn

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
## References 
Just the Instructins and Resources
