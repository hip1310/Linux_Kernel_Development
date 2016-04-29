Installing and removing my custom module.Prining message in syslog.

1. Write module code in hello.c file
2. created Makefile 
3. In makefile specified my module with obj-m += hello.o
4. Also, in make specified make -C command for changing directory to current kernel's build directory, getting information from the kernel's makefile for Processsor information, compiler information, etc. and then specified to load only my kernel module from present directory using M=$(PWD)
5. make command
6. installed the module using sudo insmod hello.ko command. So, used my module's kernel object file for installing the module
7. removed the module using rmmod hello command.
8. viewed the syslog 