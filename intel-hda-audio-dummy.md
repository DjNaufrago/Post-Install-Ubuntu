If your computer uses snd_hda_intel kernel module (Realtek ALC892 codec), sound don't work and system settings show Dummy Output, it can fixed add `options snd-hda-intel model=generic` at the end of the `/etc/modprobe.d/alsa-base.conf`.  

Only run this command once:  
`echo "options snd-hda-intel model=generic" | sudo tee -a /etc/modprobe.d/alsa-base.conf`  

You can try to set the model to `auto` instead of `generic`.  

Other models depending the computer hardware: https://docs.slackware.com/howtos:hardware:audio_and_snd-hda-intel#how_to_find_the_right_options
