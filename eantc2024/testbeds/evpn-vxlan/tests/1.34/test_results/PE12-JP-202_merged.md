# Test results for PE12-JP-202

## show hostname

```text
Hostname: PE12-JP-202
FQDN:     PE12-JP-202.ns.eantc.de
```

## show ip bgp summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.202, local AS number 65202
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor       V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  ANET.IPV4                20.200.202.200 4 65000              0         0    0    0 00:44:00 Idle(NoIf)
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.202, local AS number 65202
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  ANET.EVPN                100.0.0.200 4 65000              0         0    0    0 00:44:00 Active
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
```

## show bgp evpn route-type imet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
BGP routing table entry for imet 100.0.0.202, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
      PMSI Tunnel: Ingress Replication, MPLS Label: 1201, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 100.0.0.202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 100.0.0.202, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1303 100.0.0.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1304 100.0.0.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.202
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb
      VNI: 1000
BGP routing table entry for ip-prefix 100.0.1.202/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb
      VNI: 1000
```

## show bgp evpn route-type smet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
```

## show bgp evpn route-type spmsi detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
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

 C        100.0.0.202/32
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

 C        100.0.0.202/32
           directly connected, Loopback0


VRF: PIM
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

 B E      10.10.22.202/32 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.22.254/32 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.22.0/24 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.40.202/32 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.40.0/24 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.42.202/32 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.42.0/24 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.56.0/24 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.201.0/24 [20/0]
           via 10.20.206.206, Ethernet6
 C        10.10.202.0/24
           directly connected, Vlan1202
 B E      10.10.203.0/24 [20/0]
           via 10.20.206.206, Ethernet6
 C        10.20.56.0/24
           directly connected, Ethernet49/1
 C        10.20.206.0/24
           directly connected, Ethernet6
 B E      10.30.1.0/24 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.30.2.0/24 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.30.3.0/24 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.30.4.0/24 [20/0]
           via 10.20.206.206, Ethernet6
 B E      100.0.1.201/32 [20/0]
           via 10.20.206.206, Ethernet6
 C        100.0.1.202/32
           directly connected, Loopback1000
 B E      100.0.1.203/32 [20/0]
           via 10.20.206.206, Ethernet6
 B E      100.0.1.204/32 [20/0]
           via 10.20.206.206, Ethernet6


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


VRF: tenant-a
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

 C        10.10.201.0/24
           directly connected, Vlan1201
 C        10.30.1.0/24
           directly connected, Vlan1301
 C        10.30.2.0/24
           directly connected, Vlan1302
 C        10.30.3.0/24
           directly connected, Vlan1303
 C        10.30.4.0/24
           directly connected, Vlan1304
 C        100.0.1.202/32
           directly connected, Loopback100

```

## show ip arp vrf all

```text

VRF: PIM
Address         Age (sec)  Hardware Addr   Interface
10.20.206.206     0:00:45  985d.82c4.0271  Ethernet6

VRF: default
Address         Age (sec)  Hardware Addr   Interface

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.20.2      0:00:39  bcea.fa02.6ce2  Management1
192.168.20.18     0:00:39  e484.29cd.e801  Management1
192.168.20.19     0:00:33  c407.7858.8001  Management1
192.168.20.20     0:00:33  e484.29d0.4001  Management1
192.168.20.21     0:00:09  7081.85c1.b801  Management1
192.168.20.22     0:00:21  c407.780a.9f04  Management1
192.168.20.23     0:00:03  c407.780a.7750  Management1
192.168.20.24     0:00:33  6c87.2089.ede5  Management1
192.168.20.25     0:00:15  6c87.2089.ece5  Management1
192.168.20.26     0:00:33  04a9.59d5.df66  Management1
192.168.20.27     0:04:43  04a9.59d5.dfe6  Management1
192.168.20.28     0:00:46  98a9.2d59.bae6  Management1
192.168.20.29     0:00:09  90f7.b223.d466  Management1
192.168.20.52     0:02:11  f83e.95dc.1289  Management1

VRF: tenant-a
Address         Age (sec)  Hardware Addr   Interface
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
VNI to VLAN Mapping for Vxlan1
VNI        VLAN       Source       Interface             802.1Q Tag
---------- ---------- ------------ --------------------- ----------
1201       1201       static       Port-Channel100       1201      
                                   Vxlan1                1201      
1301       1301       static       Port-Channel100       1301      
                                   Vxlan1                1301      
1302       1302       static       Port-Channel100       1302      
                                   Vxlan1                1302      
1303       1303       static       Port-Channel100       1303      
                                   Vxlan1                1303      
1304       1304       static       Port-Channel100       1304      
                                   Vxlan1                1304      

VNI to dynamic VLAN Mapping for Vxlan1
VNI        VLAN       VRF            Source       
---------- ---------- -------------- ------------ 
1000       4094       tenant-a       evpn         

```

