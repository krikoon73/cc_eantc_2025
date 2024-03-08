# Test results for Spine1-J-180

## show version

```text
Arista DCS-7280SR-48C6-F
Hardware version: 01.02
Serial number: JPE16200927
Hardware MAC address: 444c.a873.9c0d
System MAC address: 444c.a873.9c0d

Software image version: 4.28.0F
Architecture: i686
Internal build version: 4.28.0F-26924507.4280F
Internal build ID: cc8af7a4-3c5b-4f00-bf78-68394d62ceff
Image format version: 3.0
Image optimization: Sand-4GB

Uptime: 3 days, 7 hours and 37 minutes
Total memory: 8098968 kB
Free memory: 6034116 kB

```

## show interfaces status

```text
Port       Name               Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1        PE21-J2-181        connected    routed   full   10G    10GBASE-SRL                    
Et2        Arista PE22-J2-182 connected    routed   full   10G    10GBASE-SRL                    
Et3        PE23-J2-183        connected    routed   full   10G    10GBASE-SRL                    
Et4        PE24-J2-184        connected    routed   full   10G    10GBASE-SRL                    
Et5                           notconnect   1        full   10G    Not Present                    
Et6                           notconnect   1        full   10G    Not Present                    
Et7                           notconnect   1        full   10G    Not Present                    
Et8        h3c_21             connected    routed   full   10G    10GBASE-SRL                    
Et9        Huawei-34          connected    routed   full   10G    10GBASE-SRL                    
Et10       H3C-18             connected    routed   full   10G    10GBASE-SRL                    
Et11       Nokia              connected    routed   full   10G    10GBASE-SRL                    
Et12       Ciena-3            connected    routed   full   10G    10GBASE-SRL                    
Et13                          notconnect   1        full   10G    Not Present                    
Et14                          notconnect   1        full   10G    Not Present                    
Et15       rbbn-31            connected    routed   full   10G    10GBASE-SRL                    
Et16                          notconnect   1        full   10G    Not Present                    
Et17       Cisco-ASR9K-341    connected    routed   full   10G    10GBASE-SRL                    
Et18       Cisco-NCS5K-345    connected    routed   full   10G    10GBASE-SRL                    
Et19       Cisco-NCS5K-48     connected    routed   full   10G    10GBASE-SRL                    
Et20       Cisco-8K-54        notconnect   routed   full   10G    10GBASE-AR                     
Et21       Cisco-NCS57-45     connected    routed   full   10G    10GBASE-SRL                    
Et22                          notconnect   1        full   10G    Not Present                    
Et23       H3C-26             connected    routed   full   10G    10GBASE-SRL                    
Et24       H3C-27             notconnect   routed   full   10G    10GBASE-SRL                    
Et25       Jnpr-ACX-309       connected    routed   full   10G    10GBASE-SR                     
Et26       Jnpr-ACX314        connected    routed   full   10G    10GBASE-SR                     
Et27       Cisco-VM           connected    routed   full   10G    10GBASE-LR                     
Et28                          notconnect   1        full   10G    Not Present                    
Et29                          notconnect   1        full   10G    Not Present                    
Et30                          notconnect   1        full   10G    Not Present                    
Et31                          notconnect   1        full   10G    Not Present                    
Et32                          notconnect   1        full   10G    Not Present                    
Et33                          notconnect   1        full   10G    Not Present                    
Et34                          notconnect   1        full   10G    Not Present                    
Et35                          notconnect   1        full   10G    Not Present                    
Et36                          notconnect   1        full   10G    Not Present                    
Et37                          notconnect   1        full   10G    Not Present                    
Et38                          notconnect   1        full   10G    Not Present                    
Et39                          notconnect   1        full   10G    Not Present                    
Et40                          notconnect   1        full   10G    Not Present                    
Et41                          notconnect   1        full   10G    Not Present                    
Et42                          notconnect   1        full   10G    Not Present                    
Et43                          notconnect   1        full   10G    Not Present                    
Et44                          notconnect   routed   full   10G    Not Present                    
Et45                          notconnect   1        full   10G    Not Present                    
Et46                          notconnect   1        full   10G    Not Present                    
Et47                          notconnect   1        full   10G    Not Present                    
Et48                          connected    1        full   10G    10GBASE-LR                     
Et49/1     Jnpr-MX304-379     connected    routed   full   100G   100GBASE-LR4                   
Et50/1                        notconnect   1        full   100G   100GBASE-SR4                   
Et51/1                        notconnect   1        full   100G   Not Present                    
Et52/1                        notconnect   1        full   100G   Not Present                    
Et53/1                        notconnect   1        full   100G   Not Present                    
Et54/1     PE41-J2-151        connected    routed   full   40G    40GBASE-SR4                    
Ma1                           connected    routed   a-full a-1G   10/100/1000                    

```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.180, local AS number 64512
Neighbor Status Codes: m - Under maintenance
  Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  100.0.0.3   4 64512             85       260    0    0 01:16:52 Estab   4      4
  100.0.0.18  4 64512            112       291    0    0 01:28:29 Estab   0      0
  100.0.0.21  4 64512            128       277    0    0 01:28:30 Estab   3      3
  100.0.0.26  4 64512            141       260    0    0 01:28:29 Estab   21     21
  100.0.0.31  4 64512            261       269    0    0 01:28:16 Estab   8      8
  100.0.0.34  4 64512            108       291    0    0 01:28:21 Estab   2      2
  100.0.0.161 4 64512            128       271    0    0 01:28:30 Estab   19     19
  100.0.0.181 4 64512           3442      5372    0    0 01:28:30 Estab   5      5
  100.0.0.182 4 64512            128       272    0    0 01:28:30 Estab   4      4
  100.0.0.183 4 64512           3567      5075    0    0 01:28:30 Estab   8      8
  100.0.0.184 4 64512             96       237    0    0 01:09:00 Estab   8      8
  100.0.3.45  4 64512             91       295    0    0 01:28:07 Estab   0      0
  100.0.3.48  4 64512             92       289    0    0 01:28:02 Estab   3      3
  100.0.30.9  4 64512            200       389    0    0 01:28:29 Estab   4      4
  100.0.37.9  4 64512            212       537    0    0 01:28:29 Estab   3      3
