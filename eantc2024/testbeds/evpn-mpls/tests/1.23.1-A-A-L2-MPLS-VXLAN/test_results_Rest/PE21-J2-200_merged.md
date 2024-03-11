# Test results for PE21-J2-200

## show version

```text
Arista DCS-7280SR-48C6-F
Hardware version: 01.00
Serial number: JPE16174588
Hardware MAC address: 444c.a873.5c75
System MAC address: 444c.a873.5c75

Software image version: 4.31.2F
Architecture: i686
Internal build version: 4.31.2F-35442146.4312F
Internal build ID: 635a071a-386e-447f-942c-bcc34d9ffd3c
Image format version: 3.0
Image optimization: Sand-4GB

Uptime: 3 days, 7 hours and 37 minutes
Total memory: 8051592 kB
Free memory: 5560456 kB

```

## show interfaces status

```text
Port       Name         Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1        A-PE11-201   connected    routed   full   10G    10GBASE-SRL                    
Et2        A-PE12-202   connected    routed   full   10G    10GBASE-SRL                    
Et3        A-PE13-203   connected    routed   full   10G    10GBASE-SRL                    
Et4        A-PE14-204   connected    routed   full   10G    10GBASE-SRL                    
Et5                     disabled     1        full   10G    10GBASE-LR                     
Et6        PE15-206     connected    routed   full   10G    10GBASE-SRL                    
Et7                     notconnect   1        full   10G    Not Present                    
Et8                     notconnect   1        full   10G    Not Present                    
Et9                     notconnect   1        full   10G    Not Present                    
Et10                    notconnect   1        full   10G    Not Present                    
Et11       Nokia-56     connected    routed   full   10G    10GBASE-SRL                    
Et12       Keysight-103 connected    routed   full   10G    10GBASE-SRL                    
Et13       Cisco-45-N9K notconnect   routed   full   10G    Not Present                    
Et14       Cisco-46-N9K notconnect   routed   full   10G    Not Present                    
Et15       Cisco-40-N9K connected    routed   full   10G    10GBASE-AR                     
Et16       Cisco-42-N9K connected    routed   full   10G    10GBASE-AR                     
Et17                    notconnect   1        full   10G    Not Present                    
Et18                    notconnect   1        full   10G    Not Present                    
Et19                    notconnect   1        full   10G    Not Present                    
Et20                    notconnect   1        full   10G    Not Present                    
Et21                    disabled     1        full   10G    Not Present                    
Et22                    disabled     1        full   10G    Not Present                    
Et23       Cisco-41     connected    routed   full   10G    10GBASE-SRL                    
Et24       JNPR 314     connected    routed   full   10G    10GBASE-SR                     
Et25       H3C-23       notconnect   routed   full   10G    10GBASE-SRL                    
Et26       H3C-22       connected    routed   full   10G    10GBASE-SRL                    
Et27                    disabled     1        full   10G    Not Present                    
Et28                    disabled     1        full   10G    Not Present                    
Et29                    disabled     1        full   10G    Not Present                    
Et30                    disabled     1        full   10G    Not Present                    
Et31                    disabled     1        full   10G    Not Present                    
Et32                    disabled     1        full   10G    Not Present                    
Et33                    disabled     1        full   10G    Not Present                    
Et34                    disabled     1        full   10G    Not Present                    
Et35                    disabled     1        full   10G    Not Present                    
Et36                    disabled     1        full   10G    Not Present                    
Et37                    disabled     1        full   10G    Not Present                    
Et38                    disabled     1        full   10G    Not Present                    
Et39                    disabled     1        full   10G    Not Present                    
Et40                    disabled     1        full   10G    Not Present                    
Et41                    disabled     1        full   10G    Not Present                    
Et42                    disabled     1        full   10G    Not Present                    
Et43                    disabled     1        full   10G    Not Present                    
Et44                    disabled     1        full   10G    Not Present                    
Et45                    disabled     1        full   10G    Not Present                    
Et46                    disabled     1        full   10G    Not Present                    
Et47                    disabled     1        full   10G    Not Present                    
Et48                    disabled     1        full   10G    10GBASE-SRL                    
Et49/1                  disabled     routed   full   100G   Not Present                    
Et50/1                  disabled     1        full   100G   Not Present                    
Et51/1                  notconnect   routed   full   100G   Not Present                    
Et52/1                  notconnect   1        full   100G   Not Present                    
Et53/1                  disabled     1        full   100G   Not Present                    
Et54/1                  disabled     1        full   100G   Not Present                    
Ma1                     connected    routed   a-full a-1G   10/100/1000                    

```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.200, local AS number 65000
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  NOK-41-EVPN              100.0.0.56  4 64512            443       786    0    0 01:59:37 Estab   61     61
  ANET-PE15                100.0.0.206 4 65206           1673      7014    0    0 23:14:03 Estab   3      3
  Cisco-41-EVPN            100.0.3.41  4 64512            399      3768    0    0 02:08:48 Estab   7      7
  H3C-22.EVPN              2000::22    4 65022           2502      7323    0    0 22:15:38 Estab   26     26
  H3C-23.EVPN              2000::23    4 65023           2194      6811    0    0 02:48:24 Active
  CSCO-40.EVPN             2000::40    4 65040           1570      8159    0    0 22:02:34 Estab   15     15
  CSCO-42.EVPN             2000::42    4 65042           1570      8263    0    0 22:01:21 Estab   15     15
  CSCO-45.EVPN             2000::45    4 65045           1510      7753    0    0 01:09:17 Active
  CSCO-46.EVPN             2000::46    4 65045           1523      7736    0    0 01:14:43 Active
  ANET-201.EVPN            2000::201   4 65201           2260      7785    0    0 22:15:40 Estab   23     23
  ANET-202.EVPN            2000::202   4 65202           2311      7843    0    0 22:15:40 Estab   24     24
  ANET-203.EVPN            2000::203   4 65203           3538      6691    0    0 22:15:42 Estab   29     29
  ANET-204.EVPN            2000::204   4 65204           3387      6708    0    0 22:15:40 Estab   31     31
  NOK-56.EVPN              2001::56    4 65056           4190      9544    0    0 02:19:21 Active
