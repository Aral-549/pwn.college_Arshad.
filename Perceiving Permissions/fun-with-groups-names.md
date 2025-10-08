
# Fun-with-Groups-and-files

**Problem** : The problem is to add the flag into the hacker group with *chgrp*
## My solve

**Flag:** `pwn.college{cxS35YC38m59X_8XUrmy3lYyIG2.QXycjM1wSN5gjNzEzW}`

**Thought process** :  changed the group of flag into grp16995 so that it can be read

Inputed the command
bash
```bash
id #uid=1000(hacker) gid=1000(grp16995) groups=1000(grp16995)

chgrp grp16995  /flag 

cat /flag

```


## What I learned
> * Command : *chgrp* --> *format*- *chgrp group path/to/file* 
## References 
Just Read the Instructins and Resources
