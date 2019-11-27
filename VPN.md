## Connecting to DIDE from outside

Plug in with a wired network cable in the department whenever you have that option. If you don't, then there are various options.

* The latest installers for Pulse Secure are on the
**Temp Drive IT folder** (*\\\\fi--didef3.dide.ic.ac.uk\Tmp\VPN*) - but this may be hard to access from outside when you don't
have Pulse Secure yet. These, however, might be more recent than the copies below.

* For Windows and Mac, you can try the web method [here](https://secureaccess.imperial.ac.uk), but this hasn't been
reliable on Linux, and on the working platforms involves some download. So for all platforms, the best solution is to
use the method below.

### Linux Pre-Flight

If you're installing on Linux, do these steps first. (These are tested on Ubuntu, but not Centos).

* `sudo apt install libwebkitgtk-1.0-0:i386 libdconf1:i386 dconf-gsettings-backend:i386`
* `echo "/usr/local/pulse" | sudo tee /etc/ld.so.conf.d/pulse.conf`
* `sudo ldconfig`
* `sudo apt install net-tools`

### Installation and Settings

* Download the client for [Windows](https://mrcdata.dide.ic.ac.uk/resources/ps-pulse-win-5.3r6.0-b1769-64bitinstaller.msi),
[Mac OS](https://mrcdata.dide.ic.ac.uk/resources/ps-pulse-mac-5.3r6.0-b1769-installer.dmg),
[Linux Ubuntu/Debian](https://mrcdata.dide.ic.ac.uk/resources/ps-pulse-linux-5.3r6.0-b1769-ubuntu-debian-64-bit-installer.deb)
or [Linux Centos](https://mrcdata.dide.ic.ac.uk/resources/ps-pulse-linux-5.3r6.0-b1769-centos-rhel-64-bit-installer.rpm).
* The Server URL is `https://secureaccess.imperial.ac.uk`
* Your username and password are your **IC credentials** - even though this gets you
access to your DIDE resources. The username is in simple form, with no domain prefix or suffix. The password will
be the one you use to read your email.

### See also

* The DIDE IT help page about the VPN [here](https://mrcdata.dide.ic.ac.uk/wiki/index.php/VPN_access_to_DIDE).