```

## show bgp evpn instance

```text
```

## show ip route vrf all

```text

VRF: default
Source Codes:
       C - connected, S - static, K - kernel,
       O - OSPF, IA - OSPF inter area, E1 - OSPF external type 1,
       E2 - OSPF external type 2, N1 - OSPF NSSA external type 1,
       N2 - OSPF NSSA external type2, B - Other BGP Routes,
       B I - iBGP, B E - eBGP, R - RIP, I L1 - IS-IS level 1,
       I L2 - IS-IS level 2, O3 - OSPFv3, A B - BGP Aggregate,
       A O - OSPF Summary, NG - Nexthop Group Static Route,
       V - VXLAN Control Service, M - Martian,
       DH - DHCP client installed default route,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

Gateway of last resort is not set

 C        20.41.200.0/24
           directly connected, Ethernet23
 C        20.56.200.0/24
           directly connected, Ethernet11
 C        20.200.206.0/24
           directly connected, Ethernet6
 B E      100.0.0.56/32 [20/0]
           via 20.56.200.56, Ethernet11
 C        100.0.0.200/32
           directly connected, Loopback0
 B E      100.0.0.206/32 [20/0]
           via 20.200.206.206, Ethernet6
 B E      100.0.3.41/32 [20/0]
           via 20.41.200.41, Ethernet23


VRF: mgmt
Source Codes:
       C - connected, S - static, K - kernel,
       O - OSPF, IA - OSPF inter area, E1 - OSPF external type 1,
       E2 - OSPF external type 2, N1 - OSPF NSSA external type 1,
       N2 - OSPF NSSA external type2, B - Other BGP Routes,
       B I - iBGP, B E - eBGP, R - RIP, I L1 - IS-IS level 1,
       I L2 - IS-IS level 2, O3 - OSPFv3, A B - BGP Aggregate,
       A O - OSPF Summary, NG - Nexthop Group Static Route,
       V - VXLAN Control Service, M - Martian,
       DH - DHCP client installed default route,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

Gateway of last resort:
 S        0.0.0.0/0 [1/0]
           via 192.168.20.1, Management1

 C        192.168.20.0/23
           directly connected, Management1

