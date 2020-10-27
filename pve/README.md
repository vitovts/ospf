PVE

- Configure network
```
vim /etc/network/interfaces
apt-get update
apt-get upgrade
apt-get install mc vim net-tools
systemctl restart network
```

- Add hdd
```
fdisk -l
fdisk /dev/sdb
mkfs.ext4 /dev/sdb1
mkdir /mnt/hdd1
mount -t ext4 /dev/sdb1 /mnt/hdd1
vim /etc/fstab 
```

- Create vm on winxp
```
- WinXP
  - NIC Realtek 8139 
```


```
pvecm status

dpkg-reconfigure locales

```
