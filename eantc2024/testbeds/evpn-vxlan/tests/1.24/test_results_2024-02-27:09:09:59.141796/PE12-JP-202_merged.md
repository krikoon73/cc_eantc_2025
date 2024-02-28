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
  ANET.IPV4                20.200.202.200 4 65000           1509      1487    0    0 14:43:53 Estab   13     13
  SPINE_EVPN_REMOTE        100.0.0.205    4 65205           4539      3731    0    0 14:43:53 Estab(NotNegotiated)
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.202, local AS number 65202
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  ANET.EVPN                100.0.0.200 4 65000           4227      2334    0    0 14:43:52 Estab   98     85
  SPINE_EVPN_REMOTE        100.0.0.205 4 65205           4539      3731    0    0 14:43:54 Estab   66     66
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 1303 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1303 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 1304 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 1303 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1303
BGP routing table entry for auto-discovery 1303 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1304
BGP routing table entry for auto-discovery 1304 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.201:2
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      Rx path id: 0x1
      VNI: 0
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:2
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65205:1301 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
BGP routing table entry for auto-discovery 0 0000:2222:2222:2222:1111 remote, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1301
BGP routing table entry for auto-discovery 1303 0000:2222:2222:2222:1111 remote, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1303
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111 remote, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      Rx path id: 0x1
      VNI: 0
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111 remote, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      Rx path id: 0x1
      VNI: 0
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111 remote, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      Rx path id: 0x1
      VNI: 0
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111 remote, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      Rx path id: 0x1
      VNI: 0
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
BGP routing table entry for mac-ip 001b.0100.0001, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0001, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0001 10.10.203.203, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1203 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0001 10.10.203.203, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1203 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0002, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.201, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.201, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.203, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.203, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0056.5656.5656, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 0056.5656.5656, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 0056.5656.5656 10.30.1.254, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 0056.5656.5656 10.30.1.254, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 00aa.aaaa.aaaa, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 00aa.aaaa.aaaa, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 00cc.cccc.bbbb, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip a244.0101.0001, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip a244.0101.0001, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip a244.0101.0001 10.30.1.103, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip a244.0101.0001 10.30.1.103, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0003, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0056.5656.5656, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 0056.5656.5656, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 a266.0102.0001, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 a266.0102.0001, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 a266.0102.0001 10.30.3.103, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 a266.0102.0001 10.30.3.103, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0004, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.0004 10.30.4.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.0004 10.30.4.203, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 0056.5656.5656, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 0056.5656.5656, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 a288.0103.0001, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 a288.0103.0001, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 a288.0103.0001 10.30.4.103, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 a288.0103.0001 10.30.4.103, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.201 remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:51301:51301 Route-Target-AS:65300:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.201 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.203 remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:51301:51301 Route-Target-AS:65300:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.203 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 0056.5656.5656 10.10.103.254 remote, Route Distinguisher: 100.0.0.56:1103
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1103 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.30.1.254 remote, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.30.2.254 remote, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1302:1302 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.103.254 remote, Route Distinguisher: 100.0.0.56:1103
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1103 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.203.254 remote, Route Distinguisher: 100.0.0.56:1203
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1203:1203 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1203 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254 remote, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00cc.cccc.bbbb remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 00cc.cccc.bbbb remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip a244.0101.0001 10.30.1.103 remote, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 001b.0100.0003 remote, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0003 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203 remote, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:51301:51301 Route-Target-AS:65300:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254 remote, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254 remote, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 a266.0102.0001 10.30.3.103 remote, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1303 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1304 001b.0100.0004 remote, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0004 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0004 10.30.4.203 remote, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:51301:51301 Route-Target-AS:65300:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0004 10.30.4.203 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254 remote, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254 remote, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 a288.0103.0001 10.30.4.103 remote, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
```

## show bgp evpn route-type imet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
      PMSI Tunnel: Ingress Replication, MPLS Label: 1201, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.201
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
BGP routing table entry for imet 100.0.0.203, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan Multicast Flags: IGMP proxy, OISM-supported, SBD
      VNI: 1000
      PMSI Tunnel: Ingress Replication, MPLS Label: 1000, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 100.0.0.203, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
      PMSI Tunnel: Ingress Replication, MPLS Label: 1203, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 100.0.0.203, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 100.0.0.203, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 100.0.0.204, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan Multicast Flags: IGMP proxy, OISM-supported, SBD
      VNI: 1000
      PMSI Tunnel: Ingress Replication, MPLS Label: 1000, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 100.0.0.204, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
      PMSI Tunnel: Ingress Replication, MPLS Label: 1203, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 100.0.0.204, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 100.0.0.204, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 100.0.30.14, Route Distinguisher: 100.0.30.14:1301
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.30.14
BGP routing table entry for imet 1303 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1303 100.0.0.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1303 100.0.0.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 1303 100.0.0.204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 1303 100.0.30.14, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.30.14
BGP routing table entry for imet 1304 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1304 100.0.0.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1304 100.0.0.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 1304 100.0.0.204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 1304 100.0.30.14, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.30.14
BGP routing table entry for imet 100.0.0.56 remote, Route Distinguisher: 100.0.0.56:1103
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1103
      PMSI Tunnel: Ingress Replication, MPLS Label: 1103, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.56 remote, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.201 remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1303 100.0.0.56 remote, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1303 100.0.0.201 remote, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1303 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1304 100.0.0.56 remote, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1304 100.0.0.201 remote, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1304 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.202
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
BGP routing table entry for ethernet-segment 0000:0000:0000:0203:0204 100.0.0.203, Route Distinguisher: 100.0.0.203:1
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:30:02:04 DF Election: Preference 100
BGP routing table entry for ethernet-segment 0000:0000:0000:0203:0204 100.0.0.204, Route Distinguisher: 100.0.0.204:1
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:30:02:04 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.201, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:01:11:11:11 DF Election: Preference 100
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:01:11:11:11 DF Election: Preference 150
BGP routing table entry for ethernet-segment 0000:0000:0000:0111:0111 100.0.0.56 remote, Route Distinguisher: 100.0.0.56:0
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:00:00:00:00:00:01
      Rx path id: 0x1
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.201 remote, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:01:11:11:11 DF Election: Preference 100
      Rx path id: 0x1
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:01:11:11:11 DF Election: Preference 150
BGP routing table entry for ethernet-segment 0000:2222:2222:2222:1111 100.0.0.56 remote, Route Distinguisher: 100.0.0.56:0
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:00:22:22:22:22:22
      Rx path id: 0x1
BGP routing table entry for ethernet-segment 0048:5648:5648:5648:5648 100.0.0.56 remote, Route Distinguisher: 100.0.0.56:0
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:48:56:48:56:48:56
      Rx path id: 0x1
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
BGP routing table entry for ip-prefix 10.10.103.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.10.103.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 2:2:None
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 3 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 2:2:None
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.103/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.1.103/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 2:2:None
BGP routing table entry for ip-prefix 10.30.1.201/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.1.201/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 2:2:None
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.1.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 2:2:None
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 3 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 2:2:None
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.103/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.3.103/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 2:2:None
BGP routing table entry for ip-prefix 10.30.3.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.3.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 2:2:None
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 3 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 2:2:None
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.103/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.4.103/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 2:2:None
BGP routing table entry for ip-prefix 10.30.4.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.4.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 2:2:None
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.203/32, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 100.0.1.204/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.204/32, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.103.0/24 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.10.201.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.201.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.203/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.203/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.0/24 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.1.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 3 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.103/32 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.1.201/32 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.1.201/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.201/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.203/32 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.1.203/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.203/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.2.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 3 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.0/24 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.3.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 3 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.103/32 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.3.203/32 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.3.203/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.203/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.0/24 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.4.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 3 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.103/32 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.4.203/32 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.4.203/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.203/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.203/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.203/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.204/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.204/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
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
1301  1301   VXLAN 10.30.1.201        001b.0100.0002  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.201        001b.0100.0002  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.254        00aa.aaaa.aaaa  100.0.0.56         Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.254        00aa.aaaa.aaaa  100.0.0.201        Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.103        a244.0101.0001  100.0.0.56         -   
1301  1301   VXLAN 10.30.1.103        a244.0101.0001  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.203        001b.0100.0002  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.203        001b.0100.0002  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.254        0056.5656.5656  100.0.0.56         Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.254        0056.5656.5656  100.0.0.201        Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.203        001b.0100.0003  100.0.0.203        -   
1303  1303   VXLAN 10.30.3.203        001b.0100.0003  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.0.56         Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.0.201        Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.254        0056.5656.5656  100.0.0.56         Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.254        0056.5656.5656  100.0.0.201        Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.103        a266.0102.0001  100.0.0.56         -   
1303  1303   VXLAN 10.30.3.103        a266.0102.0001  100.0.0.201        -   
1304  1304   VXLAN 10.30.4.203        001b.0100.0004  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.203        001b.0100.0004  100.0.0.203        -   
1304  1304   VXLAN 10.30.4.254        0056.5656.5656  100.0.0.56         Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.254        0056.5656.5656  100.0.0.201        Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.103        a288.0103.0001  100.0.0.56         -   
1304  1304   VXLAN 10.30.4.103        a288.0103.0001  100.0.0.201        -   
1304  1304   VXLAN 10.30.4.254        00aa.aaaa.aaaa  100.0.0.56         Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.254        00aa.aaaa.aaaa  100.0.0.201        Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.203        001b.0100.0003  100.0.30.14        -   
0     2303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.30.14        Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.254        0056.5656.5656  100.0.30.14        Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.0.56         Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.254        0056.5656.5656  100.0.0.56         Stic
                                                                         ky  
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

 I L2     20.22.205.0/24 [115/20]
           via 20.202.205.205, Ethernet10
 I L2     20.22.206.0/24 [115/30]
           via 20.202.205.205, Ethernet10
 B E      20.42.200.0/24 [20/0]
           via 20.200.202.200, Ethernet1
 I L2     20.45.205.0/24 [115/20]
           via 20.202.205.205, Ethernet10
 I L2     20.46.205.0/24 [115/20]
           via 20.202.205.205, Ethernet10
 I L2     20.56.205.0/24 [115/20]
           via 20.202.205.205, Ethernet10
 B E      20.103.200.0/24 [20/0]
           via 20.200.202.200, Ethernet1
 B E      20.200.201.0/24 [20/0]
           via 20.200.202.200, Ethernet1
 C        20.200.202.0/24
           directly connected, Ethernet1
 B E      20.200.203.0/24 [20/0]
           via 20.200.202.200, Ethernet1
 B E      20.200.204.0/24 [20/0]
           via 20.200.202.200, Ethernet1
 B E      20.201.205.0/24 [20/0]
           via 20.200.202.200, Ethernet1
 C        20.202.205.0/24
           directly connected, Ethernet10
 B E      30.14.200.0/24 [20/0]
           via 20.200.202.200, Ethernet1
 I L2     100.0.0.22/32 [115/20]
           via 20.202.205.205, Ethernet10
 I L2     100.0.0.56/32 [115/20]
           via 20.202.205.205, Ethernet10
 B E      100.0.0.200/32 [20/0]
           via 20.200.202.200, Ethernet1
 B E      100.0.0.201/32 [20/0]
           via 20.200.202.200, Ethernet1
 C        100.0.0.202/32
           directly connected, Loopback0
 B E      100.0.0.203/32 [20/0]
           via 20.200.202.200, Ethernet1
 B E      100.0.0.204/32 [20/0]
           via 20.200.202.200, Ethernet1
 I L2     100.0.0.205/32 [115/10]
           via 20.202.205.205, Ethernet10
 B E      100.0.30.14/32 [20/0]
           via 20.200.202.200, Ethernet1

```

