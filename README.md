# Kernel-Linux
Configuración del Kernel Linux en Gentoo

## NECESARIOS PARA LINUX

### Montar automaticamente DEVTMPFS

Búsqueda rápida: CONFIG_DEVTMPFS_MOUNT

```
[*] Maintain a devtmpfs filesystem to mount at /dev
```

### Soporte de disco SCSI

Búsqueda rápida: CONFIG_BLK_DEV_SD

```
SCSI device support -->
     <*> SCSI disk support
     <*> SCSI CDROM support
     <*> SCSI generic support

     [ ] SCSI low-level drivers --->
```
### Sistema de Archivos EXT4 (Sistema de Archivos Linux) y FUSE (Para compartir archivos MTP)
Búsqueda rápida: CONFIG_EXT4_FS

```
<*> Second extended fs support
<*> The Extended 3 (ext3) filesystem
<*> The Extended 4 (ext4) filesystem
[*] Ext4 POSIX Access Control Lists
[*] Ext4 Security Labels
<*> FUSE (Filesystem in Userspace) support
```

### Sistema de Archivos Microsoft

Búsqueda rápida: CONFIG_VFAT_FS

```
<*> MSDOS fs support
<*> VFAT (Windows-95) fs support
```
### Soporte de etiquetado de particiones GPT

Búsqueda rápida: CONFIG_PARTITION_ADVANCED

```
[*] Advanced partition selection
[*] EFI GUID Partition support
```
### Soporte para el cargador EFI y sus variables en el Núcleo Linux

Búsqueda rápida: CONFIG_EFI

```
[*] EFI runtime service support
[*]   EFI stub support
[*]      EFI mixed-mode support
```

## DRIVERS ESPECÍFICOS

### Gráficos Integrados Intel HD Graphics

Búsqueda rápida: CONFIG_DRM_I915


```
    <*> Direct Rendering Manager (XFree86 4.1.0 and higher DRI support)  --->
        ARM devices  ----
    < > ATI Radeon
    < > AMD GPU
    < > Nouveau (NVIDIA) cards
    <*> Intel 8xx/9xx/G3x/G4x/HD Graphics
    ()    Force probe driver for selected new Intel hardware
    [*]   Enable capturing GPU state following a hang
    [*]     Compress GPU error state
    [*]   Always enable userptr support
    [ ]   Enable Intel GVT-g graphics virtualization host support
```

### Tarjeta de sonido

Búsqueda rápida: CONFIG_SND_HDA_INTEL

```
<*> HD Audio PCI
[*] Build hwdep interface for HD-audio driver
[ ] Allow dynamic codec reconfiguration
[ ] Support digital beep via input layer
[ ] Support initialization patch loading for HD-audio
<*> Build Realtek HD-audio codec support
< > Build Analog Devices HD-audio codec support
< > Build IDT/Sigmatel HD-audio codec support
< > Build VIA HD-audio codec support
<*> Build HDMI/DisplayPort HD-audio codec support
```
### Dispositivos de entrada USB

Búsqueda rápida: CONFIG_HID_GENERIC

```
HID support --->
     -*- HID bus support
     <*> Generic HID driver
     [*] Battery level reporting for HID devices
         USB HID support --->
              <*> USB HID transport layer
```

### USB 3.0 y 2.0

Búsqueda rápida: CONFIG_USB_XHCI_HCD

```
[*] USB support --->
         <*> xHCI HCD (USB 3.0) support
         <*> EHCI HCD (USB 2.0) support
         < > OHCI HCD (USB 1.0) support
```

### Tarjeta de Red Inalámbrica

Búsqueda rápida: CONFIG_WLAN_VENDOR_REALTEK

```
[*]   Realtek devices
    < >     Realtek 8180/8185/8187SE PCI support
    < >     Realtek 8187 and 8187B USB support
    <M>     Realtek rtlwifi family of devices  --->
        <M>   Realtek RTL8192EE Wireless Network Adapter
```

### Tarjeta de Red Ethernet

Búsqueda rápida: CONFIG_NET_VENDOR_INTEL
```
    [*]   Intel devices
    < >     Intel(R) PRO/100+ support
    < >     Intel(R) PRO/1000 Gigabit Ethernet support
    <*>     Intel(R) PRO/1000 PCI-Express Gigabit Ethernet support
    [*]       Support HW cross-timestamp on PCH devices
```

## OTRAS CONFIGURACIONES

### Tranferencia de archivos Android

Búsqueda rápida: CONFIG_FUSE_FS

```
File systems  ---> 
     <*> FUSE (Filesystem in Userspace) support
```
