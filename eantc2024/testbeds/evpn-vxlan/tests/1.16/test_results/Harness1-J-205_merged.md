# Test results for Harness1-J-205

## show hostname

```text
Hostname: Harness1-J-205
FQDN:     Harness1-J-205.ns.eantc.de
```

## show ip bgp summary

```text
BGP is disabled for VRF default (Missing Router ID)

```

## show bgp evpn summary

```text
BGP is disabled for VRF default (Missing Router ID)

```

## show bgp evpn route-type auto-discovery detail

```text
BGP is disabled for VRF default
BGP routing table information for VRF default
Router identifier 0.0.0.0, local AS number 0
```

## show bgp evpn route-type mac-ip detail

```text
BGP is disabled for VRF default
BGP routing table information for VRF default
Router identifier 0.0.0.0, local AS number 0
```

## show bgp evpn route-type imet detail

```text
BGP is disabled for VRF default
BGP routing table information for VRF default
Router identifier 0.0.0.0, local AS number 0
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP is disabled for VRF default
BGP routing table information for VRF default
Router identifier 0.0.0.0, local AS number 0
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP is disabled for VRF default
BGP routing table information for VRF default
Router identifier 0.0.0.0, local AS number 0
```

## show bgp evpn route-type smet detail

```text
BGP is disabled for VRF default
BGP routing table information for VRF default
Router identifier 0.0.0.0, local AS number 0
```

## show ip route

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


```

## show ip arp

```text
Address         Age (sec)  Hardware Addr   Interface
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

```

## show ip arp vrf all

```text

