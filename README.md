# boot-screens
PXE Boot screens & menus

See [PXE Boot repo](https://github.com/chris18890/pxe-boot) for setup scripts

** note - livetxt.cfg will need updated with the IP address of the server **

** note - rescuetxt.cfg will need updated with the IP address/URL of the server that hosts the Clonezilla & GPartEd filesystems **

## structure

```
- <root dir>
  - boot-screens
  - rescue
    - avg
    - clonezilla
    - DBAN
    - gparted
    - memtest
    - pogostick
  - ubuntu-installer (latest LTS)
    - x64
    - x86
  - ubuntu-live (desktop x64)
    - xenial
    - bionic
  - win7
    - x64
    - x86
```