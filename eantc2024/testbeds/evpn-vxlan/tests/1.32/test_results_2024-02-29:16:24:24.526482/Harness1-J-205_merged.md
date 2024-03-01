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
  Neighbor   V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  100.0.0.22 4 65205           7851     35031    0    0    1d05h Active
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
192.168.21.50     0:01:29  a84f.b1a5.5221  Management1
192.168.21.59     0:03:25  6607.f5d1.ae16  Management1
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
  22    0020.1000.0002    DYNAMIC     Po300      1       0:02:28 ago
  22    0020.1000.0003    DYNAMIC     Po300      1       0:02:28 ago
  22    0020.1000.0004    DYNAMIC     Po300      1       0:02:28 ago
  22    0020.3000.0001    DYNAMIC     Po300      1       0:02:49 ago
  22    0020.3000.0002    DYNAMIC     Po300      1       0:02:49 ago
  22    0020.3000.0003    DYNAMIC     Po300      1       0:02:49 ago
  22    0020.3000.0004    DYNAMIC     Po300      1       0:02:49 ago
  22    0022.0000.0001    DYNAMIC     Et25       1       0:23:39 ago
  22    0022.0000.0002    DYNAMIC     Et25       1       0:23:39 ago
  22    0022.0000.0003    DYNAMIC     Et25       1       0:02:49 ago
  22    0022.0000.0004    DYNAMIC     Et25       1       0:02:49 ago
  22    0022.0000.0005    DYNAMIC     Et25       1       0:23:32 ago
  22    0040.0100.0001    DYNAMIC     Po300      1       0:05:30 ago
  22    0040.0100.0002    DYNAMIC     Po300      1       0:05:28 ago
  22    0056.0000.0001    DYNAMIC     Po300      1       0:02:49 ago
  22    0056.0000.0002    DYNAMIC     Po300      1       0:02:49 ago
  22    0056.0000.0003    DYNAMIC     Po300      1       0:02:49 ago
  22    0056.0000.0004    DYNAMIC     Po300      1       0:02:49 ago
  22    00aa.aaaa.aaaa    DYNAMIC     Po300      1       1 day, 0:08:43 ago
  40    0022.0000.0001    DYNAMIC     Et15       1       0:11:10 ago
  40    0022.0000.0002    DYNAMIC     Et15       1       0:07:51 ago
  40    0040.0100.0001    DYNAMIC     Et25       1       0:07:51 ago
  40    0040.0100.0002    DYNAMIC     Et25       1       0:07:51 ago
  40    0040.0100.0003    DYNAMIC     Et25       1       0:10:02 ago
  40    0056.0000.0001    DYNAMIC     Et15       1       0:02:49 ago
  40    0056.0000.0002    DYNAMIC     Et15       1       0:02:49 ago
  40    00aa.aaaa.aaaa    DYNAMIC     Et15       1       23:54:32 ago
  40    246c.8474.8ddb    DYNAMIC     Et15       1       0:07:51 ago
  40    246c.8474.8de0    DYNAMIC     Et15       1       23:55:09 ago
  56    0022.0000.0001    DYNAMIC     Et21       1       0:23:39 ago
  56    0022.0000.0002    DYNAMIC     Et21       1       0:23:39 ago
  56    0022.0000.0003    DYNAMIC     Et21       1       0:02:49 ago
  56    0022.0000.0004    DYNAMIC     Et21       1       0:02:49 ago
  56    0056.0000.0001    DYNAMIC     Et25       1       0:02:57 ago
  56    0056.0000.0002    DYNAMIC     Et25       1       0:02:57 ago
  56    0056.0000.0003    DYNAMIC     Et25       1       0:02:57 ago
  56    0056.0000.0004    DYNAMIC     Et25       1       0:02:57 ago
  56    0056.0000.0005    DYNAMIC     Et25       1       0:22:58 ago
  56    00aa.aaaa.aaaa    DYNAMIC     Et21       1       0:02:57 ago
 201    0020.1000.0001    DYNAMIC     Et25       1       0:02:49 ago
 201    0020.1000.0002    DYNAMIC     Et25       1       0:02:49 ago
 201    0020.1000.0003    DYNAMIC     Et25       1       0:02:49 ago
 201    0020.1000.0004    DYNAMIC     Et25       1       0:02:49 ago
 201    0020.1000.0005    DYNAMIC     Et25       1       0:02:28 ago
 201    0022.0000.0002    DYNAMIC     Po100      1       0:02:47 ago
 201    0022.0000.0003    DYNAMIC     Po100      1       0:02:47 ago
 201    0022.0000.0004    DYNAMIC     Po100      1       0:02:49 ago
 201    2cdd.e90b.2283    DYNAMIC     Po100      1       0:02:26 ago
 201    2cdd.e90b.25b7    DYNAMIC     Po100      1       0:00:29 ago
 203    0020.3000.0001    DYNAMIC     Et25       1       0:02:49 ago
 203    0020.3000.0002    DYNAMIC     Et25       1       0:02:49 ago
 203    0020.3000.0003    DYNAMIC     Et25       1       0:02:49 ago
 203    0020.3000.0004    DYNAMIC     Et25       1       0:02:49 ago
 203    0020.3000.0005    DYNAMIC     Et25       1       0:02:28 ago
 203    0022.0000.0001    DYNAMIC     Po200      1       0:23:39 ago
 203    0022.0000.0002    DYNAMIC     Po200      1       0:23:39 ago
 203    0022.0000.0003    DYNAMIC     Po200      1       0:02:49 ago
 203    0022.0000.0004    DYNAMIC     Po200      1       0:02:49 ago
 203    0056.0000.0001    DYNAMIC     Po200      1       0:02:49 ago
 203    0056.0000.0002    DYNAMIC     Po200      1       0:02:49 ago
 203    0056.0000.0003    DYNAMIC     Po200      1       0:02:49 ago
 203    0056.0000.0004    DYNAMIC     Po200      1       0:02:49 ago
 203    00aa.aaaa.aaaa    DYNAMIC     Po200      1       1 day, 1:42:30 ago
 203    3838.a621.e82f    DYNAMIC     Po200      1       0:02:28 ago
