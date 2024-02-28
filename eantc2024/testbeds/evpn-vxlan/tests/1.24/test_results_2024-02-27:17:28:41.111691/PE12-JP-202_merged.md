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
  CISCO_SPINE_IPV4         20.40.202.40   4 65040            184       214    0    0 02:23:49 Estab   4      4
  ANET.IPV4                20.200.202.200 4 65000           1876      1849    0    0 00:06:08 Idle(NoIf)
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.202, local AS number 65202
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  CISCO_EVPN_REMOTE        100.0.0.40  4 65040            258       259    0    0 02:23:44 Estab   18     18
  ANET.EVPN                100.0.0.200 4 65000           7382      4427    0    0 00:03:11 Active
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 1303 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65040:51301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 1303 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65040:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65040:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:2
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65040:1303 Route-Target-AS:65040:51301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
BGP routing table entry for auto-discovery 0300:0000:00fe:1500:0309 remote, Route Distinguisher: 100.0.0.45:6
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0300:0000:00fe:1500:0309 remote, Route Distinguisher: 100.0.0.46:6
 Paths: 1 available
  65040 65045
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
BGP routing table entry for mac-ip 3333.3333.3333 10.30.1.50 remote, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1301 L3 VNI: 1000 ESI: 0300:0000:00fe:1500:0309
BGP routing table entry for mac-ip 3333.3333.3333 10.30.1.50 remote, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65040 65045
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1301 L3 VNI: 1000 ESI: 0300:0000:00fe:1500:0309
BGP routing table entry for mac-ip 6c31.0e7b.8b87 remote, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 Route-Origin-IP:100.0.0.45:512 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0300:0000:00fe:1500:0309
BGP routing table entry for mac-ip 6c31.0e7b.8b87 remote, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65040 65045
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 Route-Origin-IP:100.0.0.45:512 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0300:0000:00fe:1500:0309
BGP routing table entry for mac-ip 6c31.0eb7.505f remote, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 Route-Origin-IP:100.0.0.46:512 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0300:0000:00fe:1500:0309
BGP routing table entry for mac-ip 6c31.0eb7.505f remote, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65040 65045
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 Route-Origin-IP:100.0.0.46:512 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0300:0000:00fe:1500:0309
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
BGP routing table entry for imet 100.0.0.45 remote, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.45
BGP routing table entry for imet 100.0.0.46 remote, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65040 65045
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.46
BGP routing table entry for imet 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65040:51301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1303 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65040:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1304 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65040:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.202
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:11:11:11:11:11 DF Election: Preference 150
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:11:11:11:11:11 DF Election: Preference 150
BGP routing table entry for ethernet-segment 0300:0000:00fe:1500:0309 100.0.0.45 remote, Route Distinguisher: 100.0.0.45:27001
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:00:00:fe:15
BGP routing table entry for ethernet-segment 0300:0000:00fe:1500:0309 100.0.0.45 remote, Route Distinguisher: 100.0.0.46:27001
 Paths: 1 available
  65040 65045
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:00:00:fe:15
BGP routing table entry for ethernet-segment 0300:0000:00fe:1500:0309 100.0.0.46 remote, Route Distinguisher: 100.0.0.45:27001
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:00:00:fe:15
BGP routing table entry for ethernet-segment 0300:0000:00fe:1500:0309 100.0.0.46 remote, Route Distinguisher: 100.0.0.46:27001
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:00:00:fe:15
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
BGP routing table entry for ip-prefix 10.10.44.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65040 65045
    - from - (0.0.0.0)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65040 65045
    - from - (0.0.0.0)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.10.44.0/24 remote, Route Distinguisher: 100.0.0.45:4
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.44.0/24 remote, Route Distinguisher: 100.0.0.46:4
 Paths: 1 available
  65040 65045
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.201.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24 remote, Route Distinguisher: 100.0.0.45:4
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24 remote, Route Distinguisher: 100.0.0.46:4
 Paths: 1 available
  65040 65045
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
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
0     2303   VXLAN 10.30.3.203        001b.0100.0003  100.0.30.14        -   
1303  1303   VXLAN 10.30.3.203        001b.0100.0003  100.0.30.14        -   
0     2303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.30.14        Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.254        0056.5656.5656  100.0.30.14        Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.0.56         Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.254        0056.5656.5656  100.0.0.56         Stic
                                                                         ky  