VRF: default
Address         Age (sec)  Hardware Addr   Interface

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.20.19     0:00:24  c407.7858.8001  Management1
192.168.20.20     0:00:24  e484.29d0.4001  Management1
192.168.20.22     0:02:30  c407.780a.9f04  Management1
192.168.20.23     0:04:12  c407.780a.7750  Management1
192.168.20.24     0:01:54  6c87.2089.ede5  Management1
192.168.20.25     0:00:30  6c87.2089.ece5  Management1
192.168.20.26     0:03:54  04a9.59d5.df66  Management1
192.168.21.50     0:00:13  a84f.b1a5.5221  Management1
192.168.21.59     0:00:09  6607.f5d1.ae16  Management1
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
   1    5c5a.c773.4ac0    DYNAMIC     Et17       1       19:20:06 ago
  22    0019.0100.0001    DYNAMIC     Et25       1       2:22:12 ago
  22    0019.0100.0002    DYNAMIC     Et25       1       2:22:12 ago
  22    0019.0100.0003    DYNAMIC     Et25       1       2:22:12 ago
  22    0019.0100.0004    DYNAMIC     Et25       1       1:31:55 ago
  22    0019.0100.0005    DYNAMIC     Et25       1       1:31:55 ago
  22    0056.5656.5656    DYNAMIC     Po300      1       0:17:46 ago
  22    00aa.aaaa.aaaa    DYNAMIC     Po300      1       0:17:46 ago
  40    0013.0100.0002    DYNAMIC     Et15       1       0:17:58 ago
  40    0013.0100.0003    DYNAMIC     Et15       1       0:17:58 ago
  40    0016.0100.0001    DYNAMIC     Et25       1       1:00:20 ago
  40    0016.0100.0002    DYNAMIC     Et25       1       1:00:20 ago
  40    0016.0100.0003    DYNAMIC     Et25       1       1:00:20 ago
  40    0018.0100.0002    DYNAMIC     Et15       1       1:00:20 ago
  40    0018.0100.0003    DYNAMIC     Et15       1       1:00:20 ago
  40    00aa.aaaa.aaaa    DYNAMIC     Et15       1       0:26:32 ago
  40    246c.8474.8ddb    DYNAMIC     Et15       1       1:00:20 ago
  40    246c.8474.8de0    DYNAMIC     Et15       1       1 day, 0:20:00 ago
  42    0014.0100.0002    DYNAMIC     Et16       1       1:00:20 ago
  42    0014.0100.0003    DYNAMIC     Et16       1       1:00:20 ago
  42    0015.0100.0002    DYNAMIC     Et16       1       0:17:58 ago
  42    0015.0100.0003    DYNAMIC     Et16       1       0:17:58 ago
  42    0017.0100.0001    DYNAMIC     Et25       1       1:00:20 ago
  42    0017.0100.0002    DYNAMIC     Et25       1       1:00:20 ago
  42    0017.0100.0003    DYNAMIC     Et25       1       1:00:20 ago
  42    0056.5656.5656    DYNAMIC     Et16       1       2:22:08 ago
  42    00aa.aaaa.aaaa    DYNAMIC     Et16       1       0:26:32 ago
  42    4014.827b.84ab    DYNAMIC     Et16       1       0:17:46 ago
  42    4014.827b.84b0    DYNAMIC     Et16       1       23:17:55 ago
  45    0015.0100.0002    DYNAMIC     Po301      1       0:17:58 ago
  45    0015.0100.0003    DYNAMIC     Po301      1       0:17:58 ago
  45    0016.0100.0002    DYNAMIC     Po301      1       1:00:20 ago
  45    0016.0100.0003    DYNAMIC     Po301      1       1:00:20 ago
  45    0018.0100.0001    DYNAMIC     Et25       1       1:00:20 ago
  45    0018.0100.0002    DYNAMIC     Et25       1       1:00:20 ago
  45    0018.0100.0003    DYNAMIC     Et25       1       1:00:20 ago
  45    0026.f002.0000    DYNAMIC     Po301      1       1 day, 1:04:32 ago
  45    00aa.aaaa.aaaa    DYNAMIC     Po301      1       0:26:32 ago
  45    6c31.0eb7.505f    DYNAMIC     Po301      1       0:17:46 ago
  56    0013.0100.0002    DYNAMIC     Et21       1       0:17:58 ago
  56    0013.0100.0003    DYNAMIC     Et21       1       0:17:58 ago
  56    0013.0100.0004    DYNAMIC     Et21       1       0:17:58 ago
  56    0013.0100.0005    DYNAMIC     Et21       1       0:17:58 ago
  56    0014.0100.0001    DYNAMIC     Et25       1       1:00:24 ago
  56    0014.0100.0002    DYNAMIC     Et25       1       1:00:24 ago
  56    0014.0100.0003    DYNAMIC     Et25       1       1:00:24 ago
  56    0014.0100.0004    DYNAMIC     Et25       1       1:00:24 ago
  56    0014.0100.0005    DYNAMIC     Et25       1       1:00:24 ago
  56    0017.0100.0002    DYNAMIC     Et21       1       1:00:20 ago
  56    0017.0100.0003    DYNAMIC     Et21       1       1:00:20 ago
  56    0056.5656.5656    DYNAMIC     Et21       1       2:22:08 ago
  56    00aa.aaaa.aaaa    DYNAMIC     Et21       1       0:26:32 ago
 201    0013.0100.0001    DYNAMIC     Et25       1       1:00:26 ago
 201    0013.0100.0002    DYNAMIC     Et25       1       1:00:26 ago
 201    0013.0100.0003    DYNAMIC     Et25       1       1:00:26 ago
 201    0013.0100.0004    DYNAMIC     Et25       1       1:00:26 ago
 201    0013.0100.0005    DYNAMIC     Et25       1       1:00:26 ago
 201    0015.0100.0002    DYNAMIC     Po100      1       0:17:58 ago
 201    0015.0100.0003    DYNAMIC     Po100      1       0:17:58 ago
 201    0015.0100.0004    DYNAMIC     Po100      1       0:17:58 ago
 201    0015.0100.0005    DYNAMIC     Po100      1       0:17:58 ago
 201    0056.5656.5656    DYNAMIC     Po100      1       0:17:46 ago
 201    00aa.aaaa.aaaa    DYNAMIC     Po100      1       0:27:36 ago
 201    2899.3a8f.8f6f    DYNAMIC     Po100      1       1:02:17 ago
 201    444c.a873.5c75    DYNAMIC     Et48       1       0:32:36 ago
 201    7483.ef0b.a4fb    DYNAMIC     Po100      1       1:02:17 ago
 203    0013.0100.0002    DYNAMIC     Po200      1       0:17:58 ago
 203    0013.0100.0003    DYNAMIC     Po200      1       0:17:58 ago
 203    0013.0100.0004    DYNAMIC     Po200      1       0:17:58 ago
 203    0013.0100.0005    DYNAMIC     Po200      1       0:17:58 ago
 203    0015.0100.0001    DYNAMIC     Et25       1       1:00:20 ago
 203    0015.0100.0002    DYNAMIC     Et25       1       1:00:20 ago
 203    0015.0100.0003    DYNAMIC     Et25       1       1:00:20 ago
 203    0015.0100.0004    DYNAMIC     Et25       1       1:00:20 ago
 203    0015.0100.0005    DYNAMIC     Et25       1       1:00:20 ago
 203    0017.0100.0002    DYNAMIC     Po200      1       0:17:58 ago
 203    0017.0100.0003    DYNAMIC     Po200      1       0:17:58 ago
 203    0018.0100.0003    DYNAMIC     Po200      1       0:17:58 ago
 203    00aa.aaaa.aaaa    DYNAMIC     Po200      1       0:26:32 ago
 203    3838.a621.e82f    DYNAMIC     Po200      1       0:17:46 ago
