<h1>PROXMOX</h1>

<h2>Description</h2>
I set up PROXMOX on my laptop.

Equipment I used for this set up:
- laptop (with charging cable)
- e-thernet to USB-C adapter cable
  - connects to router
- USB drive with Ventoy installed
  - You can install Ventoy on their webpage. [X](https://www.ventoy.net/en/index.html)
 

<h2>For laptops: Disable sleep function when closing lid</h2>
Enter the nano command below into the SHELL, to edit the file `/etc/systemd/logind.conf`.

(If you have a linux server, apply "sudo" in the beginning)

```
nano /etc/systemd/logind.conf
```

Navigate with the arrow keys to find and highlight the lines shown below. You can select multiple lines by pressing DEL on each line you want to edit. Change `HandleLidSwitch=suspend` to `HandleLidSwitch=ignore` and so on.

For `IdleActionSec` default time, change it to  `=0`.

Your config should look something like this:

```
... more lines ...
HandleLidSwitch=ignore
HandleLidSwitchExternalPower=ignore
HandleLidSwitchDocked=ignore
... more lines ...
IdleAction=ignore
IdleActionSec=0

```

Exit by pressing Ctrl+X, then Y and Enter to save changes.

<h2>Add static DHCP</h2>
Doing this reserves your local IP address so that the server's IP address does not change.
- Go to PROXMOX SHELL > type "ip a" into SHELL > pull from nic0: link/ ether
