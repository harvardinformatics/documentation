# Create New VM On eos-ctl01
 1. Connect to the vpn
 1. Launch libvirt, either on the machine with x-forwarding or on personal and add eos-ctl01.rc.fas.harvard.edu as an additional connection
 1. Launch new vm, choose iso from iso directory
 1. If you want to touch the openstack cluster, make sure you are on bridge br0. 
 If you want the outside world, then you want br.2444, ceph and other storage should be on br.600.
 1. Install and launch vm. If you are on internal network, 
 make sure dhcp is set to yes on boot in `/etc/sysconfig/network-scripts/[interface]`
