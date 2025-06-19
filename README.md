# Free5GC Virtual Machine Configuration (libvirt)

This repository contains the Libvirt XML configuration file used to deploy a virtual machine (VM) for benchmarking the Free5GC core in a virtualized environment. The VM was configured to host all core network functions except the User Plane Function (UPF), which was evaluated separately in bare metal and containerized setups.

## Files

- `free5gc-vm.xml`: Libvirt domain definition file specifying CPU, memory, disk, network interfaces, and other VM parameters.

## Usage

To create the VM using this configuration:

```bash
virsh define free5gc-vm.xml
virsh start free5gc-vm

