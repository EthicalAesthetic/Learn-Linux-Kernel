# Virtualisation
In this Guide we will use Oracle Virtual Box to use Linux. It is a type-2 hypervisor

## Downloads
- [Oracle Virtual Box](https://www.virtualbox.org/wiki/Downloads)
- Any Linux Distro's ISO file. (we will be using [Ubuntu](https://ubuntu.com/download/desktop))

## Setting Up Virtual Machine 
- Open the Virtual Box
- Click on NEW to create a new Virtual Machine
- Choose the folder in which you have atleast 20-50 GB free space
- Choose the ISO file (Ubuntu) in the ISO Image option.

![](Resources/Screenshot%202025-09-28%20033350.png)

- For Ubuntu it is recomended to allocate atleast 4GB (4096MB) RAM  and 2 CPUs.
- Start by allocating 20GB of Storage (Can be changed later) .

## Setting up UBUNTU
- After Powering up th VM chose "Try or Install UBUNTU"
- Follow the steps (very self-explanatory)

![](Resources/Screenshot%202025-09-28%20222959.png)

It is not visible in the full screen mode. We will fix it. 

## Fixing the resolution error / Entering the full screen
- From the Devices Tab choose the "Insert Guest Addition CD image. 

![](Resources/Screenshot%202025-09-28%20223812.png)

- You will see this CD disk icon.
- Before open this, open the Linux Terminal and type the command `sudo apt-get install bzip2 tar` to download the softwares (bzip and tar).
- Enter your password and press 'y' to start installation.

![](Resources/Screenshot%202025-09-28%20225532.png)

- Click the CD icon and Run the software.

![](Resources/Screenshot%202025-09-28%20225745.png)

- Power of the Machine by pressing cross button. 

<div align="center">
<img src="Resources/Screenshot 2025-09-28 230554.png" width=40%>
</div>

- Start the VM again, it will be resolved.

![](Resources/Screenshot%202025-09-28%20231410.png)

You can later eject that CD disk by right clicking on its icon and choosing "eject".

