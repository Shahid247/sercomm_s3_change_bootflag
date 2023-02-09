Here are the OEM Backup files from Sercomm S3

Firmware Files i.e mtd6 & mtd7 are in compressed zip format. unzip & use binary .bin file only.

Unlock MTD Partition for writing (be carefull when writing bootloader)

opkg install kmod-mtd-rw

insmod mtd-rw.ko i_want_a_brick=1
