# POO Lab.0
## Păgânu Andrei, FAF-212

A short explanation of how I installed Arch on my machine.

Screenshots of the process of the flashing of the ISO image to my flash does not exist.
Rebooted my PC, entered UEFI mode, put the flash drive as the first in the boot order.


* Initial screen
![re](images/20220911_185320.jpg) 
Console shown, ready to operate.

---

* Turning on WIFI
![](images/20220911_185406.jpg)
Software lock on WIFI adapter lifted by editing the `rfkill list`.

---
* Syncing time
![](images/20220912_092755.jpg)

---
* Connecting to wifi
![](images/20220912_092358.jpg)
`iwctl` used to connect to wifi.

---
* Partitioning disk
![](images/20220912_101909.jpg)
![](images/20220912_102008.jpg)
Created two partitions out of the free space.

---
* Building the file system.
![](images/20220912_102533.jpg)
![](images/scree1.png)
I attempted to use `pacstrap` without setting the mountpoints.
I then corrected the mistake.

---
* Using pacstrap to make the new system installation.
![](images/20220912_102713.jpg)

---
* Generaating `fstab` file
![](images/20220912_104023.jpg)

---
* Setting zone, installing Vim
![](images/20220912_104349.jpg)

---
* Editing locale file.
![](images/20220912_104833.jpg)

---
* `hostname` file was edited

---
* Editing hosts file
![](images/20220912_105800.jpg)

---
* Adding password to root, new user created, password for user.
![](images/20220912_110458.jpg)
User was added to groups, for privileges.

---
* `sudoers` file was edited
![](images/20220912_110625.jpg)
So that the user being in the wheel group matters.

---
* Installing Network Manager
![](images/20220912_110706.jpg)
So that I have access to the internet after booting into the system.
It was later enabled with `systemctl enable NetworkManager`

---
* Installing tools to set up the dual boot
![](images/20220912_110855.jpg)
Refind is a boot manager.
Installing refind
![](images/20220912_111028.jpg)
![](images/20220912_111513.jpg)
A config file had to be edited to put in the path to the partition where Linux is installed.

---
* After this, /mnt was unmounted, system reboot.
![](images/20220912_112042.jpg)

---
* Refind boot manager
![](images/20220912_112110.jpg)

---
* CLI log in screen.
![](images/20220912_112252.jpg)

---
* Video driver installation
![](images/20220912_113757.jpg)

---
* Installing xorg
![](images/20220912_113900.jpg)
Xorg is an interface between graphical software and hardware.

---
* Installing LightDM
![](images/20220912_115143.jpg)
LightDM is a desktop manager. It was installed through pacman and then enabled.
A greeter was also installed.

---
* Desktop environment xfce4 installed.
![](images/20220912_131809.jpg)

---
* Login screen and desktop
![](images/20220912_144024.jpg)
![](images/20220912_145123.jpg)

---
`git` was installed with `sudo pacman -S git` along with other developement tools.

---
* A directory for labs was created.
![](images/Screenshot_2022-09-13_14-02-20.png)
Git was initalised in this directory.

---
* Basic git configuration.
![](images/Screenshot_2022-09-13_14-11-13.png)
Files added to git.

---
* Files were commited
![](images/Screenshot_2022-09-13_14-13-09.png)

---
* At some point, the command `git remote add origin` was run.

---
* Files were pushed.
![](images/Screenshot_2022-09-13_15-19-55.png)

---
* Making the `makefile` in the directory with the `.c` file.
![](images/makefile1.png)

---
* Writing the makefile.
![](images/makefile2.png)

---
* Makefile made
![](images/makefile3.png)

---
* Running the makefile
![](images/makefile4.png)

---
* Running the executable
![](images/makefile5.png)

---