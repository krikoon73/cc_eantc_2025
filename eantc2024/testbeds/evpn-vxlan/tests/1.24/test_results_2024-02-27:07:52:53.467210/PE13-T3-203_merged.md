# Test results for PE13-T3-203

## show hostname

```text
Hostname: PE13-T3-203
FQDN:     PE13-T3-203.ns.eantc.de
```

## show ip bgp summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.203, local AS number 65203
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor       V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  ANET.IPV4                20.200.203.200 4 65000           1831      1761    0    0 21:24:56 Estab   14     14
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.203, local AS number 65203
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  ANET.EVPN                100.0.0.200 4 65000           4081      2770    0    0 21:24:55 Estab   639    639
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1203:1203 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
BGP routing table entry for mac-ip 001b.0100.0001, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0001 10.10.203.203, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1203 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0002, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0002, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.201, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.203, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0033, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0033, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0034, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0034 10.30.1.202, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0034 10.30.1.202, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0035, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0036, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0036, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0036 10.30.1.204, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0036 10.30.1.204, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0037, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0037 10.30.1.205, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0037 10.30.1.205, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0038, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0038 10.30.1.206, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0038 10.30.1.206, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0039, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0039 10.30.1.207, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0039 10.30.1.207, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003a, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003a 10.30.1.208, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003a 10.30.1.208, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003b, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003b 10.30.1.209, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003b 10.30.1.209, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003c, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003c 10.30.1.210, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003c 10.30.1.210, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003d, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003d 10.30.1.211, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003d 10.30.1.211, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003e, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003e, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003e 10.30.1.212, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003e 10.30.1.212, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003f, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003f 10.30.1.213, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.003f 10.30.1.213, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0040, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0040 10.30.1.214, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0040 10.30.1.214, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0041, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0041 10.30.1.215, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0041 10.30.1.215, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0042, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0042 10.30.1.216, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0042 10.30.1.216, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0043, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0043 10.30.1.217, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0043 10.30.1.217, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0044, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0044 10.30.1.218, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0044 10.30.1.218, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0045, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0045 10.30.1.219, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0045 10.30.1.219, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0046, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0046 10.30.1.220, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0046 10.30.1.220, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0047, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0047 10.30.1.221, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0047 10.30.1.221, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0048, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0048 10.30.1.222, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0048 10.30.1.222, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0049, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0049 10.30.1.223, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0049 10.30.1.223, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004a, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004a 10.30.1.224, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004a 10.30.1.224, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004b, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004b 10.30.1.225, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004b 10.30.1.225, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004c, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004c, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004c 10.30.1.226, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004c 10.30.1.226, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004d, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004d 10.30.1.227, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004d 10.30.1.227, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004e, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004e, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004e 10.30.1.228, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004e 10.30.1.228, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004f, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004f 10.30.1.229, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.004f 10.30.1.229, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0050, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0050, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0050 10.30.1.230, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0050 10.30.1.230, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0051, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0051 10.30.1.231, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0051 10.30.1.231, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0052, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0052 10.30.1.232, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0052 10.30.1.232, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0053, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0053 10.30.1.233, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0053 10.30.1.233, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0054, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0054 10.30.1.234, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0054 10.30.1.234, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0055, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0055 10.30.1.235, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0055 10.30.1.235, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0056, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0056 10.30.1.236, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0056 10.30.1.236, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0057, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0057 10.30.1.237, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0057 10.30.1.237, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0058, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0058 10.30.1.238, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0058 10.30.1.238, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0059, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0059, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0059 10.30.1.239, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0059 10.30.1.239, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005a, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005a 10.30.1.240, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005a 10.30.1.240, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005b, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005b 10.30.1.241, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005b 10.30.1.241, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005c, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005c 10.30.1.242, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005c 10.30.1.242, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005d, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005d 10.30.1.243, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005d 10.30.1.243, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005e, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005e, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005e 10.30.1.244, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005e 10.30.1.244, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005f, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005f 10.30.1.245, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.005f 10.30.1.245, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0060, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0060, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0060 10.30.1.246, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0060 10.30.1.246, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0061, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0061 10.30.1.247, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0061 10.30.1.247, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0062, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0062 10.30.1.248, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0062 10.30.1.248, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0063, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0063 10.30.1.249, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0063 10.30.1.249, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0064, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0064 10.30.1.250, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0064 10.30.1.250, Route Distinguisher: 100.0.0.204:1301
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 00cc.cccc.bbbb, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0003, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0065, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0065, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0065 10.30.3.201, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0065 10.30.3.201, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0066, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0066 10.30.3.202, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0066 10.30.3.202, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0067, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0068, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0068 10.30.3.204, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0068 10.30.3.204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0069, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0069 10.30.3.205, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0069 10.30.3.205, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006a, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006a 10.30.3.206, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006a 10.30.3.206, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006b, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006b 10.30.3.207, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006b 10.30.3.207, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006c, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006c 10.30.3.208, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006c 10.30.3.208, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006d, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006d 10.30.3.209, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006d 10.30.3.209, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006e, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006e 10.30.3.210, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006e 10.30.3.210, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006f, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006f 10.30.3.211, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.006f 10.30.3.211, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0070, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0070 10.30.3.212, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0070 10.30.3.212, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0071, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0071 10.30.3.213, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0071 10.30.3.213, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0072, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0072 10.30.3.214, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0072 10.30.3.214, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0073, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0073, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0073 10.30.3.215, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0073 10.30.3.215, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0074, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0074, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0074 10.30.3.216, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0074 10.30.3.216, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0075, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0075 10.30.3.217, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0075 10.30.3.217, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0076, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0076 10.30.3.218, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0076 10.30.3.218, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0077, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0077 10.30.3.219, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0077 10.30.3.219, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0078, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0078 10.30.3.220, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0078 10.30.3.220, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0079, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0079 10.30.3.221, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0079 10.30.3.221, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007a, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007a 10.30.3.222, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007a 10.30.3.222, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007b, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007b 10.30.3.223, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007b 10.30.3.223, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007c, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007c 10.30.3.224, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007c 10.30.3.224, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007d, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007d 10.30.3.225, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007d 10.30.3.225, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007e, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007e 10.30.3.226, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007e 10.30.3.226, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007f, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007f 10.30.3.227, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.007f 10.30.3.227, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0080, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0080 10.30.3.228, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0080 10.30.3.228, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0081, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0081 10.30.3.229, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0081 10.30.3.229, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0082, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0082 10.30.3.230, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0082 10.30.3.230, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0083, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0083 10.30.3.231, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0083 10.30.3.231, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0084, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0084 10.30.3.232, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0084 10.30.3.232, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0085, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0085 10.30.3.233, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0085 10.30.3.233, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0086, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0086 10.30.3.234, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0086 10.30.3.234, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0087, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0087, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0087 10.30.3.235, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0087 10.30.3.235, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0088, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0088 10.30.3.236, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0088 10.30.3.236, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0089, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0089 10.30.3.237, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0089 10.30.3.237, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008a, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008a 10.30.3.238, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008a 10.30.3.238, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008b, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008b 10.30.3.239, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008b 10.30.3.239, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008c, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008c 10.30.3.240, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008c 10.30.3.240, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008d, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008d 10.30.3.241, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008d 10.30.3.241, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008e, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008e 10.30.3.242, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008e 10.30.3.242, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008f, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008f 10.30.3.243, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.008f 10.30.3.243, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0090, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0090 10.30.3.244, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0090 10.30.3.244, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0091, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0091 10.30.3.245, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0091 10.30.3.245, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0092, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0092 10.30.3.246, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0092 10.30.3.246, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0093, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0093 10.30.3.247, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0093 10.30.3.247, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0094, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0094, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0094 10.30.3.248, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0094 10.30.3.248, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0095, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0095 10.30.3.249, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0095 10.30.3.249, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0096, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0096 10.30.3.250, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 001b.0100.0096 10.30.3.250, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0004, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.0004, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.0004 10.30.4.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.0004 10.30.4.203, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.0097, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.0097 10.30.4.201, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.0097 10.30.4.201, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.0098, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.0098, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.0098 10.30.4.202, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.0098 10.30.4.202, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.0099, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009a, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009a 10.30.4.204, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009a 10.30.4.204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009b, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009b 10.30.4.205, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009b 10.30.4.205, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009c, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009c 10.30.4.206, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009c 10.30.4.206, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009d, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009d 10.30.4.207, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009d 10.30.4.207, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009e, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009e 10.30.4.208, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009e 10.30.4.208, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009f, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009f, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009f 10.30.4.209, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.009f 10.30.4.209, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a0, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a0 10.30.4.210, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a0 10.30.4.210, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a1, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a1, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a1 10.30.4.211, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a1 10.30.4.211, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a2, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a2 10.30.4.212, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a2 10.30.4.212, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a3, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a3, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a3 10.30.4.213, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a3 10.30.4.213, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a4, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a4 10.30.4.214, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a4 10.30.4.214, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a5, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a5 10.30.4.215, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a5 10.30.4.215, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a6, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a6 10.30.4.216, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a6 10.30.4.216, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a7, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a7 10.30.4.217, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a7 10.30.4.217, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a8, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a8 10.30.4.218, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a8 10.30.4.218, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a9, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a9 10.30.4.219, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00a9 10.30.4.219, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00aa, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00aa, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00aa 10.30.4.220, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00aa 10.30.4.220, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ab, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ab, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ab 10.30.4.221, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ab 10.30.4.221, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ac, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ac, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ac 10.30.4.222, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ac 10.30.4.222, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ad, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ad, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ad 10.30.4.223, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ad 10.30.4.223, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ae, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ae 10.30.4.224, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ae 10.30.4.224, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00af, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00af 10.30.4.225, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00af 10.30.4.225, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b0, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b0 10.30.4.226, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b0 10.30.4.226, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b1, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b1, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b1 10.30.4.227, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b1 10.30.4.227, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b2, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b2 10.30.4.228, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b2 10.30.4.228, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b3, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b3, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b3 10.30.4.229, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b3 10.30.4.229, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b4, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b4 10.30.4.230, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b4 10.30.4.230, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b5, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b5 10.30.4.231, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b5 10.30.4.231, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b6, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b6 10.30.4.232, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b6 10.30.4.232, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b7, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b7 10.30.4.233, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b7 10.30.4.233, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b8, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b8, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b8 10.30.4.234, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b8 10.30.4.234, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b9, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b9, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b9 10.30.4.235, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00b9 10.30.4.235, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ba, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ba 10.30.4.236, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00ba 10.30.4.236, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00bb, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00bb 10.30.4.237, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00bb 10.30.4.237, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00bc, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00bc 10.30.4.238, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00bc 10.30.4.238, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00bd, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00bd 10.30.4.239, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00bd 10.30.4.239, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00be, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00be 10.30.4.240, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00be 10.30.4.240, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00bf, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00bf, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00bf 10.30.4.241, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00bf 10.30.4.241, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c0, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c0 10.30.4.242, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c0 10.30.4.242, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c1, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c1, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c1 10.30.4.243, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c1 10.30.4.243, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c2, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c2 10.30.4.244, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c2 10.30.4.244, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c3, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c3 10.30.4.245, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c3 10.30.4.245, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c4, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c4 10.30.4.246, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c4 10.30.4.246, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c5, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c5 10.30.4.247, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c5 10.30.4.247, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c6, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c6, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c6 10.30.4.248, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c6 10.30.4.248, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c7, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c7 10.30.4.249, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c7 10.30.4.249, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c8, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c8 10.30.4.250, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 001b.0100.00c8 10.30.4.250, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
```

## show bgp evpn route-type imet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
      PMSI Tunnel: Ingress Replication, MPLS Label: 1201, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 100.0.0.202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 100.0.0.202, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 100.0.0.203, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan Multicast Flags: IGMP proxy, OISM-supported, SBD
      VNI: 1000
      PMSI Tunnel: Ingress Replication, MPLS Label: 1000, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 100.0.0.203, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
      PMSI Tunnel: Ingress Replication, MPLS Label: 1203, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 100.0.0.203, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 100.0.0.203, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1303 100.0.0.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1304 100.0.0.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
BGP routing table entry for ethernet-segment 0000:0000:0000:0203:0204 100.0.0.203, Route Distinguisher: 100.0.0.203:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:01:11:11:11 DF Election: Preference 150
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
BGP routing table entry for ip-prefix 10.10.103.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.10.103.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.10.103.103/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.10.103.103/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
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
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.103/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.201/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.201/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.202/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.202/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.204/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.204/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.205/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.205/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.206/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.206/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.207/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.207/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.208/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.208/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.209/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.209/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.210/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.210/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.211/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.211/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.212/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.212/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.213/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.213/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.214/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.214/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.215/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.215/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.216/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.216/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.217/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.217/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.218/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.218/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.219/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.219/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.220/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.220/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.221/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.221/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.222/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.222/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.223/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.223/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.224/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.224/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.225/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.225/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.226/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.226/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.227/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.227/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.228/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.228/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.229/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.229/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.230/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.230/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.231/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.231/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.232/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.232/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.233/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.233/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.234/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.234/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.235/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.235/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.236/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.236/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.237/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.237/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.238/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.238/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.239/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.239/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.240/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.240/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.241/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.241/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.242/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.242/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.243/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.243/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.244/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.244/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.245/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.245/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.246/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.246/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.247/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.247/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.248/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.248/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.249/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.249/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.250/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.1.250/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
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
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
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
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.103/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.201/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.201/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.202/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.202/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.204/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.204/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.205/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.205/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.206/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.206/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.207/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.207/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.208/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.208/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.209/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.209/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.210/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.210/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.211/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.211/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.212/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.212/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.213/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.213/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.214/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.214/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.215/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.215/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.216/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.216/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.217/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.217/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.218/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.218/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.219/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.219/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.220/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.220/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.221/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.221/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.222/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.222/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.223/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.223/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.224/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.224/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.225/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.225/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.226/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.226/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.227/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.227/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.228/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.228/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.229/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.229/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.230/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.230/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.231/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.231/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.232/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.232/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.233/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.233/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.234/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.234/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.235/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.235/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.236/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.236/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.237/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.237/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.238/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.238/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.239/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.239/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.240/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.240/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.241/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.241/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.242/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.242/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.243/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.243/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.244/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.244/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.245/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.245/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.246/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.246/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.247/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.247/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.248/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.248/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.249/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.249/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.250/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.250/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
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
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.103/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.201/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.201/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.202/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.202/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.204/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.204/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.205/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.205/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.206/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.206/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.207/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.207/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.208/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.208/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.209/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.209/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.210/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.210/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.211/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.211/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.212/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.212/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.213/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.213/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.214/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.214/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.215/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.215/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.216/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.216/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.217/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.217/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.218/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.218/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.219/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.219/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.220/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.220/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.221/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.221/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.222/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.222/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.223/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.223/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.224/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.224/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.225/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.225/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.226/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.226/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.227/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.227/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.228/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.228/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.229/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.229/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.230/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.230/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.231/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.231/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.232/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.232/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.233/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.233/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.234/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.234/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.235/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.235/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.236/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.236/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.237/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.237/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.238/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.238/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.239/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.239/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.240/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.240/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.241/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.241/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.242/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.242/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.243/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.243/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.244/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.244/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.245/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.245/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.246/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.246/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.247/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.247/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.248/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.248/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.249/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.249/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.250/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.250/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 100.0.1.203/32, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 100.0.1.204/32, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
```

