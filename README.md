### root@proxmox:~# qm create 104 -agent 1 -bios ovmf -name HomeAssistant -net0 virtio,bridge=vmbr0   -onboot 1 -ostype l26 -scsihw virtio-scsi-pci
### root@proxmox:~# pvesm alloc local 104 vm-104-disk-0.qcow2 128
### root@proxmox:~# qm importdisk 104 haos_ova-7.4.vmdk local -format qcow2
