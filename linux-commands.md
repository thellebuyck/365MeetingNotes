# Linux Commands

Below are commands for certain troubleshooting efforts in the linux environment.   These pertain to zombied processes, open file descriptors, runaway processes.   These come in handy when we are trying to troubleshoot FileBucket, Upload server, etc.


## Commands to Troubleshoot

```ps -aef |grep php |grep master
strace -p <master pid>
then read that output to see what its hanging on
check my descriptors;
ls -al /proc/$$/fd
if I am not holding anything something else is
check my shared memory segments;
ipcs
see the stale segement referenced in my strace
ipcrm that segment
then drop my caches and sync closed descriptors
sync ; echo 3 > /proc/sys/vm/drop_caches
^^^ I know thats logic but there is some interpertation to the troubleshooting```