## show bgp evpn route-type smet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
```

## show bgp evpn route-type spmsi detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
```

## show bgp evpn arp

```text
VLAN  Label  Encap IP                 MAC             Tunnel Endpoint    Seq#
----- ------ ----- ------------------ --------------- ------------------ ----
1203  1203   VXLAN 10.10.203.203      001b.0100.0001  Local              -   
1203  1203   VXLAN 10.10.203.203      001b.0100.0001  100.0.0.204        -   
1203  1203   VXLAN 10.10.203.203      001b.0100.0001  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.201        001b.0100.0002  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.209        001b.0100.003b  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.205        001b.0100.0037  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.226        001b.0100.004c  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.249        001b.0100.0063  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.246        001b.0100.0060  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.218        001b.0100.0044  Local              -   
1301  1301   VXLAN 10.30.1.218        001b.0100.0044  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.203        001b.0100.0002  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.239        001b.0100.0059  Local              -   
1301  1301   VXLAN 10.30.1.239        001b.0100.0059  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.254        00aa.aaaa.aaaa  100.0.0.201        Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.254        00aa.aaaa.aaaa  100.0.0.202        Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.221        001b.0100.0047  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.204        001b.0100.0036  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.204        001b.0100.0036  Local              -   
1301  1301   VXLAN 10.30.1.234        001b.0100.0054  Local              -   
1301  1301   VXLAN 10.30.1.234        001b.0100.0054  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.205        001b.0100.0037  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.205        001b.0100.0037  Local              -   
1301  1301   VXLAN 10.30.1.240        001b.0100.005a  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.203        001b.0100.0035  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.221        001b.0100.0047  Local              -   
1301  1301   VXLAN 10.30.1.221        001b.0100.0047  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.216        001b.0100.0042  Local              -   
1301  1301   VXLAN 10.30.1.216        001b.0100.0042  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.209        001b.0100.003b  Local              -   
1301  1301   VXLAN 10.30.1.209        001b.0100.003b  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.245        001b.0100.005f  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.235        001b.0100.0055  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.246        001b.0100.0060  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.246        001b.0100.0060  Local              -   
1301  1301   VXLAN 10.30.1.239        001b.0100.0059  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.228        001b.0100.004e  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.211        001b.0100.003d  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.242        001b.0100.005c  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.242        001b.0100.005c  Local              -   
1301  1301   VXLAN 10.30.1.207        001b.0100.0039  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.229        001b.0100.004f  Local              -   
1301  1301   VXLAN 10.30.1.229        001b.0100.004f  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.241        001b.0100.005b  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.237        001b.0100.0057  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.237        001b.0100.0057  Local              -   
1301  1301   VXLAN 10.30.1.224        001b.0100.004a  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.225        001b.0100.004b  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.202        001b.0100.0034  Local              -   
1301  1301   VXLAN 10.30.1.202        001b.0100.0034  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.244        001b.0100.005e  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.235        001b.0100.0055  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.235        001b.0100.0055  Local              -   
1301  1301   VXLAN 10.30.1.217        001b.0100.0043  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.231        001b.0100.0051  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.232        001b.0100.0052  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.206        001b.0100.0038  Local              -   
1301  1301   VXLAN 10.30.1.206        001b.0100.0038  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.201        001b.0100.0002  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.201        001b.0100.0002  Local              -   
1301  1301   VXLAN 10.30.1.213        001b.0100.003f  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.238        001b.0100.0058  Local              -   
1301  1301   VXLAN 10.30.1.238        001b.0100.0058  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.103        a244.0101.0001  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.103        a244.0101.0001  100.0.0.202        -   
1301  1301   VXLAN 10.30.1.219        001b.0100.0045  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.229        001b.0100.004f  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.245        001b.0100.005f  Local              -   
1301  1301   VXLAN 10.30.1.245        001b.0100.005f  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.203        001b.0100.0002  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.203        001b.0100.0002  Local              -   
1301  1301   VXLAN 10.30.1.208        001b.0100.003a  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.222        001b.0100.0048  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.248        001b.0100.0062  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.250        001b.0100.0064  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.250        001b.0100.0064  Local              -   
1301  1301   VXLAN 10.30.1.213        001b.0100.003f  Local              -   
1301  1301   VXLAN 10.30.1.213        001b.0100.003f  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.231        001b.0100.0051  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.231        001b.0100.0051  Local              -   
1301  1301   VXLAN 10.30.1.243        001b.0100.005d  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.233        001b.0100.0053  Local              -   
1301  1301   VXLAN 10.30.1.233        001b.0100.0053  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.247        001b.0100.0061  Local              -   
1301  1301   VXLAN 10.30.1.247        001b.0100.0061  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.238        001b.0100.0058  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.212        001b.0100.003e  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.212        001b.0100.003e  Local              -   
1301  1301   VXLAN 10.30.1.249        001b.0100.0063  Local              -   
1301  1301   VXLAN 10.30.1.249        001b.0100.0063  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.241        001b.0100.005b  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.241        001b.0100.005b  Local              -   
1301  1301   VXLAN 10.30.1.207        001b.0100.0039  Local              -   
1301  1301   VXLAN 10.30.1.207        001b.0100.0039  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.214        001b.0100.0040  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.214        001b.0100.0040  Local              -   
1301  1301   VXLAN 10.30.1.218        001b.0100.0044  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.206        001b.0100.0038  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.236        001b.0100.0056  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.222        001b.0100.0048  Local              -   
1301  1301   VXLAN 10.30.1.222        001b.0100.0048  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.234        001b.0100.0054  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.212        001b.0100.003e  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.250        001b.0100.0064  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.215        001b.0100.0041  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.243        001b.0100.005d  Local              -   
1301  1301   VXLAN 10.30.1.243        001b.0100.005d  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.208        001b.0100.003a  Local              -   
1301  1301   VXLAN 10.30.1.208        001b.0100.003a  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.237        001b.0100.0057  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.220        001b.0100.0046  Local              -   
1301  1301   VXLAN 10.30.1.220        001b.0100.0046  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.240        001b.0100.005a  Local              -   
1301  1301   VXLAN 10.30.1.240        001b.0100.005a  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.233        001b.0100.0053  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.248        001b.0100.0062  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.248        001b.0100.0062  Local              -   
1301  1301   VXLAN 10.30.1.201        001b.0100.0033  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.204        001b.0100.0036  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.244        001b.0100.005e  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.244        001b.0100.005e  Local              -   
1301  1301   VXLAN 10.30.1.236        001b.0100.0056  Local              -   
1301  1301   VXLAN 10.30.1.236        001b.0100.0056  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.216        001b.0100.0042  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.225        001b.0100.004b  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.225        001b.0100.004b  Local              -   
1301  1301   VXLAN 10.30.1.217        001b.0100.0043  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.217        001b.0100.0043  Local              -   
1301  1301   VXLAN 10.30.1.214        001b.0100.0040  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.230        001b.0100.0050  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.254        0056.5656.5656  100.0.0.201        Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.254        0056.5656.5656  100.0.0.202        Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.227        001b.0100.004d  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.242        001b.0100.005c  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.223        001b.0100.0049  Local              -   
1301  1301   VXLAN 10.30.1.223        001b.0100.0049  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.202        001b.0100.0034  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.223        001b.0100.0049  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.226        001b.0100.004c  Local              -   
1301  1301   VXLAN 10.30.1.226        001b.0100.004c  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.211        001b.0100.003d  Local              -   
1301  1301   VXLAN 10.30.1.211        001b.0100.003d  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.220        001b.0100.0046  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.230        001b.0100.0050  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.230        001b.0100.0050  Local              -   
1301  1301   VXLAN 10.30.1.247        001b.0100.0061  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.228        001b.0100.004e  Local              -   
1301  1301   VXLAN 10.30.1.228        001b.0100.004e  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.219        001b.0100.0045  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.219        001b.0100.0045  Local              -   
1301  1301   VXLAN 10.30.1.227        001b.0100.004d  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.227        001b.0100.004d  Local              -   
1301  1301   VXLAN 10.30.1.210        001b.0100.003c  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.210        001b.0100.003c  Local              -   
1301  1301   VXLAN 10.30.1.210        001b.0100.003c  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.224        001b.0100.004a  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.224        001b.0100.004a  Local              -   
1301  1301   VXLAN 10.30.1.215        001b.0100.0041  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.215        001b.0100.0041  Local              -   
1301  1301   VXLAN 10.30.1.232        001b.0100.0052  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.232        001b.0100.0052  Local              -   
1303  1303   VXLAN 10.30.3.202        001b.0100.0066  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.238        001b.0100.008a  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.242        001b.0100.008e  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.235        001b.0100.0087  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.235        001b.0100.0087  Local              -   
1303  1303   VXLAN 10.30.3.209        001b.0100.006d  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.205        001b.0100.0069  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.205        001b.0100.0069  Local              -   
1303  1303   VXLAN 10.30.3.204        001b.0100.0068  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.216        001b.0100.0074  Local              -   
1303  1303   VXLAN 10.30.3.216        001b.0100.0074  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.232        001b.0100.0084  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.225        001b.0100.007d  Local              -   
1303  1303   VXLAN 10.30.3.225        001b.0100.007d  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.215        001b.0100.0073  Local              -   
1303  1303   VXLAN 10.30.3.215        001b.0100.0073  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.224        001b.0100.007c  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.242        001b.0100.008e  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.242        001b.0100.008e  Local              -   
1303  1303   VXLAN 10.30.3.246        001b.0100.0092  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.231        001b.0100.0083  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.225        001b.0100.007d  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.203        001b.0100.0003  Local              -   
1303  1303   VXLAN 10.30.3.203        001b.0100.0003  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.223        001b.0100.007b  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.223        001b.0100.007b  Local              -   
1303  1303   VXLAN 10.30.3.215        001b.0100.0073  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.248        001b.0100.0094  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.213        001b.0100.0071  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.213        001b.0100.0071  Local              -   
1303  1303   VXLAN 10.30.3.245        001b.0100.0091  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.207        001b.0100.006b  Local              -   
1303  1303   VXLAN 10.30.3.207        001b.0100.006b  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.254        0056.5656.5656  100.0.0.201        Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.254        0056.5656.5656  100.0.0.202        Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.206        001b.0100.006a  Local              -   
1303  1303   VXLAN 10.30.3.206        001b.0100.006a  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.214        001b.0100.0072  Local              -   
1303  1303   VXLAN 10.30.3.214        001b.0100.0072  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.234        001b.0100.0086  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.229        001b.0100.0081  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.221        001b.0100.0079  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.229        001b.0100.0081  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.229        001b.0100.0081  Local              -   
1303  1303   VXLAN 10.30.3.103        a266.0102.0001  100.0.0.201        -   
1303  1303   VXLAN 10.30.3.103        a266.0102.0001  100.0.0.202        -   
1303  1303   VXLAN 10.30.3.210        001b.0100.006e  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.210        001b.0100.006e  Local              -   
1303  1303   VXLAN 10.30.3.247        001b.0100.0093  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.247        001b.0100.0093  Local              -   
1303  1303   VXLAN 10.30.3.201        001b.0100.0065  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.210        001b.0100.006e  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.218        001b.0100.0076  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.236        001b.0100.0088  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.205        001b.0100.0069  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.209        001b.0100.006d  Local              -   
1303  1303   VXLAN 10.30.3.209        001b.0100.006d  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.249        001b.0100.0095  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.206        001b.0100.006a  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.223        001b.0100.007b  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.239        001b.0100.008b  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.250        001b.0100.0096  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.226        001b.0100.007e  Local              -   
1303  1303   VXLAN 10.30.3.226        001b.0100.007e  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.245        001b.0100.0091  Local              -   
1303  1303   VXLAN 10.30.3.245        001b.0100.0091  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.222        001b.0100.007a  Local              -   
1303  1303   VXLAN 10.30.3.222        001b.0100.007a  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.204        001b.0100.0068  Local              -   
1303  1303   VXLAN 10.30.3.204        001b.0100.0068  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.248        001b.0100.0094  Local              -   
1303  1303   VXLAN 10.30.3.248        001b.0100.0094  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.219        001b.0100.0077  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.236        001b.0100.0088  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.236        001b.0100.0088  Local              -   
1303  1303   VXLAN 10.30.3.238        001b.0100.008a  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.238        001b.0100.008a  Local              -   
1303  1303   VXLAN 10.30.3.247        001b.0100.0093  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.228        001b.0100.0080  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.212        001b.0100.0070  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.212        001b.0100.0070  Local              -   
1303  1303   VXLAN 10.30.3.233        001b.0100.0085  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.222        001b.0100.007a  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.211        001b.0100.006f  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.211        001b.0100.006f  Local              -   
1303  1303   VXLAN 10.30.3.235        001b.0100.0087  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.207        001b.0100.006b  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.220        001b.0100.0078  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.249        001b.0100.0095  Local              -   
1303  1303   VXLAN 10.30.3.249        001b.0100.0095  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.243        001b.0100.008f  Local              -   
1303  1303   VXLAN 10.30.3.243        001b.0100.008f  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.201        001b.0100.0065  Local              -   
1303  1303   VXLAN 10.30.3.201        001b.0100.0065  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.224        001b.0100.007c  Local              -   
1303  1303   VXLAN 10.30.3.224        001b.0100.007c  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.219        001b.0100.0077  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.219        001b.0100.0077  Local              -   
1303  1303   VXLAN 10.30.3.217        001b.0100.0075  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.217        001b.0100.0075  Local              -   
1303  1303   VXLAN 10.30.3.241        001b.0100.008d  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.212        001b.0100.0070  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.244        001b.0100.0090  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.227        001b.0100.007f  Local              -   
1303  1303   VXLAN 10.30.3.227        001b.0100.007f  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.237        001b.0100.0089  Local              -   
1303  1303   VXLAN 10.30.3.237        001b.0100.0089  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.211        001b.0100.006f  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.244        001b.0100.0090  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.244        001b.0100.0090  Local              -   
1303  1303   VXLAN 10.30.3.213        001b.0100.0071  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.226        001b.0100.007e  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.237        001b.0100.0089  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.230        001b.0100.0082  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.240        001b.0100.008c  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.240        001b.0100.008c  Local              -   
1303  1303   VXLAN 10.30.3.208        001b.0100.006c  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.232        001b.0100.0084  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.232        001b.0100.0084  Local              -   
1303  1303   VXLAN 10.30.3.241        001b.0100.008d  Local              -   
1303  1303   VXLAN 10.30.3.241        001b.0100.008d  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.216        001b.0100.0074  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.221        001b.0100.0079  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.221        001b.0100.0079  Local              -   
1303  1303   VXLAN 10.30.3.217        001b.0100.0075  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.239        001b.0100.008b  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.239        001b.0100.008b  Local              -   
1303  1303   VXLAN 10.30.3.208        001b.0100.006c  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.208        001b.0100.006c  Local              -   
1303  1303   VXLAN 10.30.3.246        001b.0100.0092  Local              -   
1303  1303   VXLAN 10.30.3.246        001b.0100.0092  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.0.201        Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.0.202        Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.233        001b.0100.0085  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.233        001b.0100.0085  Local              -   
1303  1303   VXLAN 10.30.3.203        001b.0100.0003  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.243        001b.0100.008f  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.231        001b.0100.0083  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.231        001b.0100.0083  Local              -   
1303  1303   VXLAN 10.30.3.234        001b.0100.0086  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.234        001b.0100.0086  Local              -   
1303  1303   VXLAN 10.30.3.240        001b.0100.008c  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.228        001b.0100.0080  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.228        001b.0100.0080  Local              -   
1303  1303   VXLAN 10.30.3.214        001b.0100.0072  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.250        001b.0100.0096  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.250        001b.0100.0096  Local              -   
1303  1303   VXLAN 10.30.3.230        001b.0100.0082  Local              -   
1303  1303   VXLAN 10.30.3.230        001b.0100.0082  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.227        001b.0100.007f  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.202        001b.0100.0066  Local              -   
1303  1303   VXLAN 10.30.3.202        001b.0100.0066  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.218        001b.0100.0076  Local              -   
1303  1303   VXLAN 10.30.3.218        001b.0100.0076  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.220        001b.0100.0078  Local              -   
1303  1303   VXLAN 10.30.3.220        001b.0100.0078  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.212        001b.0100.00a2  Local              -   
1304  1304   VXLAN 10.30.4.212        001b.0100.00a2  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.222        001b.0100.00ac  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.240        001b.0100.00be  Local              -   
1304  1304   VXLAN 10.30.4.240        001b.0100.00be  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.213        001b.0100.00a3  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.235        001b.0100.00b9  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.240        001b.0100.00be  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.221        001b.0100.00ab  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.221        001b.0100.00ab  Local              -   
1304  1304   VXLAN 10.30.4.222        001b.0100.00ac  Local              -   
1304  1304   VXLAN 10.30.4.222        001b.0100.00ac  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.236        001b.0100.00ba  Local              -   
1304  1304   VXLAN 10.30.4.236        001b.0100.00ba  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.249        001b.0100.00c7  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.249        001b.0100.00c7  Local              -   
1304  1304   VXLAN 10.30.4.201        001b.0100.0097  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.201        001b.0100.0097  Local              -   
1304  1304   VXLAN 10.30.4.244        001b.0100.00c2  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.244        001b.0100.00c2  Local              -   
1304  1304   VXLAN 10.30.4.234        001b.0100.00b8  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.246        001b.0100.00c4  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.246        001b.0100.00c4  Local              -   
1304  1304   VXLAN 10.30.4.254        0056.5656.5656  100.0.0.201        Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.254        0056.5656.5656  100.0.0.202        Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.215        001b.0100.00a5  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.215        001b.0100.00a5  Local              -   
1304  1304   VXLAN 10.30.4.228        001b.0100.00b2  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.205        001b.0100.009b  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.205        001b.0100.009b  Local              -   
1304  1304   VXLAN 10.30.4.238        001b.0100.00bc  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.213        001b.0100.00a3  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.213        001b.0100.00a3  Local              -   
1304  1304   VXLAN 10.30.4.216        001b.0100.00a6  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.224        001b.0100.00ae  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.209        001b.0100.009f  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.207        001b.0100.009d  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.207        001b.0100.009d  Local              -   
1304  1304   VXLAN 10.30.4.217        001b.0100.00a7  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.234        001b.0100.00b8  Local              -   
1304  1304   VXLAN 10.30.4.234        001b.0100.00b8  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.216        001b.0100.00a6  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.216        001b.0100.00a6  Local              -   
1304  1304   VXLAN 10.30.4.239        001b.0100.00bd  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.241        001b.0100.00bf  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.211        001b.0100.00a1  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.233        001b.0100.00b7  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.236        001b.0100.00ba  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.208        001b.0100.009e  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.207        001b.0100.009d  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.214        001b.0100.00a4  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.214        001b.0100.00a4  Local              -   
1304  1304   VXLAN 10.30.4.211        001b.0100.00a1  Local              -   
1304  1304   VXLAN 10.30.4.211        001b.0100.00a1  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.249        001b.0100.00c7  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.219        001b.0100.00a9  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.214        001b.0100.00a4  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.242        001b.0100.00c0  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.242        001b.0100.00c0  Local              -   
1304  1304   VXLAN 10.30.4.232        001b.0100.00b6  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.254        00aa.aaaa.aaaa  100.0.0.201        Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.254        00aa.aaaa.aaaa  100.0.0.202        Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.228        001b.0100.00b2  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.228        001b.0100.00b2  Local              -   
1304  1304   VXLAN 10.30.4.209        001b.0100.009f  Local              -   
1304  1304   VXLAN 10.30.4.209        001b.0100.009f  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.203        001b.0100.0004  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.203        001b.0100.0004  Local              -   
1304  1304   VXLAN 10.30.4.206        001b.0100.009c  Local              -   
1304  1304   VXLAN 10.30.4.206        001b.0100.009c  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.247        001b.0100.00c5  Local              -   
1304  1304   VXLAN 10.30.4.247        001b.0100.00c5  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.217        001b.0100.00a7  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.217        001b.0100.00a7  Local              -   
1304  1304   VXLAN 10.30.4.218        001b.0100.00a8  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.218        001b.0100.00a8  Local              -   
1304  1304   VXLAN 10.30.4.226        001b.0100.00b0  Local              -   
1304  1304   VXLAN 10.30.4.226        001b.0100.00b0  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.202        001b.0100.0098  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.230        001b.0100.00b4  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.230        001b.0100.00b4  Local              -   
1304  1304   VXLAN 10.30.4.250        001b.0100.00c8  Local              -   
1304  1304   VXLAN 10.30.4.250        001b.0100.00c8  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.215        001b.0100.00a5  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.205        001b.0100.009b  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.224        001b.0100.00ae  Local              -   
1304  1304   VXLAN 10.30.4.224        001b.0100.00ae  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.204        001b.0100.009a  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.246        001b.0100.00c4  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.220        001b.0100.00aa  Local              -   
1304  1304   VXLAN 10.30.4.220        001b.0100.00aa  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.225        001b.0100.00af  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.225        001b.0100.00af  Local              -   
1304  1304   VXLAN 10.30.4.243        001b.0100.00c1  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.244        001b.0100.00c2  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.210        001b.0100.00a0  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.210        001b.0100.00a0  Local              -   
1304  1304   VXLAN 10.30.4.210        001b.0100.00a0  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.247        001b.0100.00c5  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.230        001b.0100.00b4  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.248        001b.0100.00c6  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.248        001b.0100.00c6  Local              -   
1304  1304   VXLAN 10.30.4.229        001b.0100.00b3  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.232        001b.0100.00b6  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.232        001b.0100.00b6  Local              -   
1304  1304   VXLAN 10.30.4.242        001b.0100.00c0  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.239        001b.0100.00bd  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.239        001b.0100.00bd  Local              -   
1304  1304   VXLAN 10.30.4.103        a288.0103.0001  100.0.0.201        -   
1304  1304   VXLAN 10.30.4.103        a288.0103.0001  100.0.0.202        -   
1304  1304   VXLAN 10.30.4.245        001b.0100.00c3  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.245        001b.0100.00c3  Local              -   
1304  1304   VXLAN 10.30.4.208        001b.0100.009e  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.208        001b.0100.009e  Local              -   
1304  1304   VXLAN 10.30.4.223        001b.0100.00ad  Local              -   
1304  1304   VXLAN 10.30.4.223        001b.0100.00ad  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.204        001b.0100.009a  Local              -   
1304  1304   VXLAN 10.30.4.204        001b.0100.009a  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.238        001b.0100.00bc  Local              -   
1304  1304   VXLAN 10.30.4.238        001b.0100.00bc  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.235        001b.0100.00b9  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.235        001b.0100.00b9  Local              -   
1304  1304   VXLAN 10.30.4.248        001b.0100.00c6  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.202        001b.0100.0098  Local              -   
1304  1304   VXLAN 10.30.4.202        001b.0100.0098  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.212        001b.0100.00a2  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.231        001b.0100.00b5  Local              -   
1304  1304   VXLAN 10.30.4.231        001b.0100.00b5  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.227        001b.0100.00b1  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.206        001b.0100.009c  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.223        001b.0100.00ad  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.233        001b.0100.00b7  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.233        001b.0100.00b7  Local              -   
1304  1304   VXLAN 10.30.4.245        001b.0100.00c3  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.220        001b.0100.00aa  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.229        001b.0100.00b3  Local              -   
1304  1304   VXLAN 10.30.4.229        001b.0100.00b3  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.219        001b.0100.00a9  Local              -   
1304  1304   VXLAN 10.30.4.219        001b.0100.00a9  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.237        001b.0100.00bb  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.250        001b.0100.00c8  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.226        001b.0100.00b0  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.243        001b.0100.00c1  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.243        001b.0100.00c1  Local              -   
1304  1304   VXLAN 10.30.4.225        001b.0100.00af  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.203        001b.0100.0004  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.218        001b.0100.00a8  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.221        001b.0100.00ab  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.231        001b.0100.00b5  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.201        001b.0100.0097  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.237        001b.0100.00bb  Local              -   
1304  1304   VXLAN 10.30.4.237        001b.0100.00bb  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.227        001b.0100.00b1  Local              -   
1304  1304   VXLAN 10.30.4.227        001b.0100.00b1  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.241        001b.0100.00bf  Local              -   
1304  1304   VXLAN 10.30.4.241        001b.0100.00bf  100.0.0.204        -   
0     2303   VXLAN 10.30.3.203        001b.0100.0003  100.0.30.14        -   
0     2303   VXLAN 10.30.3.254        0056.5656.5656  100.0.30.14        Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.30.14        Stic
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

 B E      20.42.200.0/24 [20/0]
           via 20.200.203.200, Ethernet1
 B E      20.103.200.0/24 [20/0]
           via 20.200.203.200, Ethernet1
 B E      20.200.201.0/24 [20/0]
           via 20.200.203.200, Ethernet1
 B E      20.200.202.0/24 [20/0]
           via 20.200.203.200, Ethernet1
 C        20.200.203.0/24
           directly connected, Ethernet1
 B E      20.200.204.0/24 [20/0]
           via 20.200.203.200, Ethernet1
 B E      20.201.205.0/24 [20/0]
           via 20.200.203.200, Ethernet1
 B E      20.202.205.0/24 [20/0]
           via 20.200.203.200, Ethernet1
 B E      30.14.200.0/24 [20/0]
           via 20.200.203.200, Ethernet1
 B E      100.0.0.200/32 [20/0]
           via 20.200.203.200, Ethernet1
 B E      100.0.0.201/32 [20/0]
           via 20.200.203.200, Ethernet1
 B E      100.0.0.202/32 [20/0]
           via 20.200.203.200, Ethernet1
 C        100.0.0.203/32
           directly connected, Loopback0
 B E      100.0.0.204/32 [20/0]
           via 20.200.203.200, Ethernet1
 B E      100.0.30.14/32 [20/0]
           via 20.200.203.200, Ethernet1

```

