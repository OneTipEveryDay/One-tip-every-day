101.3 Change runlevels / boot targets and shutdown or reboot the system

The following is a partial list of the used files, terms and utilities:
/etc/inittab
shutdown
init
/etc/init.d/
telinit
systemd
systemctl
/etc/systemd/
/usr/lib/systemd/
wall

runlevels
Runlevels define what tasks can be accomplished in the current state (or runlevel) of a Linux system. Think of it as different stages of being alive.

systemd
On systemd, we have different targets which are groups of services:

root@debian:~# systemctl list-units --type=target # On a Debian machine
  UNIT                LOAD   ACTIVE SUB    DESCRIPTION


root@debian:~# systemctl get-default 
graphical.target

root@debian:~# systemctl status multi-user.target 
● multi-user.target - Multi-User System
     Loaded: loaded (/lib/systemd/system/multi-user.target; static)
     Active: active since Sat 2022-05-07 11:58:36 EDT; 4h 24min left
       Docs: man:systemd.special(7)

It is also possible to isolate any of the targets or move to two special targets too:

rescue: Local file systems are mounted, no networking, and root-user only (maintenance mode)
emergency: Only the root file system and in read-only mode, No networking and root-user only(maintenance mode)
reboot
halt: Stops all processes and halts CPU activities
poweroff: Like halt but also sends an ACPI shutdown signal (No lights!)

SysV runlevels
On SysV we were able to define different stages. On a Red Hat-based system we usually had 7:

0- Shutdown
1- Single-user mode (recovery); Also called S or s
2- Multi-user without networking
3- Multi-user with networking
4- to be customized by the admin
5- Multi-user with networking and graphics
6- Reboot
And in Debian based system we had:

0- Shutdown
1- Single-user mode
2- Multi-user mode with graphics
6- Reboot

