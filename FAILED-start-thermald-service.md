This error is more likely to occur on somewhat older computers. This is because thermald does not require a configuration file by default. To fix this error, we are going to install the following tool to generate the thermal_conf.xml configuration file.  

Type:  
`sudo apt install dptfxtract`  

Restart the service:  
`sudo systemctl restart thermald`