## show ip arp

```text
Address         Age (sec)  Hardware Addr   Interface
20.200.203.200    0:00:29  444c.a873.5c75  Ethernet1
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

 B E      20.42.200.0/24 [20/0]
           via 20.200.203.200, Ethernet1
 B E      20.103.200.0/24 [20/0]
           via 20.200.203.200, Ethernet1
 B E      20.200.201.0/24 [20/0]
           via 20.200.203.200, Ethernet1
 B E      20.200.202.0/24 [20/0]
           via 20.200.203.200, Ethernet1
 C        20.200.203.0/24
           directly connected, Ethernet1
 B E      20.200.204.0/24 [20/0]
           via 20.200.203.200, Ethernet1
 B E      20.201.205.0/24 [20/0]
           via 20.200.203.200, Ethernet1
 B E      20.202.205.0/24 [20/0]
           via 20.200.203.200, Ethernet1
 B E      30.14.200.0/24 [20/0]
           via 20.200.203.200, Ethernet1
 B E      100.0.0.200/32 [20/0]
           via 20.200.203.200, Ethernet1
 B E      100.0.0.201/32 [20/0]
           via 20.200.203.200, Ethernet1
 B E      100.0.0.202/32 [20/0]
           via 20.200.203.200, Ethernet1
 C        100.0.0.203/32
           directly connected, Loopback0
 B E      100.0.0.204/32 [20/0]
           via 20.200.203.200, Ethernet1
 B E      100.0.30.14/32 [20/0]
           via 20.200.203.200, Ethernet1


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

 B E      10.10.103.103/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.10.103.0/24 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.10.201.0/24 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 C        10.10.203.0/24
           directly connected, Vlan1203
 B E      10.30.1.103/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.201/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.202/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.203/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.204/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.205/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.206/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.207/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.208/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.209/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.210/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.211/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.212/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.213/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.214/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.215/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.216/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.217/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.218/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.219/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.220/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.221/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.222/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.223/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.224/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.225/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.226/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.227/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.228/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.229/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.230/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.231/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.232/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.233/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.234/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.235/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.236/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.237/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.238/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.239/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.240/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.241/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.242/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.243/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.244/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.245/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.246/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.247/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.248/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.249/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.250/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 C        10.30.1.0/24
           directly connected, Vlan1301
 C        10.30.2.0/24
           directly connected, Vlan1302
 B E      10.30.3.103/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.201/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.202/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.203/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.204/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.205/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.206/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.207/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.208/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.209/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.210/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.211/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.212/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.213/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.214/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.215/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.216/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.217/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.218/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.219/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.220/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.221/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.222/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.223/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.224/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.225/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.226/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.227/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.228/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.229/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.230/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.231/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.232/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.233/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.234/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.235/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.236/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.237/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.238/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.239/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.240/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.241/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.242/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.243/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.244/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.245/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.246/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.247/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.248/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.249/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.250/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 C        10.30.3.0/24
           directly connected, Vlan1303
 B E      10.30.4.103/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.201/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.202/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.203/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.204/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.205/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.206/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.207/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.208/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.209/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.210/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.211/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.212/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.213/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.214/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.215/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.216/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.217/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.218/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.219/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.220/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.221/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.222/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.223/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.224/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.225/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.226/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.227/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.228/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.229/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.230/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.231/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.232/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.233/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.234/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.235/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.236/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.237/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.238/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.239/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.240/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.241/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.242/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.243/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.244/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.245/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.246/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.247/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.248/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.249/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.250/32 [20/0]
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 C        10.30.4.0/24
           directly connected, Vlan1304
 C        100.0.1.203/32
           directly connected, Loopback100
 B E      100.0.1.204/32 [20/0]
           via VTEP 100.0.0.204 VNI 1000 router-mac 98:5d:82:a2:04:f9

```

