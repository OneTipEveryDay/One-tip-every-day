<div align="center">
<h1>Partitions</h1>

> [!IMPORTANT]
>  You have to PARTITION the disks, that is to create smaller parts on a big disk. These are self-contained sections on the main drive. OS sees these as standalone disks. We recognize them as: - /dev/sda1 (first partition of the first SCSI disk) - /dev/hdb3 (3rd partition on the second disk)
>

'fdisk' command examples in Linux
Let us look at some of the ways in which 'fdisk' command can be used in Linux.

## View All Disk Partitions
```b
$ sudo fdisk -l
```
<img src = "https://media.geeksforgeeks.org/wp-content/uploads/20190219150511/Screenshot-671.png">

## gparted

`A graphical tool for managing disks and partitions.

## LVM

> [! important]
> In many cases, you need to resize your partitions or even install new disks and add them to your current mount points; Increasing the total size. LVM is designed for this.
> `


## swap

> [! NOTE]
> Swap in Linux works like an extended memory. The Kernel will page memory to this partition/file. It is enough to format one partition with swap file system and define it in /etc/fstab (you will see this later in 104 modules).
>
> 



# 102.2 Install a boot manager

## Boot overview

> Most systems use BIOS or UEFI. When on BIOS, the system will do a self test called POST (Power-On Self-Test). Then it will hand over the boot process to the first sector of Master Boot Record (MBR)
> MBR is only 512 bytes so we need a smart bootloader to handle larger boot managers and even multiple systems. Some of these boot loaders are LILO, GRUB and GRUB2.
> If the system is using UEFI, the hardware will follow the UEFI stages. They start with a security phase and will continue till the end phase where the UEFI looks for an EFI System Partition, which is just a FAT32 partition (Usually the first one, but that's implementation-defined) with PE executables and runs them.
> In both cases, the binary starts the boot loader. It might be a complete bootloader on /boot/efi/ of your computer or a small loader for the main grub on the MBR or a windows loader or even a chainloader.
>

#102.4 Use Debian package management





















</div>
