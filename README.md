# Jarkom-Modul-4-I10-2023


## A. CIDR With GNS3
### 1. CIDR SUBNETTING
### 2. CIDR ROUTING
#### A. ROUTER
- 1. AURA
```
auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
      address 192.233.128.1
      netmask 255.255.255.252

auto eth2
iface eth2 inet static
      address 192.234.0.1
      netmask 255.255.255.252

auto eth3
iface eth3 inet static
      address 192.234.128.1
      netmask 255.255.255.252
```

- 2. FRIEREN
```
auto eth0
iface eth0 inet static
      address 192.234.128.2
      netmask 255.255.255.252
      gateway 192.234.128.1

auto eth1
iface eth1 inet static
      address 192.234.224.1
      netmask 255.255.255.224

auto eth2
iface eth2 inet static
      address 192.234.240.1
      netmask 255.255.255.252
```

- 3. DENKEN
```
auto eth0
iface eth0 inet static
      address 192.234.0.2
      netmask 255.255.255.252
      gateway 192.234.0.1

auto eth1
iface eth1 inet static
      address 192.234.64.1
      netmask 255.255.255.128
```

- 4. FLAMME
```
auto eth0
iface eth0 inet static
      address 192.234.240.2
      netmask 255.255.255.252
      gateway 192.234.240.1

auto eth1
iface eth1 inet static
      address 192.234.192.1
      netmask 255.255.255.252

auto eth2
iface eth2 inet static
      address 192.234.208.1
      netmask 255.255.252.0

auto eth3
iface eth3 inet static
      address 192.234.220.1
      netmask 255.255.255.248
```

- 5. FERN
```
auto eth0
iface eth0 inet static
      address 192.234.192.2
      netmask 255.255.255.252
      gateway 192.234.192.1

auto eth1
iface eth1 inet static
      address 192.234.200.1
      netmask 255.255.252.0
```

- 6. HIMMEL
```
auto eth0
iface eth0 inet static
      address 192.234.216.2
      netmask 255.255.255.252
      gateway 192.234.216.1

auto eth1
iface eth1 inet static
      address 192.234.220.1
      netmask 255.255.255.248
```

- 7. EISEN
```
auto eth0
iface eth0 inet static
      address 192.233.128.2
      netmask 255.255.255.252
      gateway 192.233.128.1

auto eth1
iface eth1 inet static
      address 192.233.112.1
      netmask 255.255.255.252

auto eth2
iface eth2 inet static
      address 192.233.80.1
      netmask 255.255.255.252

auto eth3
iface eth3 inet static
      address 192.233.32.1
      netmask 255.255.255.252

auto eth4
iface eth4 inet static
      address 192.233.96.1
      netmask 255.255.255.248
```

- 8. LUGNER
```
auto eth0
iface eth0 inet static
      address 192.233.80.2
      netmask 255.255.255.252
      gateway 192.233.80.1

auto eth1
iface eth1 inet static
      address 192.233.64.1
      netmask 255.255.252.0

auto eth2
iface eth2 inet static
      address 192.233.72.1
      netmask 255.255.255.0
```

- 9. LINIE
```
auto eth0
iface eth0 inet static
      address 192.233.32.2
      netmask 255.255.255.252
      gateway 192.233.32.1

auto eth1
iface eth1 inet static
      address 192.233.16.1
      netmask 255.255.255.0

auto eth2
iface eth2 inet static
      address 192.233.8.1
      netmask 255.255.255.252
```

- 10. LAWINE
```
auto eth0
iface eth0 inet static
      address 192.233.8.2
      netmask 255.255.255.252
      gateway 192.233.8.1

auto eth1
iface eth1 inet static
      address 192.233.4.1
      netmask 255.255.255.224
```

- 11. HEITER
```
auto eth0
iface eth0 inet static
      address 192.233.4.2
      netmask 255.255.255.224
      address 192.233.4.1

auto eth1
iface eth1 inet static
      address 192.233.0.1
      netmask 255.255.254.0
```