## show ip arp

```text
Address         Age (sec)  Hardware Addr   Interface
20.200.202.200    0:00:19  444c.a873.5c75  Ethernet1
20.202.205.205    0:00:19  444c.a873.a0ad  Ethernet10
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

 I L2     20.22.205.0/24 [115/20]
           via 20.202.205.205, Ethernet10
 I L2     20.22.206.0/24 [115/30]
           via 20.202.205.205, Ethernet10
 B E      20.42.200.0/24 [20/0]
           via 20.200.202.200, Ethernet1
 I L2     20.45.205.0/24 [115/20]
           via 20.202.205.205, Ethernet10
 I L2     20.46.205.0/24 [115/20]
           via 20.202.205.205, Ethernet10
 I L2     20.56.205.0/24 [115/20]
           via 20.202.205.205, Ethernet10
 B E      20.103.200.0/24 [20/0]
           via 20.200.202.200, Ethernet1
 B E      20.200.201.0/24 [20/0]
           via 20.200.202.200, Ethernet1
 C        20.200.202.0/24
           directly connected, Ethernet1
 B E      20.200.203.0/24 [20/0]
           via 20.200.202.200, Ethernet1
 B E      20.200.204.0/24 [20/0]
           via 20.200.202.200, Ethernet1
 B E      20.201.205.0/24 [20/0]
           via 20.200.202.200, Ethernet1
 C        20.202.205.0/24
           directly connected, Ethernet10
 B E      30.14.200.0/24 [20/0]
           via 20.200.202.200, Ethernet1
 I L2     100.0.0.22/32 [115/20]
           via 20.202.205.205, Ethernet10
 I L2     100.0.0.56/32 [115/20]
           via 20.202.205.205, Ethernet10
 B E      100.0.0.200/32 [20/0]
           via 20.200.202.200, Ethernet1
 B E      100.0.0.201/32 [20/0]
           via 20.200.202.200, Ethernet1
 C        100.0.0.202/32
           directly connected, Loopback0
 B E      100.0.0.203/32 [20/0]
           via 20.200.202.200, Ethernet1
 B E      100.0.0.204/32 [20/0]
           via 20.200.202.200, Ethernet1
 I L2     100.0.0.205/32 [115/10]
           via 20.202.205.205, Ethernet10
 B E      100.0.30.14/32 [20/0]
           via 20.200.202.200, Ethernet1


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

 B I      10.10.103.0/24 [200/0]
           via VTEP 100.0.0.56 VNI 1000 router-mac 00:01:00:00:00:56
 C        10.10.201.0/24
           directly connected, Vlan1201
 B E      10.10.203.203/32 [20/0]
           via VTEP 100.0.0.204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 100.0.0.203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 B E      10.10.203.0/24 [20/0]
           via VTEP 100.0.0.204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 100.0.0.203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 B I      10.30.1.103/32 [200/0]
           via VTEP 100.0.0.56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      10.30.1.201/32 [20/0]
           via VTEP 100.0.0.204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 100.0.0.203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 B E      10.30.1.203/32 [20/0]
           via VTEP 100.0.0.204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 100.0.0.203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 C        10.30.1.0/24
           directly connected, Vlan1301
 C        10.30.2.0/24
           directly connected, Vlan1302
 B I      10.30.3.103/32 [200/0]
           via VTEP 100.0.0.56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      10.30.3.203/32 [20/0]
           via VTEP 100.0.0.204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 100.0.0.203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 C        10.30.3.0/24
           directly connected, Vlan1303
 B I      10.30.4.103/32 [200/0]
           via VTEP 100.0.0.56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      10.30.4.203/32 [20/0]
           via VTEP 100.0.0.204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 100.0.0.203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 C        10.30.4.0/24
           directly connected, Vlan1304
 B E      100.0.1.203/32 [20/0]
           via VTEP 100.0.0.203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 B E      100.0.1.204/32 [20/0]
           via VTEP 100.0.0.204 VNI 1000 router-mac 98:5d:82:a2:04:f9

```