```

## show bgp evpn instance

```text
```

## show ip route vrf all

```text

VRF: default
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

 I L2     10.0.0.57/32 [115/90] via 20.161.180.161, Ethernet54/1
 I L2     10.0.0.58/32 [115/80] via 20.161.180.161, Ethernet54/1
 I L2     10.0.0.233/32 [115/90] via 20.161.180.161, Ethernet54/1
 I L2     10.0.0.254/32 [115/100] via 20.161.180.161, Ethernet54/1
 I L2     10.0.1.36/32 [115/60] via 20.161.180.161, Ethernet54/1
 I L2     12.0.0.219/32 [115/100] via 20.161.180.161, Ethernet54/1
 I L2     12.0.0.221/32 [115/120] via 20.161.180.161, Ethernet54/1
 I L2     12.0.0.225/32 [115/110] via 20.161.180.161, Ethernet54/1
 I L2     12.0.0.227/32 [115/110] via 20.161.180.161, Ethernet54/1
 C        20.3.180.0/24 is directly connected, Ethernet12
 C        20.18.180.0/24 is directly connected, Ethernet10
 C        20.21.180.0/24 is directly connected, Ethernet8
 C        20.26.180.0/24 is directly connected, Ethernet23
 C        20.31.180.0/24 is directly connected, Ethernet15
 C        20.34.180.0/24 is directly connected, Ethernet9
 I L2     20.52.1.0/24 [115/110] via 20.161.180.161, Ethernet54/1
 I L2     20.54.2.0/24 [115/100] via 20.161.180.161, Ethernet54/1
 I L2     20.55.2.0/24 [115/80] via 20.161.180.161, Ethernet54/1
 I L2     20.56.2.0/24 [115/100] via 20.161.180.161, Ethernet54/1
 C        20.56.180.0/24 is directly connected, Ethernet11
 I L2     20.57.10.0/24 [115/80] via 20.161.180.161, Ethernet54/1
 I L2     20.57.11.0/24 [115/80] via 20.161.180.161, Ethernet54/1
 I L2     20.57.13.0/24 [115/100] via 20.161.180.161, Ethernet54/1
 I L2     20.57.14.0/24 [115/100] via 20.161.180.161, Ethernet54/1
 I L2     20.57.15.0/24 [115/100] via 20.161.180.161, Ethernet54/1
 C        20.161.180.0/24 is directly connected, Ethernet54/1
 C        20.180.181.0/24 is directly connected, Ethernet1
 C        20.180.182.0/24 is directly connected, Ethernet2
 C        20.180.183.0/24 is directly connected, Ethernet3
 C        20.180.184.0/24 is directly connected, Ethernet4
 I L2     25.29.225.0/24 [115/80] via 20.161.180.161, Ethernet54/1
 I L2     25.36.225.0/24 [115/80] via 20.161.180.161, Ethernet54/1
 I L2     25.58.225.0/24 [115/80] via 20.161.180.161, Ethernet54/1
 I L2     25.59.225.0/24 [115/80] via 20.161.180.161, Ethernet54/1
 I L2     25.102.225.0/24 [115/80] via 20.161.180.161, Ethernet54/1
 I L2     25.107.225.0/24 [115/80] via 20.161.180.161, Ethernet54/1
 I L2     25.110.225.0/24 [115/80] via 20.161.180.161, Ethernet54/1
 I L2     25.116.225.0/24 [115/80] via 20.161.180.161, Ethernet54/1
 I L2     25.136.225.0/24 [115/80] via 20.161.180.161, Ethernet54/1
 I L2     25.138.225.0/24 [115/80] via 20.161.180.161, Ethernet54/1
 I L2     25.142.225.0/24 [115/80] via 20.161.180.161, Ethernet54/1
 I L2     25.144.225.0/24 [115/80] via 20.161.180.161, Ethernet54/1
 I L2     25.152.225.0/24 [115/80] via 20.161.180.161, Ethernet54/1
 I L2     25.153.225.0/24 [115/80] via 20.161.180.161, Ethernet54/1
 C        30.9.180.0/24 is directly connected, Ethernet25
 C        30.14.180.0/24 is directly connected, Ethernet26
 C        30.41.180.0/24 is directly connected, Ethernet17
 C        30.45.180.0/24 is directly connected, Ethernet18
 C        30.48.180.0/24 is directly connected, Ethernet19
 C        30.58.180.0/24 is directly connected, Ethernet21
 C        30.60.180.0/24 is directly connected, Ethernet27
 C        30.79.180.0/24 is directly connected, Ethernet49/1
 I L2     100.0.0.3/32 [115/20] via 20.3.180.3, Ethernet12
 I L2     100.0.0.18/32 [115/10] via 20.18.180.18, Ethernet10
 I L2     100.0.0.21/32 [115/10] via 20.21.180.21, Ethernet8
 I L2     100.0.0.26/32 [115/10] via 20.26.180.26, Ethernet23
 I L2     100.0.0.31/32 [115/10] via 20.31.180.31, Ethernet15
 I L2     100.0.0.34/32 [115/10] via 20.34.180.34, Ethernet9
 I L2     100.0.0.56/32 [115/10] via 20.56.180.56, Ethernet11
 I L2     100.0.0.161/32 [115/20] via 20.161.180.161, Ethernet54/1
 C        100.0.0.180/32 is directly connected, Loopback0
 I L2     100.0.0.181/32 [115/20] via 20.180.181.181, Ethernet1
 I L2     100.0.0.182/32 [115/10] via 20.180.182.182, Ethernet2
 I L2     100.0.0.183/32 [115/10] via 20.180.183.183, Ethernet3
 I L2     100.0.0.184/32 [115/10] via 20.180.184.184, Ethernet4
 I L2     100.0.3.41/32 [115/20] via 30.41.180.41, Ethernet17
 I L2     100.0.3.45/32 [115/20] via 30.45.180.45, Ethernet18
 I L2     100.0.3.48/32 [115/20] via 30.48.180.48, Ethernet19
 I L2     100.0.3.58/32 [115/20] via 30.58.180.58, Ethernet21
 I L2     100.0.3.60/32 [115/20] via 30.60.180.60, Ethernet27
 I L2     100.0.30.9/32 [115/10] via 30.9.180.9, Ethernet25
 I L2     100.0.37.9/32 [115/10] via 30.79.180.79, Ethernet49/1
 I L2     192.168.20.0/23 [115/10] via 20.21.180.21, Ethernet8
                                   via 20.18.180.18, Ethernet10