## show ip arp vrf all

```text

VRF: default
Address         Age (sec)  Hardware Addr   Interface
20.200.203.200    0:00:29  444c.a873.5c75  Ethernet1

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.21.47     0:03:29  5c5a.c7ff.8a0a  Management1
192.168.21.50     0:01:46  a84f.b1a5.5221  Management1
192.168.21.59     0:01:33  6607.f5d1.ae16  Management1

VRF: tenant-a
Address         Age (sec)  Hardware Addr   Interface
10.10.203.203     0:05:56  001b.0100.0001  Vlan1203, Port-Channel200
10.30.1.103             -  a244.0101.0001  Vlan1301, Vxlan1
10.30.1.201             -  001b.0100.0002  Vlan1301, Port-Channel200
10.30.1.202       1:29:58  001b.0100.0034  Vlan1301, Port-Channel200
10.30.1.203             -  001b.0100.0002  Vlan1301, Port-Channel200
10.30.1.204             -  001b.0100.0036  Vlan1301, Port-Channel200
10.30.1.205             -  001b.0100.0037  Vlan1301, Port-Channel200
10.30.1.206       1:29:58  001b.0100.0038  Vlan1301, Port-Channel200
10.30.1.207       1:29:58  001b.0100.0039  Vlan1301, Port-Channel200
10.30.1.208       1:29:58  001b.0100.003a  Vlan1301, Port-Channel200
10.30.1.209       1:29:58  001b.0100.003b  Vlan1301, Port-Channel200
10.30.1.210             -  001b.0100.003c  Vlan1301, Port-Channel200
10.30.1.211       1:29:58  001b.0100.003d  Vlan1301, Port-Channel200
10.30.1.212             -  001b.0100.003e  Vlan1301, Port-Channel200
10.30.1.213       1:29:58  001b.0100.003f  Vlan1301, Port-Channel200
10.30.1.214             -  001b.0100.0040  Vlan1301, Port-Channel200
10.30.1.215             -  001b.0100.0041  Vlan1301, Port-Channel200
10.30.1.216       1:29:58  001b.0100.0042  Vlan1301, Port-Channel200
10.30.1.217             -  001b.0100.0043  Vlan1301, Port-Channel200
10.30.1.218       1:29:58  001b.0100.0044  Vlan1301, Port-Channel200
10.30.1.219             -  001b.0100.0045  Vlan1301, Port-Channel200
10.30.1.220       1:29:58  001b.0100.0046  Vlan1301, Port-Channel200
10.30.1.221       1:29:58  001b.0100.0047  Vlan1301, Port-Channel200
10.30.1.222       1:29:58  001b.0100.0048  Vlan1301, Port-Channel200
10.30.1.223       1:29:58  001b.0100.0049  Vlan1301, Port-Channel200
10.30.1.224             -  001b.0100.004a  Vlan1301, Port-Channel200
10.30.1.225             -  001b.0100.004b  Vlan1301, Port-Channel200
10.30.1.226       1:29:58  001b.0100.004c  Vlan1301, Port-Channel200
10.30.1.227             -  001b.0100.004d  Vlan1301, Port-Channel200
10.30.1.228       1:29:58  001b.0100.004e  Vlan1301, Port-Channel200
10.30.1.229       1:29:58  001b.0100.004f  Vlan1301, Port-Channel200
10.30.1.230             -  001b.0100.0050  Vlan1301, Port-Channel200
10.30.1.231             -  001b.0100.0051  Vlan1301, Port-Channel200
10.30.1.232             -  001b.0100.0052  Vlan1301, Port-Channel200
10.30.1.233       1:29:58  001b.0100.0053  Vlan1301, Port-Channel200
10.30.1.234       1:29:58  001b.0100.0054  Vlan1301, Port-Channel200
10.30.1.235             -  001b.0100.0055  Vlan1301, Port-Channel200
10.30.1.236       1:29:58  001b.0100.0056  Vlan1301, Port-Channel200
10.30.1.237             -  001b.0100.0057  Vlan1301, Port-Channel200
10.30.1.238       1:29:58  001b.0100.0058  Vlan1301, Port-Channel200
10.30.1.239       1:29:58  001b.0100.0059  Vlan1301, Port-Channel200
10.30.1.240       1:29:58  001b.0100.005a  Vlan1301, Port-Channel200
10.30.1.241             -  001b.0100.005b  Vlan1301, Port-Channel200
10.30.1.242             -  001b.0100.005c  Vlan1301, Port-Channel200
10.30.1.243       1:29:58  001b.0100.005d  Vlan1301, Port-Channel200
10.30.1.244             -  001b.0100.005e  Vlan1301, Port-Channel200
10.30.1.245       1:29:58  001b.0100.005f  Vlan1301, Port-Channel200
10.30.1.246             -  001b.0100.0060  Vlan1301, Port-Channel200
10.30.1.247       1:29:58  001b.0100.0061  Vlan1301, Port-Channel200
10.30.1.248             -  001b.0100.0062  Vlan1301, Port-Channel200
10.30.1.249       1:29:58  001b.0100.0063  Vlan1301, Port-Channel200
10.30.1.250             -  001b.0100.0064  Vlan1301, Port-Channel200
10.30.3.103             -  a266.0102.0001  Vlan1303, Vxlan1
10.30.3.201       1:26:24  001b.0100.0065  Vlan1303, Port-Channel200
10.30.3.202       1:29:58  001b.0100.0066  Vlan1303, Port-Channel200
10.30.3.203       0:05:56  001b.0100.0003  Vlan1303, Port-Channel200
10.30.3.204       1:29:58  001b.0100.0068  Vlan1303, Port-Channel200
10.30.3.205             -  001b.0100.0069  Vlan1303, Port-Channel200
10.30.3.206       1:29:58  001b.0100.006a  Vlan1303, Port-Channel200
10.30.3.207       1:29:58  001b.0100.006b  Vlan1303, Port-Channel200
10.30.3.208             -  001b.0100.006c  Vlan1303, Port-Channel200
10.30.3.209       1:29:58  001b.0100.006d  Vlan1303, Port-Channel200
10.30.3.210             -  001b.0100.006e  Vlan1303, Port-Channel200
10.30.3.211             -  001b.0100.006f  Vlan1303, Port-Channel200
10.30.3.212             -  001b.0100.0070  Vlan1303, Port-Channel200
10.30.3.213             -  001b.0100.0071  Vlan1303, Port-Channel200
10.30.3.214       1:29:58  001b.0100.0072  Vlan1303, Port-Channel200
10.30.3.215       1:29:58  001b.0100.0073  Vlan1303, Port-Channel200
10.30.3.216       1:29:58  001b.0100.0074  Vlan1303, Port-Channel200
10.30.3.217             -  001b.0100.0075  Vlan1303, Port-Channel200
10.30.3.218       1:29:58  001b.0100.0076  Vlan1303, Port-Channel200
10.30.3.219             -  001b.0100.0077  Vlan1303, Port-Channel200
10.30.3.220       1:29:58  001b.0100.0078  Vlan1303, Port-Channel200
10.30.3.221             -  001b.0100.0079  Vlan1303, Port-Channel200
10.30.3.222       1:29:58  001b.0100.007a  Vlan1303, Port-Channel200
10.30.3.223             -  001b.0100.007b  Vlan1303, Port-Channel200
10.30.3.224       1:29:58  001b.0100.007c  Vlan1303, Port-Channel200
10.30.3.225       1:29:58  001b.0100.007d  Vlan1303, Port-Channel200
10.30.3.226       1:29:58  001b.0100.007e  Vlan1303, Port-Channel200
10.30.3.227       1:29:58  001b.0100.007f  Vlan1303, Port-Channel200
10.30.3.228             -  001b.0100.0080  Vlan1303, Port-Channel200
10.30.3.229             -  001b.0100.0081  Vlan1303, Port-Channel200
10.30.3.230       1:29:58  001b.0100.0082  Vlan1303, Port-Channel200
10.30.3.231             -  001b.0100.0083  Vlan1303, Port-Channel200
10.30.3.232             -  001b.0100.0084  Vlan1303, Port-Channel200
10.30.3.233             -  001b.0100.0085  Vlan1303, Port-Channel200
10.30.3.234             -  001b.0100.0086  Vlan1303, Port-Channel200
10.30.3.235             -  001b.0100.0087  Vlan1303, Port-Channel200
10.30.3.236             -  001b.0100.0088  Vlan1303, Port-Channel200
10.30.3.237       1:29:58  001b.0100.0089  Vlan1303, Port-Channel200
10.30.3.238             -  001b.0100.008a  Vlan1303, Port-Channel200
10.30.3.239             -  001b.0100.008b  Vlan1303, Port-Channel200
10.30.3.240             -  001b.0100.008c  Vlan1303, Port-Channel200
10.30.3.241       1:29:58  001b.0100.008d  Vlan1303, Port-Channel200
10.30.3.242             -  001b.0100.008e  Vlan1303, Port-Channel200
10.30.3.243       1:29:58  001b.0100.008f  Vlan1303, Port-Channel200
10.30.3.244             -  001b.0100.0090  Vlan1303, Port-Channel200
10.30.3.245       1:29:58  001b.0100.0091  Vlan1303, Port-Channel200
10.30.3.246       1:29:58  001b.0100.0092  Vlan1303, Port-Channel200
10.30.3.247             -  001b.0100.0093  Vlan1303, Port-Channel200
10.30.3.248       1:29:58  001b.0100.0094  Vlan1303, Port-Channel200
10.30.3.249       1:29:58  001b.0100.0095  Vlan1303, Port-Channel200
10.30.3.250             -  001b.0100.0096  Vlan1303, Port-Channel200
10.30.4.103             -  a288.0103.0001  Vlan1304, Vxlan1
10.30.4.201             -  001b.0100.0097  Vlan1304, Port-Channel200
10.30.4.202       1:29:58  001b.0100.0098  Vlan1304, Port-Channel200
10.30.4.203             -  001b.0100.0004  Vlan1304, Port-Channel200
10.30.4.204       1:29:58  001b.0100.009a  Vlan1304, Port-Channel200
10.30.4.205             -  001b.0100.009b  Vlan1304, Port-Channel200
10.30.4.206       1:29:58  001b.0100.009c  Vlan1304, Port-Channel200
10.30.4.207             -  001b.0100.009d  Vlan1304, Port-Channel200
10.30.4.208             -  001b.0100.009e  Vlan1304, Port-Channel200
10.30.4.209       1:29:58  001b.0100.009f  Vlan1304, Port-Channel200
10.30.4.210             -  001b.0100.00a0  Vlan1304, Port-Channel200
10.30.4.211       1:29:58  001b.0100.00a1  Vlan1304, Port-Channel200
10.30.4.212       1:29:58  001b.0100.00a2  Vlan1304, Port-Channel200
10.30.4.213             -  001b.0100.00a3  Vlan1304, Port-Channel200
10.30.4.214             -  001b.0100.00a4  Vlan1304, Port-Channel200
10.30.4.215             -  001b.0100.00a5  Vlan1304, Port-Channel200
10.30.4.216             -  001b.0100.00a6  Vlan1304, Port-Channel200
10.30.4.217             -  001b.0100.00a7  Vlan1304, Port-Channel200
10.30.4.218             -  001b.0100.00a8  Vlan1304, Port-Channel200
10.30.4.219       1:29:58  001b.0100.00a9  Vlan1304, Port-Channel200
10.30.4.220       1:29:58  001b.0100.00aa  Vlan1304, Port-Channel200
10.30.4.221             -  001b.0100.00ab  Vlan1304, Port-Channel200
10.30.4.222       1:29:58  001b.0100.00ac  Vlan1304, Port-Channel200
10.30.4.223       1:29:58  001b.0100.00ad  Vlan1304, Port-Channel200
10.30.4.224       1:29:58  001b.0100.00ae  Vlan1304, Port-Channel200
10.30.4.225             -  001b.0100.00af  Vlan1304, Port-Channel200
10.30.4.226       1:29:58  001b.0100.00b0  Vlan1304, Port-Channel200
10.30.4.227       1:29:58  001b.0100.00b1  Vlan1304, Port-Channel200
10.30.4.228             -  001b.0100.00b2  Vlan1304, Port-Channel200
10.30.4.229       1:29:58  001b.0100.00b3  Vlan1304, Port-Channel200
10.30.4.230             -  001b.0100.00b4  Vlan1304, Port-Channel200
10.30.4.231       1:29:58  001b.0100.00b5  Vlan1304, Port-Channel200
10.30.4.232             -  001b.0100.00b6  Vlan1304, Port-Channel200
10.30.4.233             -  001b.0100.00b7  Vlan1304, Port-Channel200
10.30.4.234       1:29:58  001b.0100.00b8  Vlan1304, Port-Channel200
10.30.4.235             -  001b.0100.00b9  Vlan1304, Port-Channel200
10.30.4.236       1:29:58  001b.0100.00ba  Vlan1304, Port-Channel200
10.30.4.237       1:29:58  001b.0100.00bb  Vlan1304, Port-Channel200
10.30.4.238       1:29:58  001b.0100.00bc  Vlan1304, Port-Channel200
10.30.4.239             -  001b.0100.00bd  Vlan1304, Port-Channel200
10.30.4.240       1:29:58  001b.0100.00be  Vlan1304, Port-Channel200
10.30.4.241       1:29:58  001b.0100.00bf  Vlan1304, Port-Channel200
10.30.4.242             -  001b.0100.00c0  Vlan1304, Port-Channel200
10.30.4.243             -  001b.0100.00c1  Vlan1304, Port-Channel200
10.30.4.244             -  001b.0100.00c2  Vlan1304, Port-Channel200
10.30.4.245             -  001b.0100.00c3  Vlan1304, Port-Channel200
10.30.4.246             -  001b.0100.00c4  Vlan1304, Port-Channel200
10.30.4.247       1:29:58  001b.0100.00c5  Vlan1304, Port-Channel200
10.30.4.248             -  001b.0100.00c6  Vlan1304, Port-Channel200
10.30.4.249             -  001b.0100.00c7  Vlan1304, Port-Channel200
10.30.4.250       1:38:19  001b.0100.00c8  Vlan1304, Port-Channel200
```