## show mac address-table

```text
          Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports      Moves   Last Move
----    -----------       ----        -----      -----   ---------
1201    00aa.aaaa.aaaa    STATIC      Router
1201    7483.ef0b.a4fb    STATIC      Router
1202    00aa.aaaa.aaaa    STATIC      Router
1202    7483.ef0b.a4fb    STATIC      Router
1301    00aa.aaaa.aaaa    STATIC      Router
1301    7483.ef0b.a4fb    STATIC      Router
1302    00aa.aaaa.aaaa    STATIC      Router
1302    7483.ef0b.a4fb    STATIC      Router
1303    00aa.aaaa.aaaa    STATIC      Router
1303    7483.ef0b.a4fb    STATIC      Router
1304    00aa.aaaa.aaaa    STATIC      Router
1304    7483.ef0b.a4fb    STATIC      Router
4094    00aa.aaaa.aaaa    STATIC      Router
4094    7483.ef0b.a4fb    STATIC      Router
Total Mac Addresses for this criterion: 14

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
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
Router identifier 100.0.0.202, local AS number 65202
```

## show bgp evpn instance

```text
EVPN instance: VLAN 1201
  Route distinguisher: 100.0.0.202:1201
  Route target import: Route-Target-AS:1201:1201
  Route target export: Route-Target-AS:1201:1201
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.202
  VXLAN: enabled
  MPLS: disabled
EVPN instance: VLAN 1301
  Route distinguisher: 100.0.0.202:1301
  Route target import: Route-Target-AS:1301:1301
  Route target export: Route-Target-AS:1301:1301
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.202
  VXLAN: enabled
  MPLS: disabled
EVPN instance: VLAN 1302
  Route distinguisher: 100.0.0.202:1302
  Route target import: Route-Target-AS:1302:1302
  Route target export: Route-Target-AS:1302:1302
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.202
  VXLAN: enabled
  MPLS: disabled
EVPN instance: VLAN-aware bundle 1303-1304
  Route distinguisher: 100.0.0.202:1303
  Route target import: Route-Target-AS:1303:1303
  Route target export: Route-Target-AS:1303:1303
  Service interface: VLAN-aware bundle
  Local VXLAN IP address: 100.0.0.202
  VXLAN: enabled
  MPLS: disabled
```

## show ip igmp snooping groups local

```text
IGMP Snooping Group Membership
EX : Filter mode Exclude
IN : Filter mode Include
IR : Ingress Replication
VLAN  Group            Members
----  ---------------  ----------------------------------------
1201  *                Cpu
1202  *                Cpu
1301  *                Cpu
1302  *                Cpu
1303  *                Cpu
1304  *                Cpu
```

## show ip igmp snooping groups evpn

```text
IGMP Snooping Group Membership
EX : Filter mode Exclude
IN : Filter mode Include
IR : Ingress Replication
VLAN  Group            Members
----  ---------------  ----------------------------------------
```

## show ip mroute vrf tenant-a detail

```text
PIM Bidirectional Mode Multicast Routing Table
RPF route: U - From unicast routing table
           M - From multicast routing table
PIM Sparse Mode Multicast Routing Table
Flags: E - Entry forwarding on the RPT, J - Joining to the SPT
    R - RPT bit is set, S - SPT bit is set, L - Source is attached
    W - Wildcard entry, X - External component interest
    I - SG Include Join alert rcvd, P - Programmed in hardware
    H - Joining SPT due to policy, D - Joining SPT due to protocol
    Z - Entry marked for deletion, C - Learned from a DR via a register
    A - Learned via Anycast RP Router, M - Learned via MSDP
    N - May notify MSDP, K - Keepalive timer not running
    T - Switching Incoming Interface, B - Learned via Border Router
    V - Source is reachable via Evpn Tenant Domain
    F - Learned via MVPN
RPF route: U - From unicast routing table
           M - From multicast routing table
* - Interface has EVPN information available in the 'detail' command output
```

## show ip igmp vrf tenant-a groups detail

```text
```

## show ip igmp vrf tenant-a interface

