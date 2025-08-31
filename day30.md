# 102.1 Design hard disk layout

## Basics
>[! IMPORTANT]
> Like any contemporary OS, Linux uses files and directories to operate. But unlike Windows, it does not use A:, C:, D:, etc. In Linux, everything is in *one big tree, starting with
`/` (called root). Any partition, disk, CD, USB, network drive, ... will be placed somewhere in this huge tree.

## Unix directories
> []
> This might be your enlightening moment in your Linux journey. Understanding Filesystem Hierarchy Standard (FHS) can help you find your programs, configs, logs and more without having prior knowledge about them. The table below has been the standard the latest revision since 2015.


+ [x] bin	`Essential command binaries` <br>
```sh
 boot	Static files of the boot loader ```
<br>
dev	`Device files`<br>
etc	`Host-specific system configuration`<br>
home	`Home directory of the users`<br>
lib	`Essential shared libraries and kernel modules`<br>
media	`Mount point for removable media`<br>
mnt	`Mount point for mounting a filesystem temporarily`<br>
opt	`Add-on application software packages`<br>
root	`Home directory of the root user`<br>
sbin	`Essential system binaries`<br>
srv	`Data for services provided by this system`<br>
tmp	`Temporary files, sometimes purged on each boot`<br>
usr	`Secondary hierarchy`<br>
var	`Variable data (logs, ...)`<br>

## Partitions


