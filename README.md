# Docker Container for FHEM

Docker image for FHEM based on Debian Jessie for usage with USB Cul
Be aware of the FHEM ports being open ... dont use this without a
reverse proxy if exposed to public networks.

The config shiped with this repo is an example with MAX! heating systems
and intertechno IT-1500 switches.

In order to "learn" new devices, you will have to comment in the following 
lines in the fhem.cfg file

```
#define autocreate autocreate
#attr autocreate autosave 1
#attr autocreate filelog ./log/%NAME-%Y.log
```

Run Directly:
```
./install
```
Rerun with altered config
```
./reinstall
```
Config files:
```
fhem.cfg
```
Reread config:
```
./restart
```
