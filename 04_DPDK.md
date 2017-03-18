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
- http://plvision.eu/blog/deploying-intel-dpdk-in-oracle-virtualbox/
- http://askubuntu.com/questions/365615/how-do-i-enable-multiple-cores-in-my-virtual-enviroment
 
## Getting Started Guide for Linux
- http://www.dpdk.org/doc/guides/linux_gsg/index.html

### 1. Introduction
- Data Plane Development Kit (DPDK)

### 2. System Requirements

#### 2.1. BIOS Setting Prerequisite on x86
- HPET timer and power management functionality
- HPET (High Precision Event Timer): https://en.wikipedia.org/wiki/High_Precision_Event_Timer

#### 2.2. Compilation of the DPDK
##### Required Tools
- GNU make
- coreutils: cmp (compare two file byte by byte), sed, grep, arch (print machine architecture), etc.
- gcc: versions 4.9 or later is recommended for all platforms. `gcc -dumpspecs`, -fstack-protector
- libc headers, often packaged as gcc-multilib, glibc-devel.x86_64
- Linux kernel headers or sources required to build kernel modules.
- Additional packages required for 32-bit compilation on 64-bit systems
- Python

##### Optional Tools
- Intel C++ Compiler (icc)
- IBM Advance ToolChain for Powerlinux
- libpcap headers and libraries (libpcap-devel) to compile and use the libpcap-based poll-mode driver. This driver is disabled by default and can be enabled by setting CONFIG_RTE_LIBRTE_PMD_PCAP=y in the build time config file.?
- libarchive headers and library are needed for some unit tests using tar to get their resources.
