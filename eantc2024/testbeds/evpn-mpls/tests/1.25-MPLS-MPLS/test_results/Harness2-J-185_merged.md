# Test results for Harness2-J-185

## show version

```text
Arista DCS-7280SR-48C6-F
Hardware version: 10.01
Serial number: JPE17131945
Hardware MAC address: 2899.3a06.b1fd
System MAC address: 2899.3a06.b1fd

Software image version: 4.27.3F
Architecture: x86_64
Internal build version: 4.27.3F-26391011.4273F
Internal build ID: 037a4a3f-ba8d-42a8-8876-433ce8a83555
Image format version: 2.0
Image optimization: DEFAULT

Uptime: 1 day, 6 hours and 36 minutes
Total memory: 8098968 kB
Free memory: 5591188 kB

```

## show interfaces status

```text
Port       Name              Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1        PE21-J2-181       notconnect   1        full   10G    10GBASE-SRL                    
Et2                          disabled     trunk    full   10G    10GBASE-SRL                    
Et3        PE23-J2-183       errdisabled  in Po68  full   10G    10GBASE-SRL                    
Et4        PE24-J2-184       connected    trunk    full   10G    10GBASE-SRL                    
Et5                          notconnect   1        full   10G    Not Present                    
Et6                          notconnect   1        full   10G    Not Present                    
Et7                          notconnect   1        full   10G    Not Present                    
Et8                          notconnect   1        full   10G    Not Present                    
Et9                          notconnect   1        full   10G    Not Present                    
Et10                         notconnect   1        full   10G    Not Present                    
Et11       Huawei-34         connected    trunk    full   10G    10GBASE-SRL                    
Et12       CIENA             connected    trunk    full   10G    10GBASE-SRL                    
Et13                         connected    in Po21  full   10G    10GBASE-SRL                    
Et14       h3c_21_CR16010E-F connected    trunk    full   10G    10GBASE-SRL                    
Et15       Ribbon            connected    in Po31  full   10G    10GBASE-SRL                    
Et16                         notconnect   1        full   10G    Not Present                    
Et17                         notconnect   1        full   10G    10GBASE-SRL                    
Et18       Cisco-45          connected    in Po151 full   10G    10GBASE-SRL                    
Et19                         connected    in Po151 full   10G    10GBASE-SRL                    
Et20                         disabled     in Po300 full   10G    10GBASE-AR                     
Et21       Nokia 7750-SR1    connected    trunk    full   10G    10GBASE-SRL                    
Et22                         notconnect   1        full   10G    Not Present                    
Et23                         notconnect   1        full   10G    Not Present                    
Et24                         notconnect   1        full   10G    Not Present                    
Et25       Juniper 33        connected    in Po33  full   10G    10GBASE-SR                     
Et26                         notconnect   1        full   10G    Not Present                    
Et27       h3c_26_S12500R-2L connected    in Po26  full   10G    10GBASE-SRL                    
Et28                         notconnect   in Po26  full   10G    10GBASE-SRL                    
Et29                         notconnect   1        full   10G    Not Present                    
Et30                         notconnect   1        full   10G    Not Present                    
Et31                         disabled     trunk    full   10G    10GBASE-SRL                    
Et32                         disabled     trunk    full   10G    10GBASE-SRL                    
Et33                         notconnect   1        full   10G    Not Present                    
Et34                         notconnect   1        full   10G    Not Present                    
Et35                         notconnect   1        full   10G    Not Present                    
Et36                         notconnect   1        full   10G    Not Present                    
Et37                         notconnect   1        full   10G    Not Present                    
Et38                         notconnect   1        full   10G    Not Present                    
Et39                         notconnect   1        full   10G    Not Present                    
Et40                         notconnect   1        full   10G    Not Present                    
Et41                         notconnect   1        full   10G    Not Present                    
Et42                         notconnect   1        full   10G    Not Present                    
Et43                         notconnect   1        full   10G    10GBASE-SR                     
Et44                         notconnect   1        full   10G    Not Present                    
Et45       Juniper-379       connected    in Po32  full   10G    10GBASE-LR                     
Et46                         notconnect   in Po300 full   10G    Not Present                    
Et47       IXIA Port         connected    trunk    full   10G    10GBASE-SRL                    
Et48                         connected    1        full   10G    10GBASE-LR                     
Et49/1                       notconnect   1        full   10G    40GBASE-PSM4                   
Et49/2                       notconnect   1        full   10G    40GBASE-PSM4                   
Et49/3                       notconnect   1        full   10G    40GBASE-PSM4                   
Et49/4                       notconnect   1        full   10G    40GBASE-PSM4                   
Et50/1                       notconnect   1        full   100G   100GBASE-SR4                   
Et51/1                       notconnect   1        full   100G   Not Present                    
Et52/1                       notconnect   1        full   100G   Not Present                    
Et53/1                       notconnect   1        full   100G   Not Present                    
Et54/1                       notconnect   1        full   100G   Not Present                    
Ma1                          connected    routed   a-full a-1G   10/100/1000                    
Po21                         notconnect   trunk    full   unconf N/A                            
Po26                         connected    trunk    full   10G    N/A                            
Po31                         connected    trunk    full   10G    N/A                            
Po32       Juniper 32        connected    trunk    full   10G    N/A                            
Po33       Juniper 33        connected    trunk    full   10G    N/A                            
Po68       Arista 68         disabled     trunk    full   unconf N/A                            
Po100                        notconnect   trunk    full   unconf N/A                            
Po151      Cisco 151         connected    trunk    full   20G    N/A                            
Po194                        notconnect   trunk    full   unconf N/A                            
Po200                        notconnect   1        full   unconf N/A                            
Po300      Ciena-Ribbon-Jnpr notconnect   trunk    full   unconf N/A                            
Po301                        notconnect   trunk    full   unconf N/A                            
Po302                        notconnect   1        full   unconf N/A                            
Po419                        disabled     trunk    full   unconf N/A                            

```