## show ip arp vrf all

```text

VRF: PIM
Address         Age (sec)  Hardware Addr   Interface

VRF: default
Address         Age (sec)  Hardware Addr   Interface
20.200.202.200    0:00:20  444c.a873.5c75  Ethernet1
20.202.205.205    0:00:19  444c.a873.a0ad  Ethernet10

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.20.2      0:03:53  bcea.fa02.6ce2  Management1
192.168.20.19     0:00:14  c407.7858.8001  Management1
192.168.20.20     0:01:21  e484.29d0.4001  Management1
192.168.20.21     0:01:15  7081.85c1.b801  Management1
192.168.20.22     0:02:22  c407.780a.9f04  Management1
192.168.20.23     0:00:39  c407.780a.7750  Management1
192.168.20.24     0:00:08  6c87.2089.ede5  Management1
192.168.20.26     0:02:04  04a9.59d5.df66  Management1
192.168.20.27     0:04:36  04a9.59d5.dfe6  Management1
192.168.20.28     0:01:21  98a9.2d59.bae6  Management1
192.168.20.29     0:03:23  90f7.b223.d466  Management1
192.168.20.52     0:03:47  f83e.95dc.1289  Management1
192.168.21.47     0:03:47  5c5a.c7ff.8a0a  Management1
192.168.21.50     0:03:47  a84f.b1a5.5221  Management1
192.168.21.59     0:02:40  6607.f5d1.ae16  Management1

VRF: tenant-a
Address         Age (sec)  Hardware Addr   Interface
10.30.1.103             -  a244.0101.0001  Vlan1301, Vxlan1
10.30.1.201             -  001b.0100.0002  Vlan1301, Vxlan1
10.30.1.203             -  001b.0100.0002  Vlan1301, Vxlan1
10.30.3.103             -  a266.0102.0001  Vlan1303, Vxlan1
10.30.3.203             -  001b.0100.0003  Vlan1303, Vxlan1
10.30.4.103             -  a288.0103.0001  Vlan1304, Vxlan1
10.30.4.203             -  001b.0100.0004  Vlan1304, Vxlan1
```

