## Connecting to DIDE from outside

Plug in with a wired network cable in the department whenever you have that option. If you don't, then there are various options.

### The Terminal Services Gateway (Windows to Windows)

To login to a Windows machine inside DIDE, from a Windows machine outside of dide, see the instructions 
[here](https://mrcdata.dide.ic.ac.uk/wiki/index.php/Remote_access_to_DIDE) - but note that although
these instructions _should work_ for Linux, mileage varies and ICT have not yet been able to 
resolve the issues. From Linux, use Pulse Secure below.

### Pulse Secure 

* The latest installers for Pulse Secure are on the
**Temp Drive IT folder** (*\\\\fi--didef3.dide.ic.ac.uk\Tmp\VPN*) - but this may be hard to access from outside when you don't
have Pulse Secure yet. These, however, might be more recent than the copies below.

* For Windows and Mac, you can try the web method [here](https://secureaccess.imperial.ac.uk), but this hasn't been
reliable on Linux, and on the working platforms involves some download. So for all platforms, the best solution is to
use the method below.

### Linux Pre-Flight

If you're installing on Linux, do these steps first. (These are tested on Ubuntu, but not Centos).

```
wget http://fr.archive.ubuntu.com/ubuntu/pool/universe/w/webkitgtk/libjavascriptcoregtk-1.0-0_2.4.11-3ubuntu3_amd64.deb
wget http://fr.archive.ubuntu.com/ubuntu/pool/universe/w/webkitgtk/libwebkitgtk-1.0-0_2.4.11-3ubuntu3_amd64.deb
wget http://security.ubuntu.com/ubuntu/pool/main/i/icu/libicu60_60.2-3ubuntu3.2_amd64.deb
sudo dpkg -i libicu60_60.2-3ubuntu3.2_amd64.deb libjavascriptcoregtk-1.0-0_2.4.11-3ubuntu3_amd64.deb libwebkitgtk-1.0-0_2.4.11-3ubuntu3_amd64.deb
sudo apt install -f
```

### Installation and Settings

* Download the client for [Windows](https://mrcdata.dide.ic.ac.uk/resources/ps-pulse-win.exe),
[Mac OS](https://mrcdata.dide.ic.ac.uk/resources/ps-pulse-mac-9.0r4.0-b1731-installer.dmg),
[Linux Ubuntu/Debian](https://mrcdata.dide.ic.ac.uk/resources/pulsesecure_9.1.R13_amd64.deb)
or [Linux Centos](https://mrcdata.dide.ic.ac.uk/resources/pulsesecure-9.1-R13.x86_64.rpm).
* The Server URL is `https://secureaccess2.imperial.ac.uk/connect`
* Your username and password are your **IC credentials** - the one used to read your email - and this gets you
access to your DIDE resources. The login is now similar to other Microsoft logins, and may involve two-factor authentication.


### See also

* The DIDE IT help page about the VPN [here](https://mrcdata.dide.ic.ac.uk/wiki/index.php/VPN_access_to_DIDE).
