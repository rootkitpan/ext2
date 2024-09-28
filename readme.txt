


sudo qemu-system-x86_64 \
	-m 2048 \
	-kernel ./linux/arch/x86/boot/bzImage \
	-append "rdinit=/sbin/init rw rootfstype=9p rootflags=trans=virtio"
	-virtio local,id=root,mount_tag=/dev/root,security_model=passthrough,path=./busybox/_install






