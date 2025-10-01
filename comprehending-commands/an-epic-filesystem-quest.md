



# An epic file system quest

**Problem** : The problem is to find the Flag Hidden in hints and directories

## My solve

**Flag:** ' pwn.college{Y6cs1C8AR3qv-mQP0v9tvHBPL7Y.QX5IDO0wSN5gjNzEzW}'
**Thought process** :   Followed the instructions  to get the flag by using and lot of use of cd, cat, ls -a, ls commands



<details>
      <summary>FUll PROCESS</summary>
      hacker@commands~an-epic-filesystem-quest:/$ ls
TEASER  challenge  flag  lib32   media  opt   run   sys  var
bin     dev        home  lib64   mnt    proc  sbin  tmp
boot    etc        lib   libx32  nix    root  srv   usr
hacker@commands~an-epic-filesystem-quest:/$ cat TEASER
Congratulations, you found the clue!
The next clue is in: /usr/lib/python3/dist-packages/_pytest/_io

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/lib/python3/dist-packages/_pytest/_io
cat: /usr/lib/python3/dist-packages/_pytest/_io: Is a directory
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/lib/python3/dist-packages/_pytest/_io
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/_pytest/_io$ ls
__init__.py  __pycache__  saferepr.py
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/_pytest/_io$ ls -a
.  ..  .HINT  __init__.py  __pycache__  saferepr.py
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/_pytest/_io$ cat .HINT
Tubular find!
The next clue is in: /opt/linux/linux-5.4/tools/arch/s390/include/uapi/asm
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/_pytest/_io$ ls /opt/linux/linux-5.4/tools/arch/s390/include/uapi/asm
SNIPPET        bpf_perf_event.h  kvm_perf.h  perf_regs.h  sie.h
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/_pytest/_io$ cd /opt/linux/linux-5.4/tools/arch/s390/include/uapi/asm
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/tools/arch/s390/include/uapi/asm$ cat SNIPPET
Congratulations, you found the clue!
The next clue is in: /usr/lib/debug/.build-id/0a

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/tools/arch/s390/include/uapi/asm$ cd /usr/lib/debug/.build-id/0a
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/0a$ cd ls -a
bash: cd: too many arguments
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/0a$ ls -a
.   0507fccacd23843237ec32a22b5b0e775814f1.debug  378305aa26a8e32cc408b9f39cae5db5f89740.debug  ALERT
..  323c2e74942fefba5c0cb0efe04575a90b5f1b.debug  7ac23f8e0c32eb01912084316784f6a747fb76.debug  d36faca36ebd36ca68a471902dd21e4a6c0c62.debug
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/0a$ cat ALERT
Congratulations, you found the clue!
The next clue is in: /usr/share/perl/5.30.0/Term

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/0a$ cat /usr/share/perl/5.30.0/Term
cat: /usr/share/perl/5.30.0/Term: Is a directory
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/0a$ ls -a /usr/share/perl/5.30.0/Term
.  ..  ANSIColor.pm  Cap.pm  Complete.pm  ReadLine.pm  SPOILER-TRAPPED
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/0a$ cat /usr/share/perl/5.30.0/Term/SPOILER-TRAPPED
Tubular find!
The next clue is in: /usr/share/doc/gcc-9-aarch64-linux-gnu-base/gomp
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/0a$ ls -a /usr/share/doc/gcc-9-aarch64-linux-gnu-base/gomp
.  ..  DOSSIER  changelog.gz
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/0a$ cat /usr/share/doc/gcc-9-aarch64-linux-gnu-base/gomp/DOSSIER
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/Documentation/driver-api/mei

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/0a$ ls -a /opt/linux/linux-5.4/Documentation/driver-api/mei
.  ..  .CUE  hdcp.rst  iamt.rst  index.rst  mei-client-bus.rst  mei.rst  nfc.rst
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/0a$ cd /opt/linux/linux-5.4/Documentation/driver-api/mei/.CUE
bash: cd: /opt/linux/linux-5.4/Documentation/driver-api/mei/.CUE: Not a directory
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/0a$ cat /opt/linux/linux-5.4/Documentation/driver-api/
mei/.CU
cat: /opt/linux/linux-5.4/Documentation/driver-api/mei/.CU: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/0a$ cd /opt/linux/linux-5.4/Documentation/driver-api/mei
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/driver-api/mei$ cat .CUE
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/drivers/pci/endpoint
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/driver-api/mei$ ls -a /opt/linux/linux-5.4/drivers/pci/endpoint
.  ..  INFO  Kconfig  Makefile  functions  pci-ep-cfs.c  pci-epc-core.c  pci-epc-mem.c  pci-epf-core.c
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/driver-api/mei$ cat /opt/linux/linux-5.4/drivers/pci/endpoint/INFO
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/block

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/driver-api/mei$ ls -a /opt/linux/linux-5.4/block
.                      .built-in.a.cmd           blk-integrity.c         blk-mq-virtio.o  bsg.c
..                     .compat_ioctl.o.cmd       blk-ioc.c               blk-mq.c         bsg.o
.GIST                  .elevator.o.cmd           blk-ioc.o               blk-mq.h         built-in.a
.badblocks.o.cmd       .genhd.o.cmd              blk-iocost.c            blk-mq.o         cmdline-parser.c
.bio.o.cmd             .ioctl.o.cmd              blk-iolatency.c         blk-pm.c         compat_ioctl.c
.blk-core.o.cmd        .ioprio.o.cmd             blk-lib.c               blk-pm.h         compat_ioctl.o
.blk-exec.o.cmd        .kyber-iosched.o.cmd      blk-lib.o               blk-pm.o         elevator.c
.blk-flush.o.cmd       .mq-deadline.o.cmd        blk-map.c               blk-rq-qos.c     elevator.o
.blk-ioc.o.cmd         .partition-generic.o.cmd  blk-map.o               blk-rq-qos.h     genhd.c
.blk-lib.o.cmd         .scsi_ioctl.o.cmd         blk-merge.c             blk-rq-qos.o     genhd.o
.blk-map.o.cmd         Kconfig                   blk-merge.o             blk-settings.c   ioctl.c
.blk-merge.o.cmd       Kconfig.iosched           blk-mq-cpumap.c         blk-settings.o   ioctl.o
.blk-mq-cpumap.o.cmd   Makefile                  blk-mq-cpumap.o         blk-softirq.c    ioprio.c
.blk-mq-debugfs.o.cmd  badblocks.c               blk-mq-debugfs-zoned.c  blk-softirq.o    ioprio.o
.blk-mq-pci.o.cmd      badblocks.o               blk-mq-debugfs.c        blk-stat.c       kyber-iosched.c
.blk-mq-sched.o.cmd    bfq-cgroup.c              blk-mq-debugfs.h        blk-stat.h       kyber-iosched.o
.blk-mq-sysfs.o.cmd    bfq-iosched.c             blk-mq-debugfs.o        blk-stat.o       mq-deadline.c
.blk-mq-tag.o.cmd      bfq-iosched.h             blk-mq-pci.c            blk-sysfs.c      mq-deadline.o
.blk-mq-virtio.o.cmd   bfq-wf2q.c                blk-mq-pci.o            blk-sysfs.o      opal_proto.h
.blk-mq.o.cmd          bio-integrity.c           blk-mq-rdma.c           blk-throttle.c   partition-generic.c
.blk-pm.o.cmd          bio.c                     blk-mq-sched.c          blk-timeout.c    partition-generic.o
.blk-rq-qos.o.cmd      bio.o                     blk-mq-sched.h          blk-timeout.o    partitions
.blk-settings.o.cmd    blk-cgroup.c              blk-mq-sched.o          blk-wbt.c        scsi_ioctl.c
.blk-softirq.o.cmd     blk-core.c                blk-mq-sysfs.c          blk-wbt.h        scsi_ioctl.o
.blk-stat.o.cmd        blk-core.o                blk-mq-sysfs.o          blk-zoned.c      sed-opal.c
.blk-sysfs.o.cmd       blk-exec.c                blk-mq-tag.c            blk.h            t10-pi.c
.blk-timeout.o.cmd     blk-exec.o                blk-mq-tag.h            bounce.c
.bounce.o.cmd          blk-flush.c               blk-mq-tag.o            bounce.o
.bsg.o.cmd             blk-flush.o               blk-mq-virtio.c         bsg-lib.c
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/driver-api/mei$ cat /opt/linux/linux-5.4/blo
ck/.GIST
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{Y6cs1C8AR3qv-mQP0v9tvHBPL7Y.QX5IDO0wSN5gjNzEzW}
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/driver-api/mei$
    </details>



## What I learned
>* Bette rundestood the use of cammands *cat* *ls-a* and *cd*
## References
Just Used The Insructions
