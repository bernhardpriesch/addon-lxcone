## Changelog

###V0.1 Beta (2015-07-13)

* Basic, initial version.
* It's able to:
    * Deploy and shutdown LXC containers (containers can be deployed with several disks attached).
    * Monitor nodes and containers.
    * Limit container's RAM.
    * Reboot, shutdown, reset and destroy containers.


###V0.3 Beta (2015-08-26)

* Several features added:
    * Support for LVM.
    * Hot-attach and detach NICs and HDDs (LVM and File-system)
    * Support for VNC.
    * Suspend, undeploy, power off and resume containers.
    * Deploy containers with several NICs and HDDs attached (LVM and File-System)
* Fixed containers monitorization issues.
* Fixed issues when adding several HDDs to a container.
* Improved NICs attachment.


###V0.4 Beta (2015-11-05)

* Improved error handling.
* Guide updated.
* Running containers will automatically start if node gets restarted.
* VNC improved.
* Several bugs fixed:
	* Fixed issues with container's hostname.
	* Fixed issues with reboot and hard reboot.
	* Fixed bridge selection in NIC hot-attaching.


###V1.0 (2015-12-17)

* Failure probe. In case any node is forcibly power off, or in case of an electrical failure, all containers that where running inside affected nodes
* NIC name matches with OpenNebula NIC ID when deploying.
* Support for Ceph.


###V1.1 (2016-04-1)

* Several issues fixed:
    * with Ubuntu as a node
    * with vnc server and connection 
    * with with attach disk   
    * when when cleaning the node 
    * with nic hot-attach
    * with poweroff and reboot compute node
* SNVCterm replaced VNCterm. Featuring:
    * It remove TLS requirements
    * Enables the usage of non-patched versions of libvncserver and others
    * Enables the usage of passwordless VNC console (it is the common usage in ONE)
    * Corrects problems in password checking

###V1.1.3 (2016-04-29)

* Issue when VNC connecting after VNC rebooting fixed
* LXC native logs now availabe in Sunstone Log
* Minor bugs fixed


###V1.1.4 (2016-11-21)

* Snapshots improved (using squashfs-tools)
* Migration improved (doing new deployment in restore because other node might not know about the lxc container yet)
* better LVM support (added lvchange commands)
* removed lxc-freeze and lxc-unfreeze commands
* improved integration with RedHat cluster


###TODO

* Live Migration
* Smooth enhanced logging
* Using LXC2 in Xenial Xerus