0     2304   VXLAN 10.30.4.203        001b.0100.0004  100.0.30.14        -   
1304  1304   VXLAN 10.30.4.203        001b.0100.0004  100.0.30.14        -   
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

 C        20.40.202.0/24
           directly connected, Ethernet48
 B E      100.0.0.40/32 [20/0]
           via 20.40.202.40, Ethernet48
 B E      100.0.0.41/32 [20/0]
           via 20.40.202.40, Ethernet48
 B E      100.0.0.45/32 [20/0]
           via 20.40.202.40, Ethernet48
 B E      100.0.0.46/32 [20/0]
           via 20.40.202.40, Ethernet48
 C        100.0.0.202/32
           directly connected, Loopback0

```

## show ip arp

```text
Address         Age (sec)  Hardware Addr   Interface
20.40.202.40      0:00:24  246c.8474.8ddb  Ethernet48
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

 C        20.40.202.0/24
           directly connected, Ethernet48
 B E      100.0.0.40/32 [20/0]
           via 20.40.202.40, Ethernet48
 B E      100.0.0.41/32 [20/0]
           via 20.40.202.40, Ethernet48
 B E      100.0.0.45/32 [20/0]
           via 20.40.202.40, Ethernet48
 B E      100.0.0.46/32 [20/0]
           via 20.40.202.40, Ethernet48
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

 C        10.20.56.0/24
           directly connected, Ethernet49/1


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

 B E      10.10.44.0/24 [20/0]
           via VTEP 100.0.0.45 VNI 1000 router-mac 6c:31:0e:7b:8b:87
 C        10.10.201.0/24
           directly connected, Vlan1201
 B E      10.30.1.0/24 [20/0]
           via VTEP 100.0.0.45 VNI 1000 router-mac 6c:31:0e:7b:8b:87

```

## show ip arp vrf all

```text

VRF: PIM
Address         Age (sec)  Hardware Addr   Interface

VRF: default
Address         Age (sec)  Hardware Addr   Interface
20.40.202.40      0:00:24  246c.8474.8ddb  Ethernet48

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.20.2      0:00:08  bcea.fa02.6ce2  Management1
192.168.20.19     0:02:22  c407.7858.8001  Management1
192.168.20.20     0:01:52  e484.29d0.4001  Management1
192.168.20.21     0:01:09  7081.85c1.b801  Management1
192.168.20.22     0:03:41  c407.780a.9f04  Management1
192.168.20.23     0:02:28  c407.780a.7750  Management1
192.168.20.24     0:00:26  6c87.2089.ede5  Management1
192.168.20.26     0:04:06  04a9.59d5.df66  Management1
192.168.20.27     0:04:55  04a9.59d5.dfe6  Management1
192.168.20.28     0:02:34  98a9.2d59.bae6  Management1
192.168.20.29     0:04:12  90f7.b223.d466  Management1
192.168.20.52     0:00:26  f83e.95dc.1289  Management1
192.168.21.47     0:00:20  5c5a.c7ff.8a0a  Management1
192.168.21.50     0:03:29  a84f.b1a5.5221  Management1
192.168.21.59     0:02:34  6607.f5d1.ae16  Management1

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
1000       4092       tenant-a       evpn         

```

## show mac address-table

```text
          Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports      Moves   Last Move