## show vxlan address-table

```text
          Vxlan Mac Address Table
----------------------------------------------------------------------

VLAN  Mac Address     Type      Prt  VTEP             Moves   Last Move
----  -----------     ----      ---  ----             -----   ---------
1301  001b.0100.0002  EVPN      Vx1  100.0.0.203      1       3:09:34 ago
                                     100.0.0.204    
1301  0056.5656.5656  EVPN      Vx1  100.0.0.56       1       14:43:55 ago
1301  00cc.cccc.bbbb  EVPN      Vx1  100.0.0.203      1       14:43:54 ago
                                     100.0.0.204    
1301  a244.0101.0001  EVPN      Vx1  100.0.0.56       1       0:35:37 ago
1303  001b.0100.0003  EVPN      Vx1  100.0.0.203      1       3:01:45 ago
                                     100.0.0.204    
1303  0056.5656.5656  EVPN      Vx1  100.0.0.56       1       14:43:55 ago
1303  a266.0102.0001  EVPN      Vx1  100.0.0.56       1       0:35:37 ago
1304  001b.0100.0004  EVPN      Vx1  100.0.0.203      1       2:36:40 ago
                                     100.0.0.204    
1304  0056.5656.5656  EVPN      Vx1  100.0.0.56       1       14:43:55 ago
1304  a288.0103.0001  EVPN      Vx1  100.0.0.56       1       0:35:37 ago
Total Remote Mac Addresses for this criterion: 10
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
1301    001b.0100.0002    DYNAMIC     Vx1        1       3:09:34 ago
1301    0056.5656.5656    STATIC      Vx1
1301    00aa.aaaa.aaaa    STATIC      Router
1301    00cc.cccc.bbbb    STATIC      Vx1
1301    2cdd.e90b.25b7    STATIC      Router
1301    a244.0101.0001    DYNAMIC     Vx1        1       0:35:37 ago
1302    00aa.aaaa.aaaa    STATIC      Router
1302    2cdd.e90b.25b7    STATIC      Router
1303    001b.0100.0003    DYNAMIC     Vx1        1       3:01:46 ago
1303    0056.5656.5656    STATIC      Vx1
1303    00aa.aaaa.aaaa    STATIC      Router
1303    2cdd.e90b.25b7    STATIC      Router
1303    a266.0102.0001    DYNAMIC     Vx1        1       0:35:37 ago
1304    001b.0100.0004    DYNAMIC     Vx1        1       2:36:40 ago
1304    0056.5656.5656    STATIC      Vx1
1304    00aa.aaaa.aaaa    STATIC      Router
1304    2cdd.e90b.25b7    STATIC      Router
1304    a288.0103.0001    DYNAMIC     Vx1        1       0:35:37 ago
4092    00aa.aaaa.aaaa    STATIC      Router
4092    2cdd.e90b.25b7    STATIC      Router
Total Mac Addresses for this criterion: 24

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
00aa.aaaa.aaaa, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
0056.5656.5656, VLAN 1303, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
00aa.aaaa.aaaa, VLAN 1303, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
0056.5656.5656, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
00cc.cccc.bbbb, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 13: 2-way
      VTEP 100.0.0.203
      VTEP 100.0.0.204
a288.0103.0001, VLAN 1304, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.56
a244.0101.0001, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.56
00aa.aaaa.aaaa, VLAN 1304, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
001b.0100.0004, VLAN 1304, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 13: 2-way
      VTEP 100.0.0.203
      VTEP 100.0.0.204
001b.0100.0003, VLAN 1303, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 13: 2-way
      VTEP 100.0.0.203
      VTEP 100.0.0.204
0056.5656.5656, VLAN 1304, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
a266.0102.0001, VLAN 1303, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.56
001b.0100.0002, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 13: 2-way
      VTEP 100.0.0.203
      VTEP 100.0.0.204
```

