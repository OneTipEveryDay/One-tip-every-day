101.1 Determine and configure hardware settings from jadi

#udev

udev (userspace /dev) is a device manager for the Linux kernel.udev also handles all user space events raised when hardware devices are added into the system or removed from it
(/dev is a special directory that contains device files, also known as special files. These files represent and provide an interface to hardware devices and pseudo-devices (virtual devices managed by the kernel)
Everything is a file:
In Linux, the philosophy is "everything is a file." This extends to hardware devices, which are represented as files within the /dev directory. This allows users and programs to interact with hardware using standard file operations like reading from and writing to files.)

In essence, udev serves as the custodian of the /dev/ directory. It abstracts the representation of devices, such as a hard disk, which is identified as /dev/sda or /dev/hd0, irrespective of its manufacturer, model, or underlying technology

proc directory
This is where the Kernel keeps its settings and properties. This directory is created on ram and files might have write access (say for some hardware configurations). You can find things like:

IRQs (interrupt requests)
I/O ports (locations in memory where CPU can talk with devices)
DMA (direct memory access, faster than I/O ports)
Processes
Network Settings