```text
Vlan1201 is up
  IGMP on this interface: enabled
  Interface address: 10.10.201.254
  Multicast routing on this interface: enabled
  Multicast TTL threshold: 0
  Current IGMP router version: 3
  IGMP query interval: 125 seconds
  IGMP max query response time: 100 deciseconds
  Last member query response interval: 10 deciseconds
  Last member query response count: 2
  IGMP querier: 100.0.1.202
  Robustness: 2
  Require router alert: routerAlertOptionalConnected
  Startup query interval: 312 deciseconds
  Startup query count: 2
  General query timer expiry: 0:00:54
  Multicast groups joined:
Vlan1301 is up
  IGMP on this interface: enabled
  Interface address: 10.30.1.254
  Multicast routing on this interface: enabled
  Multicast TTL threshold: 0
  Current IGMP router version: 3
  IGMP query interval: 125 seconds
  IGMP max query response time: 100 deciseconds
  Last member query response interval: 10 deciseconds
  Last member query response count: 2
  IGMP querier: 100.0.1.202
  Robustness: 2
  Require router alert: routerAlertOptionalConnected
  Startup query interval: 312 deciseconds
  Startup query count: 2
  General query timer expiry: 0:00:55
  Multicast groups joined:
Vlan1302 is up
  IGMP on this interface: enabled
  Interface address: 10.30.2.254
  Multicast routing on this interface: enabled
  Multicast TTL threshold: 0
  Current IGMP router version: 3
  IGMP query interval: 125 seconds
  IGMP max query response time: 100 deciseconds
  Last member query response interval: 10 deciseconds
  Last member query response count: 2
  IGMP querier: 100.0.1.202
  Robustness: 2
  Require router alert: routerAlertOptionalConnected
  Startup query interval: 312 deciseconds
  Startup query count: 2
  General query timer expiry: 0:00:53
  Multicast groups joined:
Vlan1303 is up
  IGMP on this interface: enabled
  Interface address: 10.30.3.254
  Multicast routing on this interface: enabled
  Multicast TTL threshold: 0
  Current IGMP router version: 3
  IGMP query interval: 125 seconds
  IGMP max query response time: 100 deciseconds
  Last member query response interval: 10 deciseconds
  Last member query response count: 2
  IGMP querier: 100.0.1.202
  Robustness: 2
  Require router alert: routerAlertOptionalConnected
  Startup query interval: 312 deciseconds
  Startup query count: 2
  General query timer expiry: 0:00:58
  Multicast groups joined:
Vlan1304 is up
  IGMP on this interface: enabled
  Interface address: 10.30.4.254
  Multicast routing on this interface: enabled
  Multicast TTL threshold: 0
  Current IGMP router version: 3
  IGMP query interval: 125 seconds
  IGMP max query response time: 100 deciseconds
  Last member query response interval: 10 deciseconds
  Last member query response count: 2
  IGMP querier: 100.0.1.202
  Robustness: 2
  Require router alert: routerAlertOptionalConnected
  Startup query interval: 312 deciseconds
  Startup query count: 2
  General query timer expiry: 0:00:58
  Multicast groups joined:
```

## show ip pim vrf tenant-a neighbor

```text
PIM Neighbor Table for tenant-a VRF
Neighbor Address  Interface  Uptime  Expires  Mode  Transport
```

## show pim ipv4 sparse-mode evpn gateway detail

```text
```

## show pim evpn gateway dr

```text
```

## show ip mroute detail

```text
PIM Bidirectional Mode Multicast Routing Table
RPF route: U - From unicast routing table
           M - From multicast routing table
PIM Sparse Mode Multicast Routing Table
Flags: E - Entry forwarding on the RPT, J - Joining to the SPT
    R - RPT bit is set, S - SPT bit is set, L - Source is attached
    W - Wildcard entry, X - External component interest
    I - SG Include Join alert rcvd, P - Programmed in hardware
    H - Joining SPT due to policy, D - Joining SPT due to protocol
    Z - Entry marked for deletion, C - Learned from a DR via a register
    A - Learned via Anycast RP Router, M - Learned via MSDP
    N - May notify MSDP, K - Keepalive timer not running
    T - Switching Incoming Interface, B - Learned via Border Router
    V - Source is reachable via Evpn Tenant Domain
    F - Learned via MVPN
RPF route: U - From unicast routing table
           M - From multicast routing table
* - Interface has EVPN information available in the 'detail' command output
```

## show ip pim neighbor

```text
PIM Neighbor Table for default VRF
Neighbor Address  Interface  Uptime  Expires  Mode  Transport
```

## show interfaces counters rates | nz

```text
Port      Name        Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
```

