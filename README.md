![image](https://github.com/vijawildan/Jarkom-Modul-4-I10-2023/assets/115712593/aec2d05c-2081-4613-94b5-bd081bcefd84)# Jarkom-Modul-4-I10-2023

Praktikum Jaringan Komputer Modul 4 I10
Computer Network Practicum 4th Module I10

| Name                        | NRP        |
|-----------------------------|------------|
|Riski Ilyas                  | 5025211189 |
|Vija Wildan Gita Prabawa     | 5025211261 |

## A. Topology

### Cisco Packet Tracer (CPT)
![TopoCPT](https://media.discordapp.net/attachments/919468862725046322/1180431244379557948/image.png?ex=657d6544&is=656af044&hm=938631356e54fe3256d0ba3bb1a4f86df6f7ed0dd1b8b9d74e8ff2b966e5735a&=&format=webp&quality=lossless&width=1375&height=662)
![WhatsApp Image 2023-12-02 at 21 01 35](https://github.com/vijawildan/Jarkom-Modul-4-I10-2023/assets/71499142/10d450cd-5891-49d2-a88d-75a334125c26)

## B. VLSM for CPT

According to the topology, we found a total of 21 subnet. 

![VLSMCPT](https://media.discordapp.net/attachments/919468862725046322/1180437763171045388/image.png?ex=657d6b56&is=656af656&hm=8f430bbd3ef7abfda042435cf4f18bc828718ef95844ef3fd6b921d06813e2d6&=&format=webp&quality=lossless&width=1375&height=662)

### 1. Routes
![image](https://github.com/vijawildan/Jarkom-Modul-4-I10-2023/assets/71499142/d45e18b6-1972-4920-98b4-361bb4fc329f)

### 2. Tree
![Untitled Diagram drawio](https://github.com/vijawildan/Jarkom-Modul-4-I10-2023/assets/71499142/28b6f222-febb-4c67-ba3a-14236b769898)

### 3. Subnetting
![image](https://github.com/vijawildan/Jarkom-Modul-4-I10-2023/assets/71499142/762e0242-54ef-435c-9625-261a9fc3aaf6)

## C. CIDR With GNS3
![GNS3Topo](https://media.discordapp.net/attachments/919468862725046322/1180431662782349362/image.png?ex=657d65a7&is=656af0a7&hm=d4e78823519d3efce7972aad5552d5f067094a05deddb0565c9262c59a960932&=&format=webp&quality=lossless&width=1005&height=661)
### 1. CIDR SUBNETTING
![CPTCIDR1](https://media.discordapp.net/attachments/919468862725046322/1180457184073621524/image.png?ex=657d7d6c&is=656b086c&hm=dce19e55ad86232a7bb6569e9419be8b709a273603de80013240a5a2a350a2ee&=&format=webp&quality=lossless&width=1375&height=662  )
![CPTCIDR2](https://cdn.discordapp.com/attachments/919468862725046322/1180457202088157204/image.png?ex=657d7d70&is=656b0870&hm=3079807e707650914953d3074c1736e109bcdcc8c720e475138a693922535fd6&)
![CPTCIDR3](https://cdn.discordapp.com/attachments/919468862725046322/1180457219523874837/image.png?ex=657d7d74&is=656b0874&hm=52438e967d36bf945116d9f0685a96a7fcea4e743b6e190fed372274e425147a&)
![CPTCIDR4](https://cdn.discordapp.com/attachments/919468862725046322/1180457235923611718/image.png?ex=657d7d78&is=656b0878&hm=5c3c5cbf187fac9a591c5f44e69d91c7c80b414e9e629686614a092c46e1094e&    )
![CPTCIDR5](https://cdn.discordapp.com/attachments/919468862725046322/1180457247319539753/image.png?ex=657d7d7b&is=656b087b&hm=e3d3edce2486f15a421257c7f7a467e2a2a953e23fe7b3229e8648ac470f8f7f&)
![CPTCIDR6](https://cdn.discordapp.com/attachments/919468862725046322/1180457267473166366/image.png?ex=657d7d80&is=656b0880&hm=2c0cd963ebc916ec0e5b196e1e723952c32398fbf9fc1675628e0f0ba89c4b3a&)
![CPTCIDR7](https://media.discordapp.net/attachments/919468862725046322/1180457287781978112/image.png?ex=657d7d85&is=656b0885&hm=c1c3619512a2aef0cfd8dae69966d79731f9ba4de1ab66f8e24265dd4b7af8b0&=&format=webp&quality=lossless&width=1375&height=662)
![CPTCIDR8](https://media.discordapp.net/attachments/919468862725046322/1180457304928296990/image.png?ex=657d7d89&is=656b0889&hm=060b9964c224e78c18210e9ae09c995b129785cc8e88e46c5a75b9e2915f50cd&=&format=webp&quality=lossless&width=1375&height=662)
![image](https://github.com/vijawildan/Jarkom-Modul-4-I10-2023/assets/71499142/2eb1e9c3-6fd7-4883-a21d-c3295a27d348)
### 2. CIDR TREE
![CIDRTREE](https://cdn.discordapp.com/attachments/919468862725046322/1181949174053339216/image.png?ex=6582eaf2&is=657075f2&hm=a3b575a254ddc3ca58cb097ffeda49b953521b31c18dc95b375f862199175644&)

### 3. CIDR ROUTING
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

#### C. ROUTING
- 1. AURA
```
route add -net 192.234.64.0 netmask 255.255.255.128 gw 192.234.0.2          #A14
route add -net 192.234.224.0 netmask 255.255.255.224 gw 192.234.128.2           #A15
route add -net 192.234.200.0 netmask 255.255.252.0 gw 192.234.128.2         #A21
route add -net 192.234.208.0 netmask 255.255.252.0 gw 192.234.128.2         #A17
route add -net 192.234.240.0 netmask 255.255.255.252 gw 192.234.128.2         #A16
route add -net 192.234.192.0 netmask 255.255.255.252 gw 192.234.128.2         #A20
route add -net 192.234.216.0 netmask 255.255.255.252 gw 192.234.128.2         #A18
route add -net 192.234.220.0 netmask 255.255.255.248 gw 192.234.128.2         #A19
route add -net 192.233.0.0 netmask 255.255.254.0 gw 192.233.128.2         #A1
route add -net 192.233.4.0 netmask 255.255.255.224 gw 192.233.128.2         #A2
route add -net 192.233.8.0 netmask 255.255.255.252 gw 192.233.128.2         #A3
route add -net 192.233.16.0 netmask 255.255.255.0 gw 192.233.128.2         #A4
route add -net 192.233.32.0 netmask 255.255.255.252 gw 192.233.128.2         #A5
route add -net 192.233.96.0 netmask 255.255.255.248 gw 192.233.128.2         #A6
route add -net 192.233.112.0 netmask 255.255.255.252 gw 192.233.128.2         #A7
route add -net 192.233.80.0 netmask 255.255.255.252 gw 192.233.128.2         #A8
route add -net 192.233.64.0 netmask 255.255.255.248 gw 192.233.128.2         #A9
route add -net 192.233.72.0 netmask 255.255.255.0 gw 192.233.128.2         #A10
```

- 2. FRIEREN
```
route add -net 192.234.200.0 netmask 255.255.252.0 gw 192.234.240.2         #A21
route add -net 192.234.208.0 netmask 255.255.252.0 gw 192.234.240.2         #A17
route add -net 192.234.192.0 netmask 255.255.255.252 gw 192.234.240.2         #A20
route add -net 192.234.216.0 netmask 255.255.255.252 gw 192.234.240.2         #A18
route add -net 192.234.220.0 netmask 255.255.255.248 gw 192.234.240.2         #A19
```

- 3. FLAMME
```
route add -net 192.234.200.0 netmask 255.255.252.0 gw 192.234.192.2         #A21
route add -net 192.234.220.0 netmask 255.255.255.248 gw 192.234.216.2         #A19
```

- 4. EISEN
```
route add -net 192.233.0.0 netmask 255.255.254.0 gw 192.233.32.2         #A1
route add -net 192.233.4.0 netmask 255.255.255.224 gw 192.233.32.2         #A2
route add -net 192.233.8.0 netmask 255.255.255.252 gw 192.233.32.2         #A3
route add -net 192.233.16.0 netmask 255.255.255.0 gw 192.233.32.2         #A4
route add -net 192.233.64.0 netmask 255.255.255.248 gw 192.233.80.2         #A9
route add -net 192.233.72.0 netmask 255.255.255.0 gw 192.233.80.2         #A10
```

- 5. LINIE
```
route add -net 192.233.0.0 netmask 255.255.254.0 gw 192.233.8.2         #A1
route add -net 192.233.4.0 netmask 255.255.255.224 gw 192.233.8.2         #A2
```

- 6. LAWINE
```
route add -net 192.233.0.0 netmask 255.255.254.0 gw 192.233.4.2         #A1
```

**Iptables Aura**
```
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.233.0.0/15
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.234.0.0/15
```

**Setting resolv.conf each Nodes**
```
echo nameserver 192.168.122.1 > /etc/resolv.conf
```
