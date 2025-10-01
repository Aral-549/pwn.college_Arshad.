



# An epic file system quest

**Problem** : The problem is to find the Flag Hidden in hints and directories

## My solve

**Flag:** ' pwn.college{Y6cs1C8AR3qv-mQP0v9tvHBPL7Y.QX5IDO0wSN5gjNzEzW}'
**Thought process** :   Followed the instructions  to get the flag by using and lot of use of cd, cat, ls -a, ls commands

<details> <summary> Step 1 </summary>

```bash


hacker@commands:/$ ls
TEASER  challenge  flag  lib32  media  opt  run  sys  var
bin     dev        home  lib64  mnt    proc sbin  tmp
boot    etc        lib   libx32 nix    root srv  usr

hacker@commands:/$ cat TEASER
Congratulations, you found the clue!
The next clue is in: /usr/lib/python3/dist-packages/_pytest/_io

The next clue is **hidden** --- its filename starts with a '.' character.
You'll need to look for it using special options to 'ls'.
````

</details>

<details> <summary>Step 2</summary>

```bash
hacker@commands:/$ cd /usr/lib/python3/dist-packages/_pytest/_io
hacker@commands:/usr/lib/python3/dist-packages/_pytest/_io$ ls -a
.  ..  .HINT  __init__.py  __pycache__  saferepr.py

hacker@commands:/usr/lib/python3/dist-packages/_pytest/_io$ cat .HINT
Tubular find!
The next clue is in: /opt/linux/linux-5.4/tools/arch/s390/include/uapi/asm
```

</details>



<details>
<summary>Step 3</summary>

```bash
hacker@commands:/opt/linux/linux-5.4/tools/arch/s390/include/uapi/asm$ ls
SNIPPET  bpf_perf_event.h  kvm_perf.h  perf_regs.h  sie.h

hacker@commands:/opt/linux/linux-5.4/tools/arch/s390/include/uapi/asm$ cat SNIPPET
Congratulations, you found the clue!
The next clue is in: /usr/lib/debug/.build-id/0a
```

</details>



<details>
<summary>Step 4 </summary>

```bash
hacker@commands:/usr/lib/debug/.build-id/0a$ ls -a
.  ..  0507f...debug  323c2e...debug  378305...debug  
7ac23f8...debug  d36faca...debug  ALERT

hacker@commands:/usr/lib/debug/.build-id/0a$ cat ALERT
Congratulations, you found the clue!
The next clue is in: /usr/share/perl/5.30.0/Term

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory;
otherwise, the clue will self destruct!
```

</details>



<details> <summary>Step 5</summary>

```bash
hacker@commands:/usr/lib/debug/.build-id/0a$ ls -a /usr/share/perl/5.30.0/Term
.  ..  ANSIColor.pm  Cap.pm  Complete.pm  ReadLine.pm  SPOILER-TRAPPED

hacker@commands:/usr/lib/debug/.build-id/0a$ cat /usr/share/perl/5.30.0/Term/SPOILER-TRAPPED
Tubular find!
The next clue is in: /usr/share/doc/gcc-9-aarch64-linux-gnu-base/gomp
```

</details>



<details>
<summary>Step 6 </summary>

```bash
hacker@commands:/usr/share/doc/gcc-9-aarch64-linux-gnu-base/gomp$ ls -a
.  ..  DOSSIER  changelog.gz

hacker@commands:/usr/share/doc/gcc-9-aarch64-linux-gnu-base/gomp$ cat DOSSIER
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/Documentation/driver-api/mei
```

</details>



<details>
<summary>Step 7 </summary>

```bash
hacker@commands:/opt/linux/linux-5.4/Documentation/driver-api/mei$ ls -a
.  ..  .CUE  hdcp.rst  iamt.rst  index.rst  mei-client-bus.rst  mei.rst  nfc.rst

hacker@commands:/opt/linux/linux-5.4/Documentation/driver-api/mei$ cat .CUE
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/drivers/pci/endpoint
```

</details>

<details>
<summary>Step 8 </summary>

```bash
hacker@commands:/opt/linux/linux-5.4/drivers/pci/endpoint$ ls -a
.  ..  INFO  Kconfig  Makefile  functions  
pci-ep-cfs.c  pci-epc-core.c  pci-epc-mem.c  pci-epf-core.c

hacker@commands:/opt/linux/linux-5.4/drivers/pci/endpoint$ cat INFO
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/block
```

</details>


<details> <summary>Step 9</summary>

```bash
hacker@commands:/opt/linux/linux-5.4/block$ ls -a
.  ..  .GIST  (many build artifacts omitted)

hacker@commands:/opt/linux/linux-5.4/block$ cat .GIST
CONGRATULATIONS! Your perseverance has paid off, and you have found the flag!
It is: pwn.college{Y6cs1C8AR3qv-mQP0v9tvHBPL7Y.QX5IDO0wSN5gjNzEzW}
```

</details>




## What I learned
>* Better understood the use of cammands *cat* *ls -a* and *cd*
## References
Just Used The Insructions
