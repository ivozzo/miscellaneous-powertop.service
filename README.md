# Systemd service collection 

This is a collection of custom systemd services.

## Description

Service | Description
---------|---------
 powertop.service | enabling this will start powertop with --auto-tune option
 gpu-manager.service | enabling this will send OFF signal to discrete GPU through acpi_call (you'll have to load the module on kernel)


## Usage

Copy this file in /etc/systemd/system with ```cp myService.service /etc/systemd/system/```
and then enable it with ```systemctl enable myService.service```

You can then reboot or simply start the service with ```systemctl start myService.service```