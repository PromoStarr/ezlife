# Arma 3 Gibson Install Notes

Arma3 is installed in the /mnt/data/steam/arma3 dir
force_install_dir /mnt/data/steam/arma3 is required for steamCMD validation

Startup is controlled by a script in /etc/systemd/system/arma3.service which in turn calls a bash script in /mnt/data/steam/arma3/start.sh

This script applies some startup config, pointing to custom config files and mods.

# Start, Stop, Check the Service
Systemctl takes care of the service for us use:
sudo systemctl status/start/stop/restart arma3.service

to watch console output use status or 
``` $ journal -fu arma3.service ```

# Mods installs (Script usage)
This script does the mod installs. 

Script not developed enough to fill in this bit
