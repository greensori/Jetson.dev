* with TX1 board

1. jetson start Setting (need one more ubuntu pc)

jetson id/pw : ubuntu/ubuntu

**jetson board : 

checking kernel version: $uname -r

checking linux bit : $ uname -m

ip checking : $ ifconfig

-ssh connecting:

port checking : $ netstat -tnlp

ssh checking : $ ssh

installing openssh : $ sudo apt-get install openssh-server

generate key using ssh-keygen(overwrite) : 

$ sudo ssh-keygen -t rsa -f /etc/ssh/ssh_host_rsa_key

$ sudo ssh-keygen -t dsa -f /etc/ssh/ssh_host_dsa_key


**hostPC:

connenting SSH : ssh ubuntu@ipAddress

move to home : cd ~

move to nvidia directory : cd NVIDIA-INSTALLER

read manual : cat README.txt

lausnch shell script : $ sudo ./installer.sh

after reboot : sudo reboot

optional(file send from jetson to hostPC) : $scp -r JetPack-${version}.run {hostpc}@ipAddress

JetPackinstall :

$ chmod +x JetPack-${version}.run

$ ./JetPack-${version}.run
