#102.1 Design hard disk layout

##Basics
>[]
> Like any contemporary OS, Linux uses files and directories to operate. But unlike Windows, it does not use A:, C:, D:, etc. In Linux, everything is in *one big tree, starting with
`/` (called root). Any partition, disk, CD, USB, network drive, ... will be placed somewhere in this huge tree.

##Unix directories
This might be your enlightening moment in your Linux journey. Understanding Filesystem Hierarchy Standard (FHS) can help you find your programs, configs, logs and more without having prior knowledge about them. The table below has been the standard the latest revision since 2015.
