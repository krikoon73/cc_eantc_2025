# Test results for Harness1-J-205

## show hostname

```text
Hostname: Harness1-J-205
FQDN:     Harness1-J-205.ns.eantc.de
```

## show ip bgp summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.205, local AS number 65205
Neighbor Status Codes: m - Under maintenance
  Neighbor V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.205, local AS number 65205
Neighbor Status Codes: m - Under maintenance
  Neighbor V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
```

## show bgp evpn route-type imet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
```

## show bgp evpn route-type smet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
```

## show bgp evpn route-type spmsi detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
```

## show bgp evpn arp

```text
```

## show ip route

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

 C        20.45.205.0/24
           directly connected, Ethernet50/3
 C        20.46.205.0/24
           directly connected, Ethernet50/4
 C        20.56.205.0/24
           directly connected, Ethernet49/1
 C        20.201.205.0/24
           directly connected, Ethernet50/1
 C        20.202.205.0/24
           directly connected, Ethernet50/2
 C        100.0.0.205/32
           directly connected, Loopback0

```

## show ip arp

```text
Address         Age (sec)  Hardware Addr   Interface
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

 C        20.45.205.0/24
           directly connected, Ethernet50/3
 C        20.46.205.0/24
           directly connected, Ethernet50/4
 C        20.56.205.0/24
           directly connected, Ethernet49/1
 C        20.201.205.0/24
           directly connected, Ethernet50/1
 C        20.202.205.0/24
           directly connected, Ethernet50/2
 C        100.0.0.205/32
           directly connected, Loopback0


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

## show ip arp vrf all

```text

VRF: default
Address         Age (sec)  Hardware Addr   Interface

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
```

## show vxlan address-table

```text
          Vxlan Mac Address Table
----------------------------------------------------------------------

VLAN  Mac Address     Type      Prt  VTEP             Moves   Last Move
----  -----------     ----      ---  ----             -----   ---------
Total Remote Mac Addresses for this criterion: 0
```

## show vxlan vni

```text
```

## show mac address-table

```text
          Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports      Moves   Last Move
----    -----------       ----        -----      -----   ---------
   1    444c.a873.5ca5    DYNAMIC     Et48       1       1:51:17 ago
   1    5c5a.c773.4ac0    DYNAMIC     Et17       1       1:51:17 ago
  40    246c.8474.8de0    DYNAMIC     Et15       1       1:51:15 ago
  42    00aa.aaaa.aaaa    DYNAMIC     Et16       1       0:22:01 ago
  42    4014.827b.84b0    DYNAMIC     Et16       1       1:51:17 ago
  45    0026.f002.0000    DYNAMIC     Po301      1       1:51:15 ago
  45    00aa.aaaa.aaaa    DYNAMIC     Po301      1       1:50:17 ago
  56    444c.a873.5c75    DYNAMIC     Et48       1       1:50:48 ago
 201    7483.ef0b.a4fb    DYNAMIC     Po100      1       0:41:23 ago
 203    00aa.aaaa.aaaa    DYNAMIC     Po200      1       1:32:13 ago
 203    3838.a621.e82f    DYNAMIC     Po200      1       1:51:15 ago
Total Mac Addresses for this criterion: 11

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
00aa.aaaa.aaaa, VLAN 45, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel301
7483.ef0b.a4fb, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
3838.a621.e82f, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
5c5a.c773.4ac0, VLAN 1, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet17
444c.a873.5c75, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
00aa.aaaa.aaaa, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
4014.827b.84b0, VLAN 42, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet16
444c.a873.5ca5, VLAN 1, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0026.f002.0000, VLAN 45, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel301
246c.8474.8de0, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet15
00aa.aaaa.aaaa, VLAN 42, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet16
```

## show vxlan flood vtep domain local

```text
          VXLAN Flood VTEP Table
--------------------------------------------------------------------------------

VLANS                            Ip Address
-----------------------------   ------------------------------------------------
```

## show vxlan flood vtep domain remote

```text
          VXLAN Flood VTEP Table
--------------------------------------------------------------------------------

VLANS                            Ip Address
-----------------------------   ------------------------------------------------
```

## show bgp evpn domain remote detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
```

## show bgp evpn instance

```text
```

## show interfaces counters rates | nz

```text
Port      Name           Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
```

