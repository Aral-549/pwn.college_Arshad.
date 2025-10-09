
# Understanding-shebangs

**Problem** : The problem is to run /challenge/run in after running a solve.sh script with a shebang 
## My solve

**Flag:** `pwn.college{o9aJrnDkvk3qodYzCz3eChepdAL.0VOzMDOxwSN5gjNzEzW}`

**Thought process** :  Sucessfully created *solve.sh* file using the shebangs * #!/bin/bash* ran echo command to output *hack the planet*
got the flag after running /challenge/run command
  
```bash  
vim solve.sh

chmod u+x solve.sh

/challenge/run
```


## What I learned
> * shebangs are used to tell the kernel what is the  type of file
> * #!/bin/bash --> for bash files
> *  #!/bin/python3 --> for python files
> *  #!/bin/sh --> for shell scripts
## References 
Just the Instructins and Resources
