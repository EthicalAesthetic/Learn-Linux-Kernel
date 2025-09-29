# Using Putty

It is a free open source terminal. <br>
Widely used for remote access to CLI (Command Line Interface) via SSH (Secure Shell)
- [Downlaoad putty](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)

We need the IP to access it remotely.But which IP, of our VM ?? 

If we use the command `hostname -I` in our VM's terminal it will show the private IP of the VM ie- 10.0.2.15 same for all of us. (if you enter this IP in putty to access the VM, it will throw and error).

![](Resources/Screenshot%202025-09-29%20193235.png)


But to access it remotely we need a private IP of our host system (Windows) which will have starting numbers from our network connection.
<br>
<b>To do so we have to change some Network Settings of ous VM</b>

- Go to Network Setting of your VM.

![](Resources/Screenshot%202025-09-29%20194406.png)

- Change RAT to Bridged Adapter. Click OK. And restart the VM. (You can use the command `reboot`)

🛑🛑Why this step..?🛑🛑
-

![](Resources/Screenshot%202025-09-29%20194828.png)

- Now check the IP using command `hostname -I`. It will give IP with starting numbers of your network connection.

![](Resources/Screenshot%202025-09-29%20195737.png)
![](Resources/Screenshot%202025-09-29%20200217.png)

- Now we can use this IP to access the VM remotely using Putty. Before that we have to install and start <b>OpenSSH</b> which is a service to access the VM remotely by connecting it to the server.<br>
   - `sudo apt install openssh-server`
   - `systemctl start ssh`

- Now type this IP in Putty to access the VM.

![](Resources/Screenshot%202025-09-29%20203222.png)

- Enter the username and password you created while installin UBUNTU.

![](Resources/Screenshot%202025-09-29%20203330.png)

### To confirm try making a directory from Putty.

<b>Note:</b> Your VM should be in running state to access it remotely.