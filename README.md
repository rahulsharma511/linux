CMPE 283 Assignment 1

Steps followed for completing assignment:
1.Create a virtual machine with any linux distribution(ubuntu 20.04 lts used for this assignment purpose)
2.Fork torvalds/linux git repo to your github and clone the forked repo into your virtual machine.
3.Make sure to run apt update and install build essentials, make, flex etc.
4.copy config from boot to a .config file and make sure to copy the same config file version that matches with the one which appears when uname -a command is fired
5.now run make oldconfig then run make prepare 
6.now build modules and then build kernal (cmd: make -j 4 modules, cmd: make -j 4)
7.finally install the modules and kernal and do a reboot.
8.now run make command in the directory where makefile and cmpe283.c file exists this will build and load the module.
9.now check the output in the system message buffer(cmd:dmesg)