```

## show interfaces counters rates | nz

```text
Port      Name         Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Et1       A-PE11-201    0:01      0.0   0.0%        0      0.4   0.0%        0
Et2       A-PE12-202    0:01      0.1   0.0%        0      0.3   0.0%        0
Et3       A-PE13-203    0:01      1.3   0.0%        1      0.6   0.0%        0
Et4       A-PE14-204    0:01      0.4   0.0%        0      0.2   0.0%        0
Et15      Cisco-40-N9K  0:01      0.0   0.0%        0      0.7   0.0%        0
Et16      Cisco-42-N9K  0:01      0.0   0.0%        0      0.1   0.0%        0
Et24      JNPR 314      0:01      0.0   0.0%        0      0.0   0.0%        0
Et26      H3C-22        0:01      1.2   0.0%        1      0.6   0.0%        0
Ma1                     0:01      0.0   0.0%        0      3.5   0.4%        0
```

## show running-config section router bgp

```text
router bgp 65000
   router-id 100.0.0.200
   distance bgp 20 200 200
   maximum-paths 8 ecmp 16
   neighbor default send-community
   neighbor EVPN-IPV4-LEAF peer group
   neighbor EVPN-IPV4-LEAF remote-as 65206
   neighbor EVPN-IPV4-LEAF update-source 100.0.0.200
   neighbor EVPN-IPV4-LEAF ebgp-multihop 3
   neighbor EVPN-IPV4-LEAF send-community
   neighbor EVPN-IPV4-LEAF maximum-routes 12000
   neighbor EVPN-LOCAL-PEERS peer group
   neighbor EVPN-LOCAL-PEERS update-source Loopback0
   neighbor EVPN-LOCAL-PEERS ebgp-multihop 5
   neighbor EVPN-LOCAL-PEERS maximum-routes 12000
   neighbor IPV4-LEAF peer group
   neighbor IPV4-LEAF remote-as 65206
   neighbor IPV4-LEAF send-community
   neighbor IPV4-LEAF maximum-routes 12000
   neighbor IPV6-LOCAL-PEERS peer group
   neighbor IPV6-LOCAL-PEERS maximum-routes 12000
   neighbor 20.41.200.41 remote-as 64512
   neighbor 20.41.200.41 description Cisco-41
   neighbor 20.41.200.41 send-community
   neighbor 20.41.200.41 maximum-routes 12000
   neighbor 20.56.200.56 remote-as 64512
   neighbor 20.56.200.56 description NOkia
   neighbor 20.56.200.56 send-community
   neighbor 20.56.200.56 maximum-routes 12000
   neighbor 20.200.206.206 peer group IPV4-LEAF
   neighbor 20.200.206.206 description ANET-PE15
   neighbor 100.0.0.56 remote-as 64512
   neighbor 100.0.0.56 update-source 100.0.0.200
   neighbor 100.0.0.56 description NOK-41-EVPN
   neighbor 100.0.0.56 ebgp-multihop 3
   neighbor 100.0.0.56 send-community
   neighbor 100.0.0.56 maximum-routes 12000
   neighbor 100.0.0.206 peer group EVPN-IPV4-LEAF
   neighbor 100.0.0.206 description ANET-PE15
   neighbor 100.0.3.41 remote-as 64512
   neighbor 100.0.3.41 update-source 100.0.0.200
   neighbor 100.0.3.41 description Cisco-41-EVPN
   neighbor 100.0.3.41 ebgp-multihop 3
   neighbor 100.0.3.41 send-community
   neighbor 100.0.3.41 maximum-routes 12000
   neighbor 2000::22 peer group EVPN-LOCAL-PEERS
   neighbor 2000::22 remote-as 65022
   neighbor 2000::22 description H3C-22.EVPN
   neighbor 2000::23 peer group EVPN-LOCAL-PEERS
   neighbor 2000::23 remote-as 65023
   neighbor 2000::23 description H3C-23.EVPN
   neighbor 2000::40 peer group EVPN-LOCAL-PEERS
   neighbor 2000::40 remote-as 65040
   neighbor 2000::40 description CSCO-40.EVPN
   neighbor 2000::42 peer group EVPN-LOCAL-PEERS
   neighbor 2000::42 remote-as 65042
   neighbor 2000::42 description CSCO-42.EVPN
   neighbor 2000::45 peer group EVPN-LOCAL-PEERS
   neighbor 2000::45 remote-as 65045
   neighbor 2000::45 description CSCO-45.EVPN
   neighbor 2000::46 peer group EVPN-LOCAL-PEERS
   neighbor 2000::46 remote-as 65045
   neighbor 2000::46 description CSCO-46.EVPN
   neighbor 2000::201 peer group EVPN-LOCAL-PEERS
   neighbor 2000::201 remote-as 65201
   neighbor 2000::201 description ANET-201.EVPN
   neighbor 2000::202 peer group EVPN-LOCAL-PEERS
   neighbor 2000::202 remote-as 65202
   neighbor 2000::202 description ANET-202.EVPN
   neighbor 2000::203 peer group EVPN-LOCAL-PEERS
   neighbor 2000::203 remote-as 65203
   neighbor 2000::203 description ANET-203.EVPN
   neighbor 2000::204 peer group EVPN-LOCAL-PEERS
   neighbor 2000::204 remote-as 65204
   neighbor 2000::204 description ANET-204.EVPN
   neighbor 2001::56 peer group EVPN-LOCAL-PEERS
   neighbor 2001::56 remote-as 65056
   neighbor 2001::56 description NOK-56.EVPN
   redistribute connected
   neighbor interface Et1-4,11-16,23-26 peer-group IPV6-LOCAL-PEERS peer-filter IPV6-LEAFS
   !
   address-family evpn
      neighbor EVPN-IPV4-LEAF activate
      neighbor EVPN-LOCAL-PEERS activate
      neighbor 100.0.0.56 activate
      neighbor 100.0.3.41 activate
   !
   address-family ipv4
      no neighbor EVPN-IPV4-LEAF activate
      neighbor IPV4-LEAF activate
      neighbor 20.41.200.41 activate
      neighbor 20.56.200.56 activate
      no neighbor 100.0.0.56 activate
      no neighbor 100.0.3.41 activate
   !
   address-family ipv6
      neighbor IPV6-LOCAL-PEERS activate
```

## show running-config section interfaces

```text
```