## show vxlan address-table

```text
          Vxlan Mac Address Table
----------------------------------------------------------------------

VLAN  Mac Address     Type      Prt  VTEP             Moves   Last Move
----  -----------     ----      ---  ----             -----   ---------
1301  0056.5656.5656  EVPN      Vx1  100.0.0.201      1       13:26:48 ago
                                     100.0.0.202    
1301  a244.0101.0001  EVPN      Vx1  100.0.0.201      1       0:05:48 ago
                                     100.0.0.202    
1303  0056.5656.5656  EVPN      Vx1  100.0.0.201      1       13:26:48 ago
                                     100.0.0.202    
1303  a266.0102.0001  EVPN      Vx1  100.0.0.201      1       0:05:48 ago
                                     100.0.0.202    
1304  0056.5656.5656  EVPN      Vx1  100.0.0.201      1       13:26:48 ago
                                     100.0.0.202    
1304  a288.0103.0001  EVPN      Vx1  100.0.0.201      1       0:05:48 ago
                                     100.0.0.202    
4094  2cdd.e90b.2283  EVPN      Vx1  100.0.0.201              13:26:53 ago
4094  2cdd.e90b.25b7  EVPN      Vx1  100.0.0.202              13:28:30 ago
4094  985d.82a2.04f9  EVPN      Vx1  100.0.0.204              21:24:56 ago
Total Remote Mac Addresses for this criterion: 9
```

