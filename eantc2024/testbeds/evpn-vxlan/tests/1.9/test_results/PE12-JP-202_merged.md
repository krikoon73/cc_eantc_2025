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
  ANET.IPV4                20.200.202.200 4 65000           3315      3162    0    0 00:30:18 Idle(NoIf)
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.202, local AS number 65202
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  ANET.EVPN                100.0.0.200 4 65000           9876      8976    0    0 00:27:21 Active
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
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
BGP routing table entry for ethernet-segment 0000:0000:0000:0201:0202 100.0.0.202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:10:02:02 DF Election: Preference 200
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
VLAN  Label  Encap IP                 MAC             Tunnel Endpoint    Seq#
----- ------ ----- ------------------ --------------- ------------------ ----
1303  1303   VXLAN 10.30.3.103        0022.2200.0004  100.0.0.103        -   
1303  1303   VXLAN 10.30.3.40         0016.0100.0004  100.0.0.40         -   
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

 B E      10.10.40.25/32 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.40.202/32 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.40.0/24 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.42.25/32 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.42.202/32 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.42.0/24 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.45.25/32 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.45.202/32 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.45.0/24 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.56.56/32 [20/0]
           via 10.20.206.206, Ethernet6
 B E      10.10.56.202/32 [20/0]
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
 B E      10.30.2.56/32 [20/0]
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
10.20.206.206     0:00:34  985d.82c4.0271  Ethernet6
10.20.56.56       0:00:22  407c.7dc4.ab93  Ethernet49/1
10.10.202.202     0:11:23  0013.0100.0001  Vlan1202, not learned

VRF: default
Address         Age (sec)  Hardware Addr   Interface

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.20.2      0:00:06  bcea.fa02.6ce2  Management1
192.168.20.18     0:04:47  e484.29cd.e801  Management1
192.168.20.19     0:01:32  c407.7858.8001  Management1
192.168.20.21     0:03:21  7081.85c1.b801  Management1
192.168.20.22     0:01:32  c407.780a.9f04  Management1
192.168.20.23     0:03:09  c407.780a.7750  Management1
192.168.20.24     0:01:50  6c87.2089.ede5  Management1
192.168.20.25     0:01:44  6c87.2089.ece5  Management1
192.168.20.26     0:04:40  04a9.59d5.df66  Management1
192.168.20.29     0:01:56  90f7.b223.d466  Management1
192.168.20.52     0:01:56  f83e.95dc.1289  Management1
192.168.21.50     0:03:21  a84f.b1a5.5221  Management1
192.168.21.59     0:00:18  6607.f5d1.ae16  Management1

VRF: tenant-a
Address         Age (sec)  Hardware Addr   Interface
10.30.3.40        0:55:01  0016.0100.0004  Vlan1303, not learned
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
  Local ethernet segment:
    ESI: 0000:0000:0000:0201:0202
      Interface: Port-Channel100
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:10:02:02
      DF election algorithm: preference
      Designated forwarder: 100.0.0.202
EVPN instance: VLAN 1301
  Route distinguisher: 100.0.0.202:1301
  Route target import: Route-Target-AS:1301:1301
  Route target export: Route-Target-AS:1301:1301
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.202
  VXLAN: enabled
  MPLS: disabled
  Local ethernet segment:
    ESI: 0000:0000:0000:0201:0202
      Interface: Port-Channel100
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:10:02:02
      DF election algorithm: preference
      Designated forwarder: 100.0.0.202
EVPN instance: VLAN 1302
  Route distinguisher: 100.0.0.202:1302
  Route target import: Route-Target-AS:1302:1302
  Route target export: Route-Target-AS:1302:1302
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.202
  VXLAN: enabled
  MPLS: disabled
  Local ethernet segment:
    ESI: 0000:0000:0000:0201:0202
      Interface: Port-Channel100
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:10:02:02
      DF election algorithm: preference
      Designated forwarder: 100.0.0.202
EVPN instance: VLAN-aware bundle 1303-1304
  Route distinguisher: 100.0.0.202:1303
  Route target import: Route-Target-AS:1303:1303
  Route target export: Route-Target-AS:1303:1303
  Service interface: VLAN-aware bundle
  Local VXLAN IP address: 100.0.0.202
  VXLAN: enabled
  MPLS: disabled
  Local ethernet segment:
    ESI: 0000:0000:0000:0201:0202
      Interface: Port-Channel100
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:10:02:02
      DF election algorithm: preference
      Designated forwarder: 100.0.0.202
```

## show interfaces counters rates | nz

```text
Port      Name        Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Ma1                    0:05      0.0   0.0%        0      0.1   0.0%        0
```

