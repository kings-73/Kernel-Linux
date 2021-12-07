# Kernel-Linux
Configuración del Kernel Linux en Gentoo

DRIVERS

## Gráficos Integrados Intel HD Graphics

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

## Tarjeta de Red Inalámbrica

Búsqueda rápida: CONFIG_WLAN_VENDOR_REALTEK

```
[*]   Realtek devices
    < >     Realtek 8180/8185/8187SE PCI support
    < >     Realtek 8187 and 8187B USB support
    <M>     Realtek rtlwifi family of devices  --->
        <M>   Realtek RTL8192EE Wireless Network Adapter
```

## Tarjeta de Red Ethernet

Búsqueda rápida: CONFIG_NET_VENDOR_INTEL
```
    [*]   Intel devices
    < >     Intel(R) PRO/100+ support
    < >     Intel(R) PRO/1000 Gigabit Ethernet support
    <*>     Intel(R) PRO/1000 PCI-Express Gigabit Ethernet support
    [*]       Support HW cross-timestamp on PCH devices
```
