# Jarkom-Modul-4-I10-2023

Praktikum Jaringan Komputer Modul 4 I10
Computer Network Practicum 4th Module I10

| Name                        | NRP        |
|-----------------------------|------------|
|Riski Ilyas                  | 5025211189 |
|Vija Wildan Gita Prabawa     | 5025211261 |

## A. Topology

### Cisco Packet Tracer (CPT)
![TopoCPT](https://media.discordapp.net/attachments/919468862725046322/1180431244379557948/image.png?ex=657d6544&is=656af044&hm=938631356e54fe3256d0ba3bb1a4f86df6f7ed0dd1b8b9d74e8ff2b966e5735a&=&format=webp&quality=lossless&width=1375&height=662)

## B. VLSM for CPT

According to the topology, we found a total of 21 subnet. 

![VLSMCPT](https://media.discordapp.net/attachments/919468862725046322/1180437763171045388/image.png?ex=657d6b56&is=656af656&hm=8f430bbd3ef7abfda042435cf4f18bc828718ef95844ef3fd6b921d06813e2d6&=&format=webp&quality=lossless&width=1375&height=662)


## C. CIDR With GNS3
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

#### B. CLIENTS & SERVERS
- 1. ROYALCAPITAL
```
auto eth0
iface eth0 inet static
      address 192.234.64.2
      netmask 255.255.255.128
      gateway 192.234.64.1
```

- 2. WILLEREGION
```
auto eth0
iface eth0 inet static
      address 192.234.64.65
      netmask 255.255.255.128
      gateway 192.234.64.1
```

- 3. LAKEKORIDOR
```
auto eth0
iface eth0 inet static
      address 192.234.224.2
      netmask 255.255.255.224
      gateway 192.234.224.1
```

- 4. APPETITREGION
```
auto eth0
iface eth0 inet static
      address 192.234.200.2
      netmask 255.255.252.0
      gateway 192.234.200.1
```

- 5. LAUBHILLS
```
auto eth0
iface eth0 inet static
      address 192.234.202.117
      netmask 255.255.252.0
      gateway 192.234.200.1
```

- 6. ROHRROAD
```
auto eth0
iface eth0 inet static
      address 192.234.208.2
      netmask 255.255.252.0
      gateway 192.234.208.1
```

- 7. SCHWERMOUNTAINS
```
auto eth0
iface eth0 inet static
      address 192.234.220.2
      netmask 255.255.255.248
      gateway 192.234.220.1
```

- 8. RICHTER
```
auto eth0
iface eth0 inet static
      address 192.233.96.2
      netmask 255.255.255.248
      gateway 192.233.96.1
```

- 9. REVOLTS
```
auto eth0
iface eth0 inet static
      address 192.233.96.3
      netmask 255.255.255.248
      gateway 192.233.96.1
```

- 10. STARK
```
auto eth0
iface eth0 inet static
      address 192.233.112.2
      netmask 255.255.255.252
      gateway 192.233.112.1
```

- 11. TURKREION
```
auto eth0
iface eth0 inet static
      address 192.233.64.2
      netmask 255.255.252.0
      gateway 192.233.64.1
```

- 12. GROBEFOREST
```
auto eth0
iface eth0 inet static
      address 192.233.72.2
      netmask 255.255.255.0
      gateway 192.233.72.1
```

- 13. GRANZCHANNEL
```
auto eth0
iface eth0 inet static
      address 192.233.16.2
      netmask 255.255.255.0
      gateway 192.233.16.1
```

- 14. BREDREGION
```
auto eth0
iface eth0 inet static
      address 192.233.4.3
      netmask 255.255.255.224
      gateway 192.233.4.1
```

- 15. SEIN
```
auto eth0
iface eth0 inet static
      address 192.233.0.2
      netmask 255.255.254.0
      gateway 192.233.0.1
```

- 16. RIEGELCANYON
```
auto eth0
iface eth0 inet static
      address 192.233.0.3
      netmask 255.255.254.0
      gateway 192.233.0.1
```
