# VMWARE WORKSTATION 14
## Solve: “ERROR: NOT ENOUGH PHYSICAL MEMORY IS AVAILABLE TO POWER ON THIS VIRTUAL MACHINE WITH ITS CONFIGURED SETTINGS.”
```shell
sudo su
cd /tmp
cp -p /usr/lib/vmware/modules/source/vmmon.tar /usr/lib/vmware/modules/source/vmmon.tar~backup
cp /usr/lib/vmware/modules/source/vmmon.tar .
tar xf vmmon.tar
rm vmmon.tar
wget https://raw.githubusercontent.com/mkubecek/vmware-host-modules/fadedd9c8a4dd23f74da2b448572df95666dfe12/vmmon-only/linux/hostif.c
mv -f hostif.c vmmon-only/linux/hostif.c 
tar cf vmmon.tar vmmon-only
rm -rf vmmon-only
mv -f vmmon.tar /usr/lib/vmware/modules/source/vmmon.tar 
vmware-modconfig --console --install-all
```
Comments: “vmmon” is the virtual machine monitor kernel module. You need to modify the source file “hostif.c,” and rebuild the kernel module by running code above.

Original link: http://blog.nowherelan.com/2017/12/04/vmware-workstation-14-error-not-enough-physical-memory-is-available-to-power-on-this-virtual-machine-with-its-configured-settings/