## show vxlan flood vtep domain local

```text
          VXLAN Flood VTEP Table
--------------------------------------------------------------------------------

VLANS                            Ip Address
-----------------------------   ------------------------------------------------
1201                            100.0.0.201    
1301,1303-1304                  100.0.0.203     100.0.0.204    
1302                            100.0.0.201     100.0.0.203     100.0.0.204    
```

## show vxlan flood vtep domain remote

```text
          VXLAN Flood VTEP Table
--------------------------------------------------------------------------------

VLANS                            Ip Address
-----------------------------   ------------------------------------------------
1301,1303-1304                  100.0.0.56      100.0.0.201    
```

## show bgp evpn domain remote detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 1303 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1303
BGP routing table entry for auto-discovery 1303 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1304
BGP routing table entry for auto-discovery 1304 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.201:2
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      Rx path id: 0x1
      VNI: 0
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:2
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65205:1301 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
BGP routing table entry for auto-discovery 0 0000:2222:2222:2222:1111 remote, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1301
BGP routing table entry for auto-discovery 1303 0000:2222:2222:2222:1111 remote, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1303
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111 remote, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      Rx path id: 0x1
      VNI: 0
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111 remote, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      Rx path id: 0x1
      VNI: 0
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111 remote, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      Rx path id: 0x1
      VNI: 0
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111 remote, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      Rx path id: 0x1
      VNI: 0
