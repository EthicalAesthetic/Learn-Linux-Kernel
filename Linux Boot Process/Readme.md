![Linux-Boot-Process](Resources/Screenshot%202025-09-25%20191506.png)

**Step 1** - When we turn on the power, BIOS (Basic Input/Output System) or UEFI (Unified Extensible Firmware Interface) firmware is loaded from non-volatile memory, and executes POST (Power On Self Test).

**Step 2** - BIOS/UEFI detects the devices connected to the system, including CPU, RAM, and storage.

**Step 3** - Choose a booting device to boot the OS from. This can be the hard drive, the network

**Step 3** - Select a boot device for the OS. This can be the hard drive, the network

**Step 4** - BIOS/UEFI runs the boot loader (GRUB), which provides a menu to choose the OS or the kernel or kernel options.

**Step 5** - After the kernel is ready, we now switch to the user space. The kernel starts up systemd as the first user-space process, which manages the processes and services, probes all remaining hardware, mounts filesystems, and runs a desktop environment.

**Step 6** - systemd activates the default.target unit by default when the system boots. Additional units are executed as well.

**Step 7** - The system runs a set of startup scripts and configures the environment.

**Step 8** - The users are presented with a login window. The system is now ready.



## Learning Video: 
Watch this video for a visual explanation of the Linux boot process: [Linux Boot Process Overview](https://youtu.be/XpFsMB6FoOs?si=qpnfKc0njE5xBojg)

[Another video](https://youtu.be/sebgrmiYdk4?si=iSTxZIX6teyKIhWy)