## show bgp evpn summary

```text
BGP is disabled for VRF default
```

## show bgp evpn instance

```text
```

## show ip route vrf tenant-a

```text

VRF: tenant-a
Codes: C - connected, S - static, K - kernel, 
       O - OSPF, IA - OSPF inter area, E1 - OSPF external type 1,
       E2 - OSPF external type 2, N1 - OSPF NSSA external type 1,
       N2 - OSPF NSSA external type2, B - Other BGP Routes,
       B I - iBGP, B E - eBGP, R - RIP, I L1 - IS-IS level 1,
       I L2 - IS-IS level 2, O3 - OSPFv3, A B - BGP Aggregate,
       A O - OSPF Summary, NG - Nexthop Group Static Route,
       V - VXLAN Control Service, M - Martian,
       DH - DHCP client installed default route,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route

Gateway of last resort is not set


! IP routing not enabled
```

## show interfaces counters rates | nz

```text
Port      Name        Intvl   In Mbps      %  In Kpps  Out Mbps      % Out Kpps
Et4       PE24-J2-184  0:05       2.7   0.0%        0       2.7   0.0%        0
Et12      CIENA        0:05       0.9   0.0%        0       0.9   0.0%        0
Et14      h3c_21_CR16  0:05       0.9   0.0%        0       0.9   0.0%        0
Et15      Ribbon       0:05       0.9   0.0%        0       0.9   0.0%        0
Et25      Juniper 33   0:05       0.0   0.0%        0       0.0   0.0%        0
Et47      IXIA Port    0:05       5.3   0.1%        0       5.3   0.1%        0
Ma1                    0:05       0.0   0.0%        0       0.1   0.0%        0
Po31                   0:05       0.9   0.0%        0       0.9   0.0%        0
Po32      Juniper 32   0:05       0.0   0.0%        0       0.0   0.0%        0
Po33      Juniper 33   0:05       0.0   0.0%        0       0.0   0.0%        0
Po68      Arista 68    0:05       0.0      -        0       0.0      -        0
Po151     Cisco 151    0:05       0.0   0.0%        0       0.0   0.0%        0
```

## show running-config section router bgp

```text
```

## show running-config section interfaces

```text
```

## show bgp vpn-ipv4 detail

```text
BGP is disabled for VRF default
```

## show patch panel detail

```text
PW Fault Legend:
   ET-IN - Ethernet receive fault
   ET-OUT - Ethernet transmit fault
   TUN-IN - Tunnel receive fault
   TUN-OUT - Tunnel transmit fault
   NF - Pseudowire not forwarding (other reason)

```

