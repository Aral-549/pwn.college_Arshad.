
# Detaching-and-attaching
**Problem** : The problem is to run screen command ,detach from it and run /challenge/run
## My solve

**Flag:** `pwn.college{47BahulKjQRH6tzs-V2Eq-KHuDQ.0lN4IDOxwSN5gjNzEzW}`

**Thought process** :  Sucessfully ran scrren command which lead to another window and detached from it with *ctrl + A and the d*


```bash
screen # ctrl + A and the d

/challenge/run

screen -r
 ```


## What I learned
> * learned how to use screen command to detach press ctrl + A release and press d
> * command format: *screen -S mysession* to start a session
> * command format: *screen -r mysession* to start a session
## References 
Just the Instructins and Resources






