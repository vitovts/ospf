Create CT on PVE witch Docker

- Add in config CT

vim /etc/pve/local/lxc/1XX.conf
```
arch: amd64
cores: 2
insert--->>>features: keyctl=1,nesting=1
hostname: xxx
memory: 2048
nameserver: x.x.x.x
net0: name=eth0,bridge=vmbr0,firewall=1,hwaddr=xx:xx:xx:xx:xx:xx,ip=dhcp,type=veth
ostype: ubuntu
rootfs: local-lvm:vm-xxx-disk-0,size=20G
swap: 512
unprivileged: 1
```

- Install
```
apt update -y
apt-get install curl -y
wget -O - https://raw.githubusercontent.com/vitovts/proto/master/work/cogniteq/docker-lxc-init-1.sh | bash
```