BGP routing table entry for mac-ip 001b.0100.0002 remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.201 remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:51301:51301 Route-Target-AS:65300:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.201 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.203 remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:51301:51301 Route-Target-AS:65300:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.203 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 0056.5656.5656 10.10.103.254 remote, Route Distinguisher: 100.0.0.56:1103
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1103 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.30.1.254 remote, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.30.2.254 remote, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1302:1302 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.103.254 remote, Route Distinguisher: 100.0.0.56:1103
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1103 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.203.254 remote, Route Distinguisher: 100.0.0.56:1203
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1203:1203 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1203 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254 remote, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00cc.cccc.bbbb remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 00cc.cccc.bbbb remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip a244.0101.0001 10.30.1.103 remote, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 001b.0100.0003 remote, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0003 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203 remote, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:51301:51301 Route-Target-AS:65300:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254 remote, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254 remote, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 a266.0102.0001 10.30.3.103 remote, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1303 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1304 001b.0100.0004 remote, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0004 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0004 10.30.4.203 remote, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:51301:51301 Route-Target-AS:65300:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0004 10.30.4.203 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254 remote, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254 remote, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      Rx path id: 0x1
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 a288.0103.0001 10.30.4.103 remote, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for imet 100.0.0.56 remote, Route Distinguisher: 100.0.0.56:1103
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1103
      PMSI Tunnel: Ingress Replication, MPLS Label: 1103, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.56 remote, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.201 remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1303 100.0.0.56 remote, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1303 100.0.0.201 remote, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1303 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1304 100.0.0.56 remote, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1304 100.0.0.201 remote, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      Rx path id: 0x1
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1304 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for ethernet-segment 0000:0000:0000:0111:0111 100.0.0.56 remote, Route Distinguisher: 100.0.0.56:0
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:00:00:00:00:00:01
      Rx path id: 0x1
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.201 remote, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:01:11:11:11 DF Election: Preference 100
      Rx path id: 0x1
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:01:11:11:11 DF Election: Preference 150
BGP routing table entry for ethernet-segment 0000:2222:2222:2222:1111 100.0.0.56 remote, Route Distinguisher: 100.0.0.56:0
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:00:22:22:22:22:22
      Rx path id: 0x1
