# DPDK

## DPDK Quick Start on Ubuntu
### Link: http://www.dpdk.org/doc/quick-start

### Issues
#### When make, "fatal error: pcap.h: No such file or directory"
- sudo apt-get install libpcap-dev
- http://stackoverflow.com/questions/5779784/pcap-h-header-file-problem

#### When run "sudo echo 64 > /sys/devices/system/node/node0/hugepages/hugepages-2048kB/nr_hugepages", Permission denied
- https://www.cyberciti.biz/faq/ubuntu-linux-root-password-default-password/
- sudo bash

#### Deploying Intel DPDK in VirtualBox
- 
