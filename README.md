# boot-screens
PXE Boot screens & menus

See [PXE Boot repo](https://github.com/chris18890/pxe-boot) for setup scripts

**note - livetxt.cfg will need updated with the IP address of the server**

## structure

- `<root dir>`
  - `boot-screens`
  - `rescue`
    - `avg ` (uses [Memdisk](https://www.syslinux.org/wiki/index.php?title=MEMDISK))
    - `DBAN` (uses Memdisk)
    - `memtest86` (using the [bootable binary](http://memtest.org/#downiso))
    - `pogostick` (uses Memdisk)
  - `ubuntu-installer` (latest LTS Netboot image hosted locally via vmlinuz/initrd)
    - `x64` (Focal)
  - `debian-installer` (latest Stable Netboot image hosted locally via vmlinuz/initrd)
    - `x86` (Bookworm)
  - `ubuntu-live` (desktop x64 hosted locally via vmlinuz/initrd, filesystem served over NFS, see note above)
    - `noble`
    - `jammy`
    - `focal`