## show vxlan vni

```text
VNI to VLAN Mapping for Vxlan1
VNI        VLAN       Source       Interface             802.1Q Tag
---------- ---------- ------------ --------------------- ----------
1203       1203       static       Port-Channel200       1203      
                                   Vxlan1                1203      
1301       1301       static       Port-Channel200       1301      
                                   Vxlan1                1301      
1302       1302       static       Port-Channel200       1302      
                                   Vxlan1                1302      
1303       1303       static       Port-Channel200       1303      
                                   Vxlan1                1303      
1304       1304       static       Port-Channel200       1304      
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
1203    001b.0100.0001    DYNAMIC     Po200      2       0:04:39 ago
1203    00aa.aaaa.aaaa    STATIC      Router
1301    001b.0100.0002    DYNAMIC     Po200      2       1:39:39 ago
1301    001b.0100.0033    DYNAMIC     Po200      2       1:29:39 ago
1301    001b.0100.0034    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.0035    DYNAMIC     Po200      1       1:34:39 ago
1301    001b.0100.0036    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.0037    DYNAMIC     Po200      1       1:34:39 ago
1301    001b.0100.0038    DYNAMIC     Po200      1       1:34:39 ago
1301    001b.0100.0039    DYNAMIC     Po200      1       1:34:08 ago
1301    001b.0100.003a    DYNAMIC     Po200      1       1:34:39 ago
1301    001b.0100.003b    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.003c    DYNAMIC     Po200      1       1:34:39 ago
1301    001b.0100.003d    DYNAMIC     Po200      1       1:34:39 ago
1301    001b.0100.003e    DYNAMIC     Po200      2       1:29:39 ago
1301    001b.0100.003f    DYNAMIC     Po200      1       1:34:08 ago
1301    001b.0100.0040    DYNAMIC     Po200      1       1:34:08 ago
1301    001b.0100.0041    DYNAMIC     Po200      1       1:34:39 ago
1301    001b.0100.0042    DYNAMIC     Po200      1       1:34:08 ago
1301    001b.0100.0043    DYNAMIC     Po200      1       1:34:08 ago
1301    001b.0100.0044    DYNAMIC     Po200      1       1:34:08 ago
1301    001b.0100.0045    DYNAMIC     Po200      1       1:34:08 ago
1301    001b.0100.0046    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.0047    DYNAMIC     Po200      1       1:34:39 ago
1301    001b.0100.0048    DYNAMIC     Po200      1       1:34:39 ago
1301    001b.0100.0049    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.004a    DYNAMIC     Po200      1       1:34:08 ago
1301    001b.0100.004b    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.004c    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.004d    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.004e    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.004f    DYNAMIC     Po200      1       1:34:08 ago
1301    001b.0100.0050    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.0051    DYNAMIC     Po200      1       1:34:08 ago
1301    001b.0100.0052    DYNAMIC     Po200      1       1:34:39 ago
1301    001b.0100.0053    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.0054    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.0055    DYNAMIC     Po200      1       1:34:39 ago
1301    001b.0100.0056    DYNAMIC     Po200      1       1:34:08 ago
1301    001b.0100.0057    DYNAMIC     Po200      1       1:34:08 ago
1301    001b.0100.0058    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.0059    DYNAMIC     Po200      2       1:29:39 ago
1301    001b.0100.005a    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.005b    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.005c    DYNAMIC     Po200      1       1:34:08 ago
1301    001b.0100.005d    DYNAMIC     Po200      1       1:34:39 ago
1301    001b.0100.005e    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.005f    DYNAMIC     Po200      1       1:34:08 ago
1301    001b.0100.0060    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.0061    DYNAMIC     Po200      1       1:42:58 ago
1301    001b.0100.0062    DYNAMIC     Po200      1       1:34:39 ago
1301    001b.0100.0063    DYNAMIC     Po200      1       1:34:08 ago
1301    001b.0100.0064    DYNAMIC     Po200      1       1:34:39 ago
1301    0056.5656.5656    STATIC      Vx1
1301    00aa.aaaa.aaaa    STATIC      Router
1301    00cc.cccc.bbbb    STATIC      Po200
1301    a244.0101.0001    DYNAMIC     Vx1        1       0:05:49 ago
1302    00aa.aaaa.aaaa    STATIC      Router
1303    001b.0100.0003    DYNAMIC     Po200      1       1:44:39 ago
1303    001b.0100.0065    DYNAMIC     Po200      2       1:24:39 ago
1303    001b.0100.0066    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.0067    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.0068    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.0069    DYNAMIC     Po200      1       1:34:08 ago
1303    001b.0100.006a    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.006b    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.006c    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.006d    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.006e    DYNAMIC     Po200      1       1:34:08 ago
1303    001b.0100.006f    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.0070    DYNAMIC     Po200      1       1:34:08 ago
1303    001b.0100.0071    DYNAMIC     Po200      1       1:34:08 ago
1303    001b.0100.0072    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.0073    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.0074    DYNAMIC     Po200      2       1:29:39 ago
1303    001b.0100.0075    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.0076    DYNAMIC     Po200      1       1:34:08 ago
1303    001b.0100.0077    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.0078    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.0079    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.007a    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.007b    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.007c    DYNAMIC     Po200      1       1:34:08 ago
1303    001b.0100.007d    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.007e    DYNAMIC     Po200      1       1:34:08 ago
1303    001b.0100.007f    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.0080    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.0081    DYNAMIC     Po200      1       1:34:08 ago
1303    001b.0100.0082    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.0083    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.0084    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.0085    DYNAMIC     Po200      1       1:34:08 ago
1303    001b.0100.0086    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.0087    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.0088    DYNAMIC     Po200      1       1:34:08 ago
1303    001b.0100.0089    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.008a    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.008b    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.008c    DYNAMIC     Po200      1       1:34:08 ago
1303    001b.0100.008d    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.008e    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.008f    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.0090    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.0091    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.0092    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.0093    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.0094    DYNAMIC     Po200      1       1:42:58 ago
1303    001b.0100.0095    DYNAMIC     Po200      1       1:34:39 ago
1303    001b.0100.0096    DYNAMIC     Po200      1       1:34:39 ago
1303    0056.5656.5656    STATIC      Vx1
1303    00aa.aaaa.aaaa    STATIC      Router
1303    a266.0102.0001    DYNAMIC     Vx1        1       0:05:49 ago
1304    001b.0100.0004    DYNAMIC     Po200      1       1:19:33 ago
1304    001b.0100.0097    DYNAMIC     Po200      1       1:34:08 ago
1304    001b.0100.0098    DYNAMIC     Po200      2       1:29:39 ago
1304    001b.0100.0099    DYNAMIC     Po200      1       1:34:38 ago
1304    001b.0100.009a    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.009b    DYNAMIC     Po200      1       1:34:39 ago
1304    001b.0100.009c    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.009d    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.009e    DYNAMIC     Po200      1       1:34:08 ago
1304    001b.0100.009f    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00a0    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00a1    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00a2    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00a3    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00a4    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00a5    DYNAMIC     Po200      1       1:34:08 ago
1304    001b.0100.00a6    DYNAMIC     Po200      1       1:34:08 ago
1304    001b.0100.00a7    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00a8    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00a9    DYNAMIC     Po200      1       1:34:39 ago
1304    001b.0100.00aa    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00ab    DYNAMIC     Po200      2       1:24:39 ago
1304    001b.0100.00ac    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00ad    DYNAMIC     Po200      2       1:29:39 ago
1304    001b.0100.00ae    DYNAMIC     Po200      1       1:34:08 ago
1304    001b.0100.00af    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00b0    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00b1    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00b2    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00b3    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00b4    DYNAMIC     Po200      1       1:34:39 ago
1304    001b.0100.00b5    DYNAMIC     Po200      1       1:34:08 ago
1304    001b.0100.00b6    DYNAMIC     Po200      1       1:34:08 ago
1304    001b.0100.00b7    DYNAMIC     Po200      1       1:34:39 ago
1304    001b.0100.00b8    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00b9    DYNAMIC     Po200      2       1:24:39 ago
1304    001b.0100.00ba    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00bb    DYNAMIC     Po200      1       1:34:39 ago
1304    001b.0100.00bc    DYNAMIC     Po200      1       1:34:39 ago
1304    001b.0100.00bd    DYNAMIC     Po200      1       1:34:39 ago
1304    001b.0100.00be    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00bf    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00c0    DYNAMIC     Po200      1       1:34:08 ago
1304    001b.0100.00c1    DYNAMIC     Po200      1       1:42:58 ago
1304    001b.0100.00c2    DYNAMIC     Po200      1       1:34:39 ago
1304    001b.0100.00c3    DYNAMIC     Po200      1       1:34:08 ago
1304    001b.0100.00c4    DYNAMIC     Po200      1       1:34:39 ago
1304    001b.0100.00c5    DYNAMIC     Po200      1       1:34:08 ago
1304    001b.0100.00c6    DYNAMIC     Po200      2       1:24:39 ago
1304    001b.0100.00c7    DYNAMIC     Po200      1       1:34:39 ago
1304    001b.0100.00c8    DYNAMIC     Po200      1       1:52:28 ago
1304    0056.5656.5656    STATIC      Vx1
1304    00aa.aaaa.aaaa    STATIC      Router
1304    a288.0103.0001    DYNAMIC     Vx1        1       0:05:49 ago
4094    00aa.aaaa.aaaa    STATIC      Router
4094    2cdd.e90b.2283    DYNAMIC     Vx1        0       13:26:53 ago
4094    2cdd.e90b.25b7    DYNAMIC     Vx1        0       13:28:30 ago
4094    985d.82a2.04f9    DYNAMIC     Vx1        0       21:24:56 ago
Total Mac Addresses for this criterion: 170

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
001b.0100.0034, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0072, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0085, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
00aa.aaaa.aaaa, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 13: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
001b.0100.00c4, VLAN 1304, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0099, VLAN 1304, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.006b, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0066, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.008f, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00c7, VLAN 1304, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00c8, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.009f, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.004c, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.004b, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00b7, VLAN 1304, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00bb, VLAN 1304, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00a4, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0083, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0052, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0086, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
0056.5656.5656, VLAN 1303, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 13: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
001b.0100.005e, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0047, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0069, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00bd, VLAN 1304, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00b5, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.006a, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0043, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00a5, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0054, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.007c, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0050, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.004e, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00ae, VLAN 1304, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00c0, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.006c, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.007e, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0080, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0078, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0061, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00c2, VLAN 1304, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
00aa.aaaa.aaaa, VLAN 1303, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 13: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
001b.0100.009d, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.008d, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0082, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00ab, VLAN 1304, seq 2, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0051, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.003c, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0059, VLAN 1301, seq 2, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0037, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00a2, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0048, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0093, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.005d, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00b0, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.004f, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0087, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00b8, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.005a, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00c5, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0060, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0046, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.005c, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0042, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00ac, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0056.5656.5656, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 13: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
001b.0100.00a0, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0084, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
00cc.cccc.bbbb, VLAN 1301, seq 1, pref 64, configuredStaticMac, source: Local Static
   Port-Channel200
001b.0100.003d, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0089, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0038, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.004d, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0063, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.003b, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.007d, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
a288.0103.0001, VLAN 1304, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 13: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
001b.0100.0096, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0071, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0092, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0036, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0058, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0077, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00a6, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0040, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00a1, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.003e, VLAN 1301, seq 2, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0098, VLAN 1304, seq 2, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0070, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00b9, VLAN 1304, seq 2, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
a244.0101.0001, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 13: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
001b.0100.005f, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0075, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.008b, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.007a, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00af, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0067, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0062, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0053, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0064, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00a8, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.008e, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0039, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0094, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0076, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.003a, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.007b, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0045, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00be, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.006f, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.007f, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0056, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0049, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0055, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00b6, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.004a, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.009a, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00b4, VLAN 1304, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0033, VLAN 1301, seq 2, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.008c, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
00aa.aaaa.aaaa, VLAN 1304, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 13: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
001b.0100.00aa, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0004, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00bf, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0079, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00b2, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00b1, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00c1, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.005b, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00a3, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0065, VLAN 1303, seq 2, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0097, VLAN 1304, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.009e, VLAN 1304, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.008a, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0003, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.009b, VLAN 1304, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.006e, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0035, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00ba, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.006d, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0068, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0088, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0095, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0001, VLAN 1203, seq 2, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0056.5656.5656, VLAN 1304, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 13: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
001b.0100.0090, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00bc, VLAN 1304, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0081, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00c3, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00a7, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00ad, VLAN 1304, seq 2, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.003f, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.009c, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0057, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0074, VLAN 1303, seq 2, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.00c6, VLAN 1304, seq 2, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0044, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00a9, VLAN 1304, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
a266.0102.0001, VLAN 1303, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 13: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
001b.0100.0091, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.00b3, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0002, VLAN 1301, seq 2, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0041, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001b.0100.0073, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
```

