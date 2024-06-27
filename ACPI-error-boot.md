Although it is displayed as an error, it is due to an incompatibility between the linux kernel and an old BIOS. When Linux tries to read some specific ACPI parameters, which don't exist, or are wrong, it fails and reports this kind of error. The recommendation is not to show it, but not to deactivate it.  
  
Open '/etc/default/grub' in an editor with root access (with pluma, gedit, pico, etc.).  
`sudo pluma /etc/default/grub`  

Change this line:  
`GRUB_CMDLINE_LINUX_DEFAULT='quiet splash'`  
  
For this:  
`GRUB_CMDLINE_LINUX_DEFAULT='quiet splash loglevel=3'`  

Save, exit and type in terminal:  
`sudo update-grub`  

Reboot and see the results.