Total Mac Addresses for this criterion: 80

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
0019.0100.0003, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0016.0100.0003, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0013.0100.0005, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0016.0100.0001, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0013.0100.0003, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet21
0015.0100.0002, VLAN 45, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel301
0015.0100.0003, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
00aa.aaaa.aaaa, VLAN 45, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel301
0013.0100.0003, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet15
0013.0100.0004, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0019.0100.0002, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0019.0100.0004, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0018.0100.0002, VLAN 45, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
4014.827b.84ab, VLAN 42, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet16
0014.0100.0004, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
6c31.0eb7.505f, VLAN 45, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel301
0015.0100.0005, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0015.0100.0003, VLAN 45, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel301
0015.0100.0002, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
2899.3a8f.8f6f, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
7483.ef0b.a4fb, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
00aa.aaaa.aaaa, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0018.0100.0003, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet15
0014.0100.0002, VLAN 42, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet16
3838.a621.e82f, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0013.0100.0005, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0016.0100.0002, VLAN 45, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel301
5c5a.c773.4ac0, VLAN 1, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet17
0015.0100.0003, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0019.0100.0005, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0019.0100.0001, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0013.0100.0004, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0056.5656.5656, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0013.0100.0002, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet15
0017.0100.0001, VLAN 42, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0017.0100.0002, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0013.0100.0002, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet21
0015.0100.0005, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0015.0100.0002, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0018.0100.0001, VLAN 45, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0014.0100.0002, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0013.0100.0001, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
00aa.aaaa.aaaa, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0017.0100.0003, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0018.0100.0002, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet15
0015.0100.0001, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0013.0100.0004, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet21
4014.827b.84b0, VLAN 42, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet16
246c.8474.8ddb, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet15
0056.5656.5656, VLAN 42, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet16
0013.0100.0003, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0018.0100.0003, VLAN 45, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0015.0100.0004, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0016.0100.0003, VLAN 45, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel301
0013.0100.0002, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0014.0100.0005, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0056.5656.5656, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel300
0017.0100.0002, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet21
00aa.aaaa.aaaa, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet21
0017.0100.0003, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet21
0014.0100.0001, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
00aa.aaaa.aaaa, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet15
0014.0100.0003, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
00aa.aaaa.aaaa, VLAN 22, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel300
0013.0100.0005, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet21
0015.0100.0003, VLAN 42, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet16
0056.5656.5656, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet21
444c.a873.5c75, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0013.0100.0003, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0015.0100.0004, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0017.0100.0002, VLAN 42, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0013.0100.0002, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0026.f002.0000, VLAN 45, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel301
0016.0100.0002, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
246c.8474.8de0, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet15
0015.0100.0002, VLAN 42, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet16
0014.0100.0003, VLAN 42, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet16
0018.0100.0003, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
00aa.aaaa.aaaa, VLAN 42, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet16
0017.0100.0003, VLAN 42, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
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
BGP is disabled for VRF default
BGP routing table information for VRF default
Router identifier 0.0.0.0, local AS number 0
```

## show bgp evpn instance

```text
```

## show interfaces counters rates | nz

```text
Port      Name        Intvl   In Mbps      %  In Kpps  Out Mbps      % Out Kpps
Et1       ANET-201     0:01       0.6   0.0%        1       0.4   0.0%        0
Et2       ANET-202     0:01       0.2   0.0%        0       0.4   0.0%        0
Et3       ANET-203     0:01      95.2   1.2%      170       0.8   0.0%        1
Et13      Cisco-45-46  0:05       0.2   0.0%        0       0.3   0.0%        0
Et14      Cisco-45-46  0:05       0.4   0.0%        0       0.3   0.0%        0
Et15                   0:05       6.1   0.1%       10       0.6   0.0%        1
Et16                   0:05       0.6   0.0%        1       0.6   0.0%        1
Et21      Nokia-56     0:05       0.8   0.0%        1       0.8   0.0%        1
Et25      Keysight-Ge  0:05     110.7   1.4%      186     110.4   1.4%      186
Et27                   0:05       0.2   0.0%        0      96.3   1.2%      172
Et28                   0:05       0.1   0.0%        0       3.9   0.1%        6
Et48      Spine-host   0:05       0.0   0.0%        0       2.1   0.0%        3
Ma1                    0:05       0.0   0.0%        0       0.1   0.0%        0
Po100                  0:05       0.8   0.0%        1       0.8   0.0%        1
Po200                  0:01      95.2   1.2%      170       0.8   0.0%        1
Po300                  0:05       0.3   0.0%        0     100.0   0.6%      178
Po301                  0:05       0.6   0.0%        1       0.6   0.0%        0
```