Total Mac Addresses for this criterion: 64

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
0022.0000.0002, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet15
0022.0000.0002, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet21
2cdd.e90b.2283, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0056.0000.0004, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0040.0100.0001, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel300
0056.0000.0002, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0020.1000.0002, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0022.0000.0003, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0022.0000.0001, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0022.0000.0004, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0056.0000.0003, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0020.1000.0004, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0056.0000.0001, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
3838.a621.e82f, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0056.0000.0003, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel300
0020.3000.0002, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel300
2cdd.e90b.25b7, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0020.1000.0003, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel300
0022.0000.0003, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0020.3000.0003, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0022.0000.0004, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet21
0020.3000.0001, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel300
0040.0100.0001, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0020.3000.0004, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel300
0056.0000.0004, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel300
0022.0000.0002, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
00aa.aaaa.aaaa, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0056.0000.0001, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel300
0022.0000.0002, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0022.0000.0001, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0040.0100.0002, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel300
0022.0000.0004, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
246c.8474.8ddb, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet15
0022.0000.0003, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet21
0056.0000.0005, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0020.1000.0001, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0022.0000.0005, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0056.0000.0002, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel300
00aa.aaaa.aaaa, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet21
0020.1000.0003, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0020.1000.0005, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
00aa.aaaa.aaaa, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet15
0020.1000.0004, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel300
0056.0000.0004, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
00aa.aaaa.aaaa, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel300
0022.0000.0002, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0020.3000.0004, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0022.0000.0004, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0056.0000.0002, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet15
0056.0000.0002, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0020.3000.0003, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel300
0022.0000.0001, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet21
0020.3000.0001, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0040.0100.0002, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0022.0000.0003, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0022.0000.0001, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet15
0020.1000.0002, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel300
246c.8474.8de0, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet15
0056.0000.0001, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0040.0100.0003, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0056.0000.0001, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet15
0020.3000.0005, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0020.3000.0002, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0056.0000.0003, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
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

## show ipv6 interface brief

```text
 Interface   Status    MTU   IPv6 Address              Addr State   Addr Source
----------- -------- ------ ------------------------- ------------- -----------
 Et30        down     1500   <linklocal-unassigned>    inactive     link local 

```

## show ipv6 bgp summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.205, local AS number 65205
Neighbor Status Codes: m - Under maintenance
  Neighbor V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
```

## show ipv6 bgp

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
RPKI Origin Validation codes: V - valid, I - invalid, U - unknown
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
```

## show ipv6 route

```text

VRF: default
Displaying 0 of 3 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route


```

## show ipv6 bgp vrf all

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
RPKI Origin Validation codes: V - valid, I - invalid, U - unknown
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
```

## show ipv6 route vrf all

```text

VRF: default
Displaying 0 of 3 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route



VRF: mgmt
Displaying 0 of 3 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route


! IPv6 routing not enabled
```

## show bgp ipv6 unicast summary lldp

```text
BGP summary information for VRF default
Router identifier 100.0.0.205, local AS number 65205
Neighbor Status Codes: m - Under maintenance
  Neighbor LLDP Neighbor                  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
```

## show ipv6 neighbors vrf all

```text

VRF: default
IPv6 Address                                  Age Hardware Addr   Interface

VRF: mgmt
IPv6 Address                                  Age Hardware Addr   Interface
```

## show ipv6 neighbors remote

```text
ARP remote bindings
VLAN IP Address MAC Address    Source         
---- ---------- -------------- ---------------
```

## show ipv6 nd ra neighbors

```text
```

## show ipv6 nd ra neighbors vrf tenant-a

```text
```

## show interfaces counters rates | nz

```text
Port      Name           Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Et1       ANET-201        0:01      0.0   0.0%        0      0.1   0.0%        0
Et2       ANET-202        0:01      0.0   0.0%        0      0.1   0.0%        0
Et3       ANET-203        0:01      0.2   0.0%        0      0.2   0.0%        0
Et15                      0:01      0.7   0.0%        1      0.7   0.0%        1
Et21      Nokia-56        0:01      0.4   0.0%        0      0.4   0.0%        0
Et25      Keysight-Gen    0:01      3.0   0.0%        4      3.0   0.0%        4
Et27                      0:01      1.2   0.0%        1      0.9   0.0%        1
Et28                      0:01      0.3   0.0%        0      0.5   0.0%        0
Po100                     0:01      0.0   0.0%        0      0.2   0.0%        0
Po200                     0:01      0.2   0.0%        0      0.2   0.0%        0
Po300                     0:01      1.5   0.0%        2      1.4   0.0%        1
```

