# 102.1 Design hard disk layout

## Basics
>[! IMPORTANT]
> Like any contemporary OS, Linux uses files and directories to operate. But unlike Windows, it does not use A:, C:, D:, etc. In Linux, everything is in *one big tree, starting with
`/` (called root). Any partition, disk, CD, USB, network drive, ... will be placed somewhere in this huge tree.

## Unix directories
> []
> This might be your enlightening moment in your Linux journey. Understanding Filesystem Hierarchy Standard (FHS) can help you find your programs, configs, logs and more without having prior knowledge about them. The table below has been the standard the latest revision since 2015.

Directory	`Description`
bin	`Essential command binaries`
boot	`Static files of the boot loader`
dev	`Device files`
etc	`Host-specific system configuration`
home	`Home directory of the users`
lib	`Essential shared libraries and kernel modules`
media	`Mount point for removable media`
mnt	`Mount point for mounting a filesystem temporarily`
opt	`Add-on application software packages`
root	`Home directory of the root user`
sbin	`Essential system binaries`
srv	`Data for services provided by this system`
tmp	`Temporary files, sometimes purged on each boot`
usr	`Secondary hierarchy`
var	`Variable data (logs, ...)`