BGP routing table entry for ethernet-segment 0048:5648:5648:5648:5648 100.0.0.56 remote, Route Distinguisher: 100.0.0.56:0
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:48:56:48:56:48:56
      Rx path id: 0x1
BGP routing table entry for ip-prefix 10.10.103.0/24 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.10.201.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.201.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.203/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.203/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.0/24 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.1.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 3 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.103/32 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.1.201/32 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.1.201/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.201/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.203/32 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.1.203/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.203/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.2.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 3 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.0/24 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.3.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 3 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.103/32 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.3.203/32 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.3.203/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.203/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.0/24 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.4.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 3 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.103/32 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.4.203/32 remote, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local
    100.0.0.56 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.56, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.4.203/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.203/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.203/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.203/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.204/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204
    100.0.0.201 from 100.0.0.205 (100.0.0.205)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.201, Cluster list: 100.0.0.205 
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      Rx path id: 0x1
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.204/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
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
      ES-Import RT: 00:00:01:11:11:11
      DF election algorithm: preference
      Designated forwarder: 100.0.0.202
      Non-Designated forwarder: 100.0.0.201
EVPN instance: VLAN 1301
  Route distinguisher: 100.0.0.202:1301
  Route distinguisher remote: 100.0.0.202:1301
  Route target import: Route-Target-AS:1301:1301
  Route target export: Route-Target-AS:1301:1301
  Route target import remote: Route-Target-AS:65205:1301
  Route target export remote: Route-Target-AS:65205:1301
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.202
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:0000:0000:0203:0204
    Active TEPs: 100.0.0.203, 100.0.0.204
    ESI: 0000:2222:2222:2222:1111
    Active TEPs: 100.0.0.56
  Local ethernet segment:
    ESI: 0000:1111:1111:1111:1111
      Interface: Vxlan1
      Mode: all-active
      State: up
      ES-Import RT: 00:00:01:11:11:11
      DF election algorithm: preference
      Designated forwarder: 100.0.0.202
      Non-Designated forwarder: 100.0.0.201
EVPN instance: VLAN 1302
  Route distinguisher: 100.0.0.202:1302
  Route target import: Route-Target-AS:1302:1302
  Route target export: Route-Target-AS:1302:1302
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.202
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:0000:0000:0203:0204
    Active TEPs: 100.0.0.203, 100.0.0.204
  Local ethernet segment:
    ESI: 0000:1111:1111:1111:1111
      Interface: Vxlan1
      Mode: all-active
      State: up
      ES-Import RT: 00:00:01:11:11:11
      DF election algorithm: preference
      Designated forwarder: 100.0.0.202
      Non-Designated forwarder: 100.0.0.201
EVPN instance: VLAN-aware bundle 1303-1304
  Route distinguisher: 100.0.0.202:1303
  Route distinguisher remote: 100.0.0.202:1303
  Route target import: Route-Target-AS:1303:1303
  Route target export: Route-Target-AS:1303:1303
  Route target import remote: Route-Target-AS:65205:1303
  Route target export remote: Route-Target-AS:65205:1303
  Service interface: VLAN-aware bundle
  Local VXLAN IP address: 100.0.0.202
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:0000:0000:0203:0204
    Active TEPs: 100.0.0.203, 100.0.0.204
    ESI: 0000:2222:2222:2222:1111
    Active TEPs: 100.0.0.56
  Local ethernet segment:
    ESI: 0000:1111:1111:1111:1111
      Interface: Vxlan1
      Mode: all-active
      State: up
      ES-Import RT: 00:00:01:11:11:11
      DF election algorithm: preference
      Designated forwarder: 100.0.0.202
      Non-Designated forwarder: 100.0.0.201
```

## show interfaces counters rates | nz

```text
Port      Name         Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Et1       A-Spine-200   0:01      1.9   0.0%        2      0.0   0.0%        0
Et10      SPINE_REMOTE  0:05      0.0   0.0%        0      1.9   0.0%        2
Ma1                     0:05      0.0   0.0%        0      0.2   0.0%        0
```

