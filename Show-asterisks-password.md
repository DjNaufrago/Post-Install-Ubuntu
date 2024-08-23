Displays asterisks when entering the password on a terminal (by default, it is not visible when typing).  

`sudo pico /etc/sudoers`  

Change the following line:

`Defaults        env_reset` 

For this:  

`Defaults        env_reset,pwfeedback`  

Save and close the file. That's all!
