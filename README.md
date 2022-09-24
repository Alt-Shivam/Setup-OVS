# Setup-OVS on Ubuntu

## Become root user
```
sudo su
```
## Install required packages
```
sudo apt install -y build-essential fakeroot graphviz autoconf automake bzip2 debhelper dh-autoreconf libssl-dev libtool openssl procps python-all python-zopeinterface module-assistant dkms make libc6-dev python-argparse uuid-runtime netbase kmod  iproute2 openvswitch-switch
```
## Clone OVS repo
```
git clone https://github.com/openvswitch/ovs.git --depth 1
```
## Cd to directory and install ovs
```
cd ovs
./boot.sh
./configure
make
```
