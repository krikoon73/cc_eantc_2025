# Test results for Harness1-J-205

## show hostname

```text
Hostname: Harness1-J-205
FQDN:     Harness1-J-205.ns.eantc.de
```

## show ip bgp summary

```text
BGP is disabled for VRF default
```

## show bgp evpn summary

```text
BGP is disabled for VRF default
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

## show bgp evpn route-type spmsi detail

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
192.168.20.19     0:00:49  c407.7858.8001  Management1
192.168.20.22     0:02:37  c407.780a.9f04  Management1
192.168.20.23     0:00:55  c407.780a.7750  Management1
192.168.20.24     0:02:37  6c87.2089.ede5  Management1
192.168.20.25     0:00:49  6c87.2089.ece5  Management1
192.168.20.26     0:03:55  04a9.59d5.df66  Management1
192.168.21.47     0:04:13  5c5a.c7ff.8a0a  Management1
192.168.21.50     0:02:43  a84f.b1a5.5221  Management1
192.168.21.59     0:04:19  6607.f5d1.ae16  Management1
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
   1    444c.a873.5ca5    DYNAMIC     Et48       1       1 day, 20:39:11 ago
   1    5c5a.c773.4ac0    DYNAMIC     Et17       1       1 day, 20:38:36 ago
  40    00aa.aaaa.aaaa    DYNAMIC     Et15       1       0:21:37 ago
  40    246c.8474.8de0    DYNAMIC     Et15       1       2 days, 23:20:31 ago
  42    00aa.aaaa.aaaa    DYNAMIC     Et16       1       0:11:25 ago
  42    4014.827b.84b0    DYNAMIC     Et16       1       2 days, 22:18:26 ago
  45    0026.f002.0000    DYNAMIC     Po301      1       3 days, 0:05:03 ago
  45    00aa.aaaa.aaaa    DYNAMIC     Po301      1       1:09:46 ago
  56    0014.0100.0001    DYNAMIC     Et25       1       0:39:43 ago
  56    0056.5656.5656    DYNAMIC     Et21       1       0:41:52 ago
 201    0013.0100.0001    DYNAMIC     Et25       1       18:21:26 ago
 201    00aa.aaaa.aaaa    DYNAMIC     Po100      1       0:00:40 ago
 201    444c.a873.5c75    DYNAMIC     Et48       1       0:00:40 ago
 201    7483.ef0b.a4fb    DYNAMIC     Po100      1       18:32:15 ago
 203    0015.0100.0001    DYNAMIC     Et25       1       18:21:26 ago
 203    3838.a621.e82f    DYNAMIC     Po200      1       17:36:15 ago
 203    985d.82a2.04f9    DYNAMIC     Po200      1       17:36:11 ago
Total Mac Addresses for this criterion: 17

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
985d.82a2.04f9, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
7483.ef0b.a4fb, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
00aa.aaaa.aaaa, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
3838.a621.e82f, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
5c5a.c773.4ac0, VLAN 1, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet17
0013.0100.0001, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
0015.0100.0001, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
4014.827b.84b0, VLAN 42, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet16
0014.0100.0001, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
00aa.aaaa.aaaa, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet15
0056.5656.5656, VLAN 56, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet21
444c.a873.5c75, VLAN 201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
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
Et2       ANET-202     0:01       0.6   0.0%        1       0.6   0.0%        1
Et3       ANET-203     0:01       0.6   0.0%        1       0.0   0.0%        0
Et4       ANET-204     0:01       0.0   0.0%        0       0.6   0.0%        1
Et21      Nokia-56     0:05       0.9   0.0%        1       0.6   0.0%        1
Et25      Keysight-Ge  0:05       2.0   0.0%        3       2.3   0.0%        3
Et48      Spine-host   0:05       0.0   0.0%        0       4.1   0.1%        6
Ma1                    0:05       0.0   0.0%        0       0.1   0.0%        0
Po100                  0:01       0.6   0.0%        1       0.6   0.0%        1
Po200                  0:05       0.6   0.0%        1       0.6   0.0%        0
```

