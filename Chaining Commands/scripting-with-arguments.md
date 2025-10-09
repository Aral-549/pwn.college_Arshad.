
# Scripting-with-arguments

**Problem** : The problem is to run /challenge/run /after writhinf a *sript.sh* file such that it outputa the arguments in a reverse order
## My solve

**Flag:** `pwn.college{o1hA5et7uPrRlnai_9S4TUyy8MI.0VNzMDOxwSN5gjNzEzW}`

**Thought process** :  create a script.sh file so that it reverses the two inputed arrguments 
  
```bash  
vim solve.sh 

bash ~/solve.sh killer hero # Output : hero killer

/challenge/run
```


## What I learned
> * shebangs are used to tell the kernel what is the  type of file
> *  #!/bin/bash --> for bash files
> *  #!/bin/python3 --> for python files
> *  #!/bin/sh --> for shell scripts
> *  learned how to add commands while scripting $1 --> 1st argument $2--> 2nd argument 
## References 
Just the Instructins and Resources