## show vxlan flood vtep domain local

```text
          VXLAN Flood VTEP Table
--------------------------------------------------------------------------------

VLANS                            Ip Address
-----------------------------   ------------------------------------------------
1203,4094                       100.0.0.204    
1301-1304                       100.0.0.201     100.0.0.202     100.0.0.204    
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
Router identifier 100.0.0.203, local AS number 65203
```

## show bgp evpn instance

```text
EVPN instance: SBD tenant-a
  Route distinguisher: 100.0.0.203:1000
  Route target import: Route-Target-AS:1000:1000
  Route target export: Route-Target-AS:1000:1000
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.203
  VXLAN: enabled
  MPLS: disabled
EVPN instance: VLAN 1203
  Route distinguisher: 100.0.0.203:1203
  Route target import: Route-Target-AS:1203:1203
  Route target export: Route-Target-AS:1203:1203
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.203
  VXLAN: enabled
  MPLS: disabled
  Local ethernet segment:
    ESI: 0000:0000:0000:0203:0204
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:30:02:04
      DF election algorithm: preference
      Designated forwarder: 100.0.0.204
      Non-Designated forwarder: 100.0.0.203
EVPN instance: VLAN 1301
  Route distinguisher: 100.0.0.203:1301
  Route target import: Route-Target-AS:1301:1301
  Route target export: Route-Target-AS:1301:1301
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.203
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:1111:1111:1111:1111
    Active TEPs: 100.0.0.201, 100.0.0.202
  Local ethernet segment:
    ESI: 0000:0000:0000:0203:0204
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:30:02:04
      DF election algorithm: preference
      Designated forwarder: 100.0.0.204
      Non-Designated forwarder: 100.0.0.203
EVPN instance: VLAN 1302
  Route distinguisher: 100.0.0.203:1302
  Route target import: Route-Target-AS:1302:1302
  Route target export: Route-Target-AS:1302:1302
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.203
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:1111:1111:1111:1111
    Active TEPs: 100.0.0.201, 100.0.0.202
  Local ethernet segment:
    ESI: 0000:0000:0000:0203:0204
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:30:02:04
      DF election algorithm: preference
      Designated forwarder: 100.0.0.204
      Non-Designated forwarder: 100.0.0.203
EVPN instance: VLAN-aware bundle 1303-1304
  Route distinguisher: 100.0.0.203:1303
  Route target import: Route-Target-AS:1303:1303
  Route target export: Route-Target-AS:1303:1303
  Service interface: VLAN-aware bundle
  Local VXLAN IP address: 100.0.0.203
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:1111:1111:1111:1111
    Active TEPs: 100.0.0.201, 100.0.0.202
  Local ethernet segment:
    ESI: 0000:0000:0000:0203:0204
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:30:02:04
      DF election algorithm: preference
      Designated forwarder: 100.0.0.204
      Non-Designated forwarder: 100.0.0.203
```

## show interfaces counters rates | nz

```text
Port      Name        Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Et1       A-Spine-200  0:01      1.0   0.0%        0      0.9   0.0%        0
Et5       A-Harn-205   0:01      0.6   0.0%        0      0.6   0.0%        0
Ma1                    0:05      0.1   0.0%        0      0.8   0.1%        0
Po200                  0:01      0.6   0.0%        0      0.6   0.0%        0
```

