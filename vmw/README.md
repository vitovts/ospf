VMWare


- VMware P2V Linux
 1. VMware vCenter Converter Single
 2. Connect to SSH (vim /etc/ssh/sshd_config -->> PasswordAuthentication yes) 
 3. ESXi(vCenter), Linux, VMware Converter -> tcp port 22, 443, 902
 4. GRUB (not LILO)
 5. del optical disk
 6. DHCP or (Option -->> Helper VW network IPv4 ip address static)
