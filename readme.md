### Creating a NAS using Debian CLI and an OrangePi 5

Install and flash Debian CLI (bullseye) to MicroSD card to use in OrangePi 5 (OPi5)

SSH into OPi5 and install openmediavault 
```
wget -O - https://raw.githubusercontent.com/OpenMediaVault-Plugin-Developers/installScript/master/install | sudo bash
```

Install Plex Media Server using
```
sudo apt-get install apt-transport-https

curl https://downloads.plex.tv/plex-keys/PlexSign.key | sudo apt-key add -

echo deb https://downloads.plex.tv/repo/deb public main | sudo tee /etc/apt/sources.list.d/plexmediaserver.list

sudo apt-get update

sudo apt install plexmediaserver
```

Added external USB harddrive as storage onto OpenMediaVault

Enabled user read/write ability

Configured and enabled NFS and SMB fileshare services

Successfully connected to NAS using network fileshare on windows



