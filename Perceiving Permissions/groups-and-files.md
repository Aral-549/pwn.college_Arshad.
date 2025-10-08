
# Groups-and-files

**Problem** : The problem is to add the flag into the hacker group with *chgrp*
## My solve

**Flag:** `pwn.college{AQpvtWazw0OCNQ85oj4G6kKmXvz.QXxcjM1wSN5gjNzEzW}`

**Thought process** :   cd'ed to the */* Directory and changed the group of flag into hacker so that it can be read

Inputed the command
bash
```bash
cd /

chgrp hacker flag

cat flag

```


## What I learned
> * Command : *chgrp* --> *format*- *chgrp group path/to/file* 
## References 
Just Read the Instructins and Resources