VRF: mgmt
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

Gateway of last resort:
 S        0.0.0.0/0 [1/0] via 192.168.20.1, Management1

 C        192.168.20.0/23 is directly connected, Management1


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
Et2       Arista PE22  0:05       0.0   0.0%        0       8.1   0.1%        1
Et8       h3c_21       0:05       8.2   0.1%        1       8.1   0.1%        1
Et9       Huawei-34    0:05       0.0   0.0%        0       8.1   0.1%        1
Et10      H3C-18       0:05       4.1   0.0%        0       4.1   0.0%        0
Et11      Nokia        0:05       0.0   0.0%        0       8.2   0.1%        1
Et12      Ciena-3      0:05       1.8   0.0%        0       2.0   0.0%        0
Et19      Cisco-NCS5K  0:05       3.1   0.0%        0       3.9   0.0%        0
Et23      H3C-26       0:05       4.1   0.0%        0      12.2   0.1%        1
Et25      Jnpr-ACX-30  0:05       2.0   0.0%        0       1.0   0.0%        0
Et49/1    Jnpr-MX304-  0:05      32.6   0.0%        3       0.0   0.0%        0
```

## show running-config section router bgp

```text
router bgp 64512
   router-id 100.0.0.180
   distance bgp 20 200 200
   bgp route-reflector preserve-attributes always
   maximum-paths 8 ecmp 16
   bgp listen range 100.0.0.0/8 peer-group EVPN-RR-CLIENTS remote-as 64512
   neighbor EVPN-RR-CLIENTS peer group
   neighbor EVPN-RR-CLIENTS remote-as 64512
   neighbor EVPN-RR-CLIENTS next-hop-unchanged
   neighbor EVPN-RR-CLIENTS update-source Loopback0
   neighbor EVPN-RR-CLIENTS ebgp-multihop 3
   neighbor EVPN-RR-CLIENTS route-reflector-client
   neighbor EVPN-RR-CLIENTS additional-paths send any
   neighbor EVPN-RR-CLIENTS send-community
   neighbor EVPN-RR-CLIENTS maximum-routes 12000
   neighbor EVPN-RR-CLIENTS_VXLAN peer group
   neighbor EVPN-RR-CLIENTS_VXLAN remote-as 64512
   neighbor EVPN-RR-CLIENTS_VXLAN next-hop-unchanged
   neighbor EVPN-RR-CLIENTS_VXLAN update-source Loopback0
   neighbor EVPN-RR-CLIENTS_VXLAN ebgp-multihop 3
   neighbor EVPN-RR-CLIENTS_VXLAN route-reflector-client
   neighbor EVPN-RR-CLIENTS_VXLAN additional-paths send any
   neighbor EVPN-RR-CLIENTS_VXLAN send-community
   neighbor EVPN-RR-CLIENTS_VXLAN maximum-routes 12000
   neighbor 100.0.0.56 remote-as 666
   neighbor 100.0.0.181 peer group EVPN-RR-CLIENTS_VXLAN
   neighbor 100.0.0.183 peer group EVPN-RR-CLIENTS_VXLAN
   neighbor 100.0.0.184 peer group EVPN-RR-CLIENTS_VXLAN
   neighbor 100.0.3.41 remote-as 666
   !
   address-family evpn
      neighbor EVPN-RR-CLIENTS activate
      neighbor EVPN-RR-CLIENTS encapsulation mpls next-hop-self source-interface Loopback0
      neighbor EVPN-RR-CLIENTS_VXLAN activate
      neighbor EVPN-RR-CLIENTS_VXLAN encapsulation vxlan 
      no neighbor 100.0.3.41 activate
      next-hop resolution disabled
   !
   address-family ipv4
      no neighbor EVPN-RR-CLIENTS activate
      no neighbor EVPN-RR-CLIENTS_VXLAN activate
```

## show running-config section interfaces

```text
alias d show interfaces description | grep -v 'not\|down'
```

