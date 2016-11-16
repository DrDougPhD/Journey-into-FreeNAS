# Journey-into-FreeNAS
Notes, scripts, and other things related to my journey into a FreeNAS installation and configuration.

## First Installation

1. Download the current stable release of FreeNAS from [here](http://www.freenas.org/download-freenas-release/).
2. Write the downloaded FreeNAS-9.10.1-U4.iso file to a 1GB USB flash drive.  
    $ sudo dd if=FreeNAS-9.10.1-U4.iso of=/dev/sdb bs=4M
3. Plug said flash drive into system and boot.
This will likely require frantic smashing of [F12] immediately after powering on.
4. Once the installation window is reached, plug in another flash drive with at least an 8GB capacity.
5. Follow installation instructions to install on that drive.
6. Reboot system, unplug 1GB drive, boot into FreeNAS.

## Initial Configuration
1. Upon booting, FreeNAS will do some randomization stuff that I'm not familiar with.
Let that do its thing.
2. Once finished, a Console setup prompt will pop up asking for network interface configuration.
Do that.
3. Now all that's left is to start configuring stuff within the FreeNAS web interface.
Point your web browser to [http://freenas.local/](http://freenas.local/) to access your system.

## Things I need to do
* Install ssh
* View the system log.
  * Analogous to dmesg in Linux.
