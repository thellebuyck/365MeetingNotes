# RHEL VM Configuration Instructions

These instructions are for cloning a VM in VCenter.   This is a standard setup for Linux Redhat environments

## Cloning Process

These are the instructions for cloning a new Virtual Machine.

1. Login into VCenter
1. Search for the base virtual machine that you want to clone.
    1. Make sure you get the cluster, storage and host information. This will be important.
1. When you begin the clone process, make sure to do the following:
    1. Clone to the same cluster.  If the base VM is in the ManagedWay cluster, select ManagedWay.  If the base clone is in the Signs365 Cluster, select Signs365.
    1. Provide a unique name for the VM.
    1. Select a storage location that is different from the source virtual machine.  It is important to not select the same storage location as the source virtual machine.  If you select the same location as the source virtual machine, the clone process will take longer.
    1. On the clone options, be sure to uncheck all three checkboxes.  
    1. Click Next and then Finish and the clone process will begin.

## Configuration Process

These are the steps for configuring a cloned virtual machine. This guide will help you setup a RHEL virtual machine from the command line.

1. Login to VCenter
1. Before starting the virtual machine, ensure that the virtual machine is not connected to the network
    1. From the Summary tab:  Edit Settings -> Uncheck the box next to ```Network Adapter 1``` labeled ```Connected```
    1. Start the virtual machine.
    1. Launch the virtual machine.
1. Login with root user credentials (see LastPass for credentials).
1. On the command line type the command ```nmtui``` and press enter.  This command will launch the Network Manager TUI utility.
1. From the Network Manager TUI
    1. Edit a connection - choose the option ```ens192```
        1. Tab over to the IP Address and enter a new address*.
            1. * To get a new address, you will need a utility like ```Angry IP Scanner``` to find an address that is not currently in use
        1. Tab down to "OK" to save the information
            1. You should not need to change the Domain, DNS or gateway information.
        1.  Tab to the ```Back``` option and return to the main menu
    1. Select ```Set system hostname``` option
        1. From here set the Fully Qualified Domain Name for the local domain
            1. i.e. ```hqclonedvm01d.signs365.local```
        1. Tab to ```Ok``` and return to the main menu.
        1. Select ```Quit``` and return to the command line.
    1. Return to VCenter and the ```Edit Settings``` link and check the box next to the ```Network Adapter 1``` that says ```Connected```
    2. From the command line issue the following command ```service network restart```
        1. You should be able to ping an external address from the command line as well as ping the virtual machine from another machine on the network.