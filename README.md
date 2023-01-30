# boot-screens
PXE Boot screens & menus

See [PXE Boot repo](https://github.com/chris18890/pxe-boot) for setup scripts

**note - livetxt.cfg will need updated with the IP address of the server**

**note - rescuetxt.cfg will need updated with the IP address/URL of the server that hosts the Clonezilla & GPartEd filesystems**

## structure

```
- <root dir>
  - boot-screens
  - rescue
    - avg (uses [Memdisk](https://www.syslinux.org/wiki/index.php?title=MEMDISK))
    - clonezilla (hosted locally via vmlinuz/initrd, squashFS served via http, see note above)
    - DBAN (uses Memdisk)
    - gparted (hosted locally via vmlinuz/initrd, squashFS served via http, see note above)
    - memtest86 (using the [bootable binary](http://memtest.org/#downiso))
    - pogostick (uses Memdisk)
  - ubuntu-installer (latest LTS Netboot image hosted locally via vmlinuz/initrd)
    - x64
  - ubuntu-live (desktop x64 hosted locally via vmlinuz/initrd, filesystem served over NFS, see note above)
    - bionic
    - cosmic
  - win7 (WIP, currently trying [wimboot](https://ipxe.org/wimboot))
    - x64
    - x86
```