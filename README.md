# sercomm_s3_change_bootflag_to_install_OpenWrt
edited config file for sercomm s3 router

Upload Sercomm_s3_config.cfg to your router

In this config i already enabled ssh on 192.168.1.1

here are the login details

Config file password  E1234

admin   E12345678

SuperUser E12345678

Login via SSH at 192.168.1.1 with SuperUser

then press sh in shell

then issue the following command to set bootflag to "Boot Flag : Sercomm1"

printf 1 | dd bs=1 seek=7 count=1 of=/dev/mtdblock3

reboot

Then login to web interface & login using admin account

upload OpenWrt-Factory image using the web interface..