----    -----------       ----        -----      -----   ---------
1201    00aa.aaaa.aaaa    STATIC      Router
1201    2cdd.e90b.25b7    STATIC      Router
1202    00aa.aaaa.aaaa    STATIC      Router
1202    2cdd.e90b.25b7    STATIC      Router
1301    00aa.aaaa.aaaa    STATIC      Router
1301    2cdd.e90b.25b7    STATIC      Router
1302    00aa.aaaa.aaaa    STATIC      Router
1302    2cdd.e90b.25b7    STATIC      Router
1303    00aa.aaaa.aaaa    STATIC      Router
1303    2cdd.e90b.25b7    STATIC      Router
1304    00aa.aaaa.aaaa    STATIC      Router
1304    2cdd.e90b.25b7    STATIC      Router
4092    00aa.aaaa.aaaa    STATIC      Router
4092    2cdd.e90b.25b7    STATIC      Router
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
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65040:51301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 1303 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65040:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65040:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:2
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65040:1303 Route-Target-AS:65040:51301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
BGP routing table entry for auto-discovery 0300:0000:00fe:1500:0309 remote, Route Distinguisher: 100.0.0.45:6
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0300:0000:00fe:1500:0309 remote, Route Distinguisher: 100.0.0.46:6
 Paths: 1 available
  65040 65045
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for mac-ip 3333.3333.3333 10.30.1.50 remote, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1301 L3 VNI: 1000 ESI: 0300:0000:00fe:1500:0309
BGP routing table entry for mac-ip 3333.3333.3333 10.30.1.50 remote, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65040 65045
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1301 L3 VNI: 1000 ESI: 0300:0000:00fe:1500:0309
BGP routing table entry for mac-ip 6c31.0e7b.8b87 remote, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 Route-Origin-IP:100.0.0.45:512 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0300:0000:00fe:1500:0309
BGP routing table entry for mac-ip 6c31.0e7b.8b87 remote, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65040 65045
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 Route-Origin-IP:100.0.0.45:512 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0300:0000:00fe:1500:0309
BGP routing table entry for mac-ip 6c31.0eb7.505f remote, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 Route-Origin-IP:100.0.0.46:512 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0300:0000:00fe:1500:0309
BGP routing table entry for mac-ip 6c31.0eb7.505f remote, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65040 65045
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 Route-Origin-IP:100.0.0.46:512 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0300:0000:00fe:1500:0309
BGP routing table entry for imet 100.0.0.45 remote, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.45
BGP routing table entry for imet 100.0.0.46 remote, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65040 65045
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.46
BGP routing table entry for imet 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65040:51301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1303 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65040:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1304 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65040:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:11:11:11:11:11 DF Election: Preference 150
BGP routing table entry for ethernet-segment 0300:0000:00fe:1500:0309 100.0.0.45 remote, Route Distinguisher: 100.0.0.45:27001
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:00:00:fe:15
BGP routing table entry for ethernet-segment 0300:0000:00fe:1500:0309 100.0.0.45 remote, Route Distinguisher: 100.0.0.46:27001
 Paths: 1 available
  65040 65045
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:00:00:fe:15
BGP routing table entry for ethernet-segment 0300:0000:00fe:1500:0309 100.0.0.46 remote, Route Distinguisher: 100.0.0.45:27001
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:00:00:fe:15
BGP routing table entry for ethernet-segment 0300:0000:00fe:1500:0309 100.0.0.46 remote, Route Distinguisher: 100.0.0.46:27001
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:00:00:fe:15
BGP routing table entry for ip-prefix 10.10.44.0/24 remote, Route Distinguisher: 100.0.0.45:4
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.44.0/24 remote, Route Distinguisher: 100.0.0.46:4
 Paths: 1 available
  65040 65045
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.201.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24 remote, Route Distinguisher: 100.0.0.45:4
 Paths: 1 available
  65040 65045
    100.0.0.45 from 100.0.0.40 (100.0.0.40)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24 remote, Route Distinguisher: 100.0.0.46:4
 Paths: 1 available
  65040 65045
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1000
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
    ESI: 0000:1111:1111:1111:1111
      Interface: Vxlan1
      Mode: all-active
      State: up
      ES-Import RT: 00:11:11:11:11:11
      DF election algorithm: preference
      Designated forwarder: 100.0.0.202
EVPN instance: VLAN 1301
  Route distinguisher: 100.0.0.202:1301
  Route distinguisher remote: 100.0.0.202:1301
  Route target import: Route-Target-AS:1301:1301
  Route target export: Route-Target-AS:1301:1301
  Route target import remote: Route-Target-AS:65040:51301
  Route target export remote: Route-Target-AS:65040:51301
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.202
  VXLAN: enabled
  MPLS: disabled
  Local ethernet segment:
    ESI: 0000:1111:1111:1111:1111
      Interface: Vxlan1
      Mode: all-active
      State: up
      ES-Import RT: 00:11:11:11:11:11
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
    ESI: 0000:1111:1111:1111:1111
      Interface: Vxlan1
      Mode: all-active
      State: up
      ES-Import RT: 00:11:11:11:11:11
      DF election algorithm: preference
      Designated forwarder: 100.0.0.202
EVPN instance: VLAN-aware bundle 1303-1304
  Route distinguisher: 100.0.0.202:1303
  Route distinguisher remote: 100.0.0.202:1303
  Route target import: Route-Target-AS:1303:1303
  Route target export: Route-Target-AS:1303:1303
  Route target import remote: Route-Target-AS:65040:1303
  Route target export remote: Route-Target-AS:65040:1303
  Service interface: VLAN-aware bundle
  Local VXLAN IP address: 100.0.0.202
  VXLAN: enabled
  MPLS: disabled
  Local ethernet segment:
    ESI: 0000:1111:1111:1111:1111
      Interface: Vxlan1
      Mode: all-active
      State: up
      ES-Import RT: 00:11:11:11:11:11
      DF election algorithm: preference
      Designated forwarder: 100.0.0.202
```

## show interfaces counters rates | nz

```text
Port      Name           Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Ma1                       0:05      0.0   0.0%        0      0.1   0.0%        0
```

