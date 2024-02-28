# Test results for PE14-T3-204

## show hostname

```text
Hostname: PE14-T3-204
FQDN:     PE14-T3-204.ns.eantc.de
```

## show ip bgp summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.204, local AS number 65204
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor       V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  ANET.IPV4                20.200.204.200 4 65000           2373      2294    0    0    1d04h Estab   11     11
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.204, local AS number 65204
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  ANET.EVPN                100.0.0.200 4 65000           9416      4105    0    0    1d04h Estab   178    178
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.204, local AS number 65204
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1203:1203 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.30.14:1301
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.30.14:1305
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.30.14:1306
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 1303 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
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
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:2
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.30.14:0
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:1303:1303 Route-Target-AS:65205:1301 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.22:2301
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 2301
BGP routing table entry for auto-discovery 0 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65314 65205 65206 65056
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2301
BGP routing table entry for auto-discovery 0 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 1303 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65314 65205 65206 65056
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2303
BGP routing table entry for auto-discovery 1303 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.22:2301
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
BGP routing table entry for auto-discovery 0500:00ff:2200:0005:1500, Route Distinguisher: 100.0.30.14:0
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0500:00ff:2200:0005:1700, Route Distinguisher: 100.0.30.14:0
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0500:00ff:2200:0005:1800, Route Distinguisher: 100.0.30.14:0
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.204, local AS number 65204
BGP routing table entry for mac-ip 001b.0100.0001, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1203 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001b.0100.0002, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:5
      VNI: 1301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 001b.0100.0002, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:5 EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 001b.0100.0002, Route Distinguisher: 100.0.30.14:1301
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:5
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 0056.5656.5656, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201 65206 65056
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 0056.5656.5656, Route Distinguisher: 100.0.30.14:1301
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 0056.5656.5656 10.10.103.254, Route Distinguisher: 100.0.0.56:1103
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1103 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.30.1.254, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65314 65205 65206 65056
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 0056.5656.5656 10.30.1.254, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.30.1.254, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201 65206 65056
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 0056.5656.5656 10.30.1.254, Route Distinguisher: 100.0.30.14:1301
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 0056.5656.5656 10.30.2.254, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201 65206 65056
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.14:1301
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0500:00ff:2200:0005:1500
BGP routing table entry for mac-ip 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.14:1306
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.103.254, Route Distinguisher: 100.0.0.56:1103
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1103 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.203.254, Route Distinguisher: 100.0.0.56:1203
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1203 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65314 65205 65206 65056
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201 65206 65056
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.30.14:1301
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0500:00ff:2200:0005:1500
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.30.14:1306
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 00cc.cccc.bbbb, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 00cc.cccc.bbbb, Route Distinguisher: 100.0.30.14:1306
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip a244.0101.0001, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip a244.0101.0001, Route Distinguisher: 100.0.30.14:1301
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip a244.0101.0001 10.30.1.103, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip a244.0101.0001 10.30.1.103, Route Distinguisher: 100.0.0.103:2301
 Paths: 1 available
  65000 65314 65205 65206 65103
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1301 L3 VNI: 1000 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip a244.0101.0001 10.30.1.103, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip a244.0101.0001 10.30.1.103, Route Distinguisher: 100.0.30.14:1301
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip f8c1.1604.3007, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip f8c1.1604.3007, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip f8c1.1604.3007, Route Distinguisher: 100.0.30.14:1301
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip f8c1.1604.3007, Route Distinguisher: 100.0.30.14:1306
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip f8c1.1604.3007 10.30.1.14, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip f8c1.1604.3007 10.30.1.14, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip f8c1.1604.3007 10.30.1.14, Route Distinguisher: 100.0.30.14:1301
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip f8c1.1604.3007 10.30.1.14, Route Distinguisher: 100.0.30.14:1306
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 001b.0100.0003, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:5
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65314 65205 65206 65056
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:5
      VNI: 2303 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:5
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 0056.5656.5656, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 0056.5656.5656, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65314 65205 65206 65056
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2303 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.14:1305
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0500:00ff:2200:0005:1700
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65314 65205 65206 65056
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2303 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.30.14:1305
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0500:00ff:2200:0005:1700
BGP routing table entry for mac-ip 1303 a266.0102.0001, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 a266.0102.0001, Route Distinguisher: 100.0.30.14:1305
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 a266.0102.0001 10.30.3.103, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 a266.0102.0001 10.30.3.103, Route Distinguisher: 100.0.0.103:2303
 Paths: 1 available
  65000 65314 65205 65206 65103
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 2303 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 a266.0102.0001 10.30.3.103, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1303 a266.0102.0001 10.30.3.103, Route Distinguisher: 100.0.30.14:1305
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 f8c1.1604.3007, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 f8c1.1604.3007, Route Distinguisher: 100.0.30.14:1305
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 f8c1.1604.3007 10.30.3.14, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65314 65205 65206 65056
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2303 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 f8c1.1604.3007 10.30.3.14, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 f8c1.1604.3007 10.30.3.14, Route Distinguisher: 100.0.30.14:1305
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 0056.5656.5656, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 0056.5656.5656, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254, Route Distinguisher: 100.0.0.56:51304
 Paths: 1 available
  65000 65314 65205 65206 65056
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.14:1305
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0500:00ff:2200:0005:1800
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.0.56:51304
 Paths: 1 available
  65000 65314 65205 65206 65056
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.30.14:1305
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0500:00ff:2200:0005:1800
BGP routing table entry for mac-ip 1304 a288.0103.0001, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 a288.0103.0001, Route Distinguisher: 100.0.30.14:1305
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1304 a288.0103.0001 10.30.4.103, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 a288.0103.0001 10.30.4.103, Route Distinguisher: 100.0.0.103:2303
 Paths: 1 available
  65000 65314 65205 65206 65103
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 2304 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 a288.0103.0001 10.30.4.103, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 1304 a288.0103.0001 10.30.4.103, Route Distinguisher: 100.0.30.14:1305
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1304 f8c1.1604.3007, Route Distinguisher: 100.0.0.56:51304
 Paths: 1 available
  65000 65314 65205 65206 65056
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 f8c1.1604.3007, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1304 f8c1.1604.3007, Route Distinguisher: 100.0.30.14:1305
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 f8c1.1604.3007 10.30.4.14, Route Distinguisher: 100.0.0.56:51304
 Paths: 1 available
  65000 65314 65205 65206 65056
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 f8c1.1604.3007 10.30.4.14, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1304 f8c1.1604.3007 10.30.4.14, Route Distinguisher: 100.0.30.14:1305
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
```

## show bgp evpn route-type imet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.204, local AS number 65204
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
      PMSI Tunnel: Ingress Replication, MPLS Label: 1022, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:2301
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 2301
      PMSI Tunnel: Ingress Replication, MPLS Label: 2301, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:1103
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1103
      PMSI Tunnel: Ingress Replication, MPLS Label: 1103, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.56
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan Multicast Flags: IGMP proxy, OISM-supported, SBD
      VNI: 1000
      PMSI Tunnel: Ingress Replication, MPLS Label: 1000, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 100.0.0.204, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
      PMSI Tunnel: Ingress Replication, MPLS Label: 1203, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 100.0.0.204, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 100.0.0.204, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 100.0.30.14, Route Distinguisher: 100.0.30.14:1301
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.30.14
BGP routing table entry for imet 100.0.30.14, Route Distinguisher: 100.0.30.14:1306
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.30.14
BGP routing table entry for imet 1303 100.0.0.22, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 1303 100.0.0.56, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1303 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.201
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
BGP routing table entry for imet 1303 100.0.30.14, Route Distinguisher: 100.0.30.14:1305
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.30.14
BGP routing table entry for imet 1304 100.0.0.22, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 1304 100.0.0.56, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1304 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.201
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
BGP routing table entry for imet 1304 100.0.30.14, Route Distinguisher: 100.0.30.14:1305
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.30.14
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.204, local AS number 65204
BGP routing table entry for ethernet-segment 0000:0000:0000:0203:0204 100.0.0.203, Route Distinguisher: 100.0.0.203:1
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:30:02:04 DF Election: Preference 100
BGP routing table entry for ethernet-segment 0000:0000:0000:0203:0204 100.0.0.204, Route Distinguisher: 100.0.0.204:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:30:02:04 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.201, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:11:11:11:11:11 DF Election: Preference 100
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.30.14, Route Distinguisher: 100.0.30.14:0
 Paths: 1 available
  65000 65314
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:11:11:11:11:11
BGP routing table entry for ethernet-segment 0000:2222:2222:2222:1111 100.0.0.22, Route Distinguisher: 100.0.0.22:0
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:22:22:22:22:22 DF Election: Modulus-based
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.204, local AS number 65204
BGP routing table entry for ip-prefix 10.10.103.0/24, Route Distinguisher: 100.0.0.103:1103
 Paths: 1 available
  65000 65314 65205 65206 65103
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.103.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201 65206 65103
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN 2:2:None
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.14/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN 2:2:None
BGP routing table entry for ip-prefix 10.30.1.103/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201 65206 65103
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:2c:dd:e9:0b:22:83
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.14/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN 2:2:None
BGP routing table entry for ip-prefix 10.30.3.103/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201 65206 65103
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.3.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN 2:2:None
BGP routing table entry for ip-prefix 10.30.3.254/32, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.254/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:2c:dd:e9:0b:22:83
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.14/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN 2:2:None
BGP routing table entry for ip-prefix 10.30.4.103/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201 65206 65103
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.4.254/32, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  65000 65314 65205
    100.0.30.14 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.254/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 100.0.1.203/32, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 100.0.1.204/32, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
```

## show bgp evpn route-type smet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.204, local AS number 65204
```

## show bgp evpn route-type spmsi detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.204, local AS number 65204
```

## show bgp evpn arp

```text
VLAN  Label  Encap IP                 MAC             Tunnel Endpoint    Seq#
----- ------ ----- ------------------ --------------- ------------------ ----
0     1103   VXLAN 10.10.103.103      a222.0100.0001  100.0.30.14        -   
1203  1203   VXLAN 10.10.203.204      444c.a873.5c75  100.0.0.203        -   
1203  1203   VXLAN 10.10.203.203      001b.0100.0001  100.0.0.203        -   
1203  1203   VXLAN 10.10.203.203      001b.0100.0001  Local              -   
1203  1203   VXLAN 10.10.203.203      001b.0100.0001  100.0.0.203        -   
1203  1203   VXLAN 10.10.203.254      00aa.aaaa.aaaa  100.0.30.14        Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.202        444c.a873.5c75  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.238        001b.0100.0058  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.232        001b.0100.0052  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.221        001b.0100.0047  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.103        a244.0101.0001  100.0.0.202        -   
1301  1301   VXLAN 10.30.1.208        001b.0100.003a  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.245        001b.0100.005f  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.209        001b.0100.003b  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.236        001b.0100.0056  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.237        001b.0100.0057  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.244        001b.0100.005e  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.239        001b.0100.0059  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.216        001b.0100.0042  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.240        001b.0100.005a  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.241        001b.0100.005b  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.246        001b.0100.0060  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.203        001b.0100.0035  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.229        001b.0100.004f  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.222        001b.0100.0048  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.204        001b.0100.0036  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.242        001b.0100.005c  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.226        001b.0100.004c  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.206        001b.0100.0038  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.203        001b.0100.0002  100.0.0.203        6   
1301  1301   VXLAN 10.30.1.225        001b.0100.004b  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.217        001b.0100.0043  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.224        001b.0100.004a  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.220        001b.0100.0046  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.214        001b.0100.0040  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.223        001b.0100.0049  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.249        001b.0100.0063  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.103        a244.0101.0001  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.103        a244.0101.0001  100.0.30.14        -   
1301  1301   VXLAN 10.30.1.230        001b.0100.0050  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.254        00aa.aaaa.aaaa  100.0.0.201        Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.254        00aa.aaaa.aaaa  100.0.30.14        Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.254        00aa.aaaa.aaaa  100.0.30.14        -   
1301  1301   VXLAN 10.30.1.211        001b.0100.003d  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.247        001b.0100.0061  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.210        001b.0100.003c  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.250        001b.0100.0064  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.248        001b.0100.0062  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.231        001b.0100.0051  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.254        0056.5656.5656  100.0.0.201        Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.254        0056.5656.5656  100.0.30.14        Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.254        0056.5656.5656  100.0.30.14        -   
1301  1301   VXLAN 10.30.1.212        001b.0100.003e  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.207        001b.0100.0039  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.218        001b.0100.0044  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.215        001b.0100.0041  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.201        001b.0100.0033  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.233        001b.0100.0053  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.235        001b.0100.0055  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.234        001b.0100.0054  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.201        001b.0100.0002  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.228        001b.0100.004e  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.227        001b.0100.004d  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.202        001b.0100.0034  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.14         f8c1.1604.3007  100.0.0.201        Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.14         f8c1.1604.3007  100.0.30.14        Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.213        001b.0100.003f  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.243        001b.0100.005d  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.205        001b.0100.0037  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.219        001b.0100.0045  100.0.0.203        -   
1302  1302   VXLAN 10.30.2.202        444c.a873.5c75  100.0.0.203        -   
1302  1302   VXLAN 10.30.2.254        0056.5656.5656  100.0.30.14        Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.103        a266.0102.0001  100.0.0.201        -   
1303  1303   VXLAN 10.30.3.103        a266.0102.0001  100.0.30.14        -   
1303  1303   VXLAN 10.30.3.203        001b.0100.0003  100.0.0.203        5   
0     2303   VXLAN 10.30.3.203        001b.0100.0003  100.0.30.14        5   
1303  1303   VXLAN 10.30.3.203        001b.0100.0003  Local              5   
1303  1303   VXLAN 10.30.3.254        0056.5656.5656  100.0.0.201        Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.254        0056.5656.5656  100.0.30.14        Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.0.201        Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.30.14        Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.30.14        -   
1303  1303   VXLAN 10.30.3.14         f8c1.1604.3007  100.0.30.14        Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.14         f8c1.1604.3007  100.0.30.14        Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.103        a288.0103.0001  100.0.0.201        -   
1304  1304   VXLAN 10.30.4.103        a288.0103.0001  100.0.30.14        -   
1304  1304   VXLAN 10.30.4.14         f8c1.1604.3007  100.0.30.14        Stic
                                                                         ky  
0     2304   VXLAN 10.30.4.14         f8c1.1604.3007  100.0.30.14        Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.254        0056.5656.5656  100.0.0.201        Stic
                                                                         ky  
0     2304   VXLAN 10.30.4.254        0056.5656.5656  100.0.30.14        Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.254        00aa.aaaa.aaaa  100.0.0.201        Stic
                                                                         ky  
0     2304   VXLAN 10.30.4.254        00aa.aaaa.aaaa  100.0.30.14        Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.254        00aa.aaaa.aaaa  100.0.30.14        -   
0     2303   VXLAN 10.30.3.103        a266.0102.0001  100.0.30.14        -   
0     2303   VXLAN 10.30.3.203        001b.0100.0003  100.0.30.14        5   
0     2303   VXLAN 10.30.3.254        0056.5656.5656  100.0.30.14        Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.30.14        Stic
                                                                         ky  
0     2304   VXLAN 10.30.4.103        a288.0103.0001  100.0.30.14        -   
0     2304   VXLAN 10.30.4.203        001b.0100.0004  100.0.30.14        1   
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

 B E      20.40.201.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      20.103.200.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      20.200.201.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      20.200.203.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 C        20.200.204.0/24
           directly connected, Ethernet1
 B E      20.201.205.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      30.14.200.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.200/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.201/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.203/32 [20/0]
           via 20.200.204.200, Ethernet1
 C        100.0.0.204/32
           directly connected, Loopback0
 B E      100.0.30.14/32 [20/0]
           via 20.200.204.200, Ethernet1

```

## show ip arp

```text
Address         Age (sec)  Hardware Addr   Interface
20.200.204.200    0:00:03  444c.a873.5c75  Ethernet1
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

 B E      20.40.201.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      20.103.200.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      20.200.201.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      20.200.203.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 C        20.200.204.0/24
           directly connected, Ethernet1
 B E      20.201.205.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      30.14.200.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.200/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.201/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.203/32 [20/0]
           via 20.200.204.200, Ethernet1
 C        100.0.0.204/32
           directly connected, Loopback0
 B E      100.0.30.14/32 [20/0]
           via 20.200.204.200, Ethernet1


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

 B E      10.10.103.0/24 [20/0]
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.10.201.0/24 [20/0]
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 C        10.10.203.0/24
           directly connected, Vlan1203
 B E      10.30.1.14/32 [20/0]
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.1.103/32 [20/0]
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 C        10.30.1.0/24
           directly connected, Vlan1301
 C        10.30.2.0/24
           directly connected, Vlan1302
 B E      10.30.3.14/32 [20/0]
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.103/32 [20/0]
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.3.203/32 [20/0]
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 C        10.30.3.0/24
           directly connected, Vlan1303
 B E      10.30.4.14/32 [20/0]
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      10.30.4.103/32 [20/0]
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 C        10.30.4.0/24
           directly connected, Vlan1304
 B E      100.0.1.203/32 [20/0]
           via VTEP 100.0.0.203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 C        100.0.1.204/32
           directly connected, Loopback100

```

## show ip arp vrf all

```text

VRF: default
Address         Age (sec)  Hardware Addr   Interface
20.200.204.200    0:00:03  444c.a873.5c75  Ethernet1

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.21.47     0:03:48  5c5a.c7ff.8a0a  Management1
192.168.21.50     0:01:04  a84f.b1a5.5221  Management1

VRF: tenant-a
Address         Age (sec)  Hardware Addr   Interface
10.10.203.203           -  001b.0100.0001  Vlan1203, Port-Channel200
10.30.1.14              -  f8c1.1604.3007  Vlan1301, Vxlan1
10.30.1.103             -  a244.0101.0001  Vlan1301, Vxlan1
10.30.3.14              -  f8c1.1604.3007  Vlan1303, Vxlan1
10.30.3.103             -  a266.0102.0001  Vlan1303, Vxlan1
10.30.3.203             -  001b.0100.0003  Vlan1303, Vxlan1
10.30.4.14              -  f8c1.1604.3007  Vlan1304, Vxlan1
10.30.4.103             -  a288.0103.0001  Vlan1304, Vxlan1
```

## show vxlan address-table

```text
          Vxlan Mac Address Table
----------------------------------------------------------------------

VLAN  Mac Address     Type      Prt  VTEP             Moves   Last Move
----  -----------     ----      ---  ----             -----   ---------
1301  001b.0100.0002  EVPN      Vx1  100.0.0.201      20      0:01:55 ago
                                     100.0.30.14    
1301  0056.5656.5656  EVPN      Vx1  100.0.0.201      1       0:10:10 ago
                                     100.0.30.14    
1301  a244.0101.0001  EVPN      Vx1  100.0.0.201      2       0:10:10 ago
                                     100.0.30.14    
1301  f8c1.1604.3007  EVPN      Vx1  100.0.0.201      1       0:10:10 ago
                                     100.0.30.14    
1302  0056.5656.5656  EVPN      Vx1  100.0.30.14      1       1:56:41 ago
1303  001b.0100.0003  EVPN      Vx1  100.0.30.14      12      0:03:25 ago
1303  0056.5656.5656  EVPN      Vx1  100.0.0.201      1       1:16:10 ago
                                     100.0.30.14    
1303  a266.0102.0001  EVPN      Vx1  100.0.0.201      3       1:16:10 ago
                                     100.0.30.14    
1303  f8c1.1604.3007  EVPN      Vx1  100.0.30.14      1       2:38:57 ago
1304  0056.5656.5656  EVPN      Vx1  100.0.0.201      1       1:16:10 ago
                                     100.0.30.14    
1304  a288.0103.0001  EVPN      Vx1  100.0.0.201      3       1:16:10 ago
                                     100.0.30.14    
1304  f8c1.1604.3007  EVPN      Vx1  100.0.30.14      1       2:38:57 ago
4093  c407.780a.9f31  EVPN      Vx1  100.0.30.14              7:19:13 ago
4094  2cdd.e90b.2283  EVPN      Vx1  100.0.0.201              21:01:50 ago
4094  2cdd.e90b.25b7  EVPN      Vx1  100.0.0.202              21:03:27 ago
4094  3838.a621.e82f  EVPN      Vx1  100.0.0.203              1 day, 4:59:53 ago
4094  c407.780a.9f31  EVPN      Vx1  100.0.30.14              1:56:41 ago
Total Remote Mac Addresses for this criterion: 17
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
1001       4093                      evpn         

```

## show mac address-table

```text
          Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports      Moves   Last Move
----    -----------       ----        -----      -----   ---------
1203    001b.0100.0001    DYNAMIC     Po200      1       0:20:58 ago
1203    00aa.aaaa.aaaa    STATIC      Router
1301    001b.0100.0002    DYNAMIC     Vx1        20      0:01:55 ago
1301    0056.5656.5656    STATIC      Vx1
1301    00aa.aaaa.aaaa    STATIC      Router
1301    00cc.cccc.bbbb    STATIC      Po200
1301    a244.0101.0001    DYNAMIC     Vx1        2       0:10:10 ago
1301    f8c1.1604.3007    STATIC      Vx1
1302    0056.5656.5656    STATIC      Vx1
1302    00aa.aaaa.aaaa    STATIC      Router
1303    001b.0100.0003    DYNAMIC     Vx1        12      0:03:25 ago
1303    0056.5656.5656    STATIC      Vx1
1303    00aa.aaaa.aaaa    STATIC      Router
1303    a266.0102.0001    DYNAMIC     Vx1        3       1:16:10 ago
1303    f8c1.1604.3007    STATIC      Vx1
1304    0056.5656.5656    STATIC      Vx1
1304    00aa.aaaa.aaaa    STATIC      Router
1304    a288.0103.0001    DYNAMIC     Vx1        3       1:16:10 ago
1304    f8c1.1604.3007    STATIC      Vx1
4093    00aa.aaaa.aaaa    STATIC      Router
4093    c407.780a.9f31    DYNAMIC     Vx1        0       7:19:14 ago
4094    00aa.aaaa.aaaa    STATIC      Router
4094    2cdd.e90b.2283    DYNAMIC     Vx1        0       21:01:50 ago
4094    2cdd.e90b.25b7    DYNAMIC     Vx1        0       21:03:27 ago
4094    3838.a621.e82f    DYNAMIC     Vx1        0       1 day, 4:59:54 ago
4094    c407.780a.9f31    DYNAMIC     Vx1        0       1:56:42 ago
Total Mac Addresses for this criterion: 26

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
f8c1.1604.3007, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 19: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.30.14
00aa.aaaa.aaaa, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 19: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.30.14
0056.5656.5656, VLAN 1303, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 19: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.30.14
f8c1.1604.3007, VLAN 1303, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.30.14
00aa.aaaa.aaaa, VLAN 1303, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 19: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.30.14
00aa.aaaa.aaaa, VLAN 1203, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.30.14
0056.5656.5656, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 19: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.30.14
00cc.cccc.bbbb, VLAN 1301, seq 1, pref 48, evpnIntfStaticMac, source: BGP
   Port-Channel200
a288.0103.0001, VLAN 1304, seq 3, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 19: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.30.14
a244.0101.0001, VLAN 1301, seq 2, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 19: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.30.14
0056.5656.5656, VLAN 1302, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.30.14
f8c1.1604.3007, VLAN 1304, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.30.14
00aa.aaaa.aaaa, VLAN 1304, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 19: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.30.14
001b.0100.0003, VLAN 1303, seq 12, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.30.14
001b.0100.0001, VLAN 1203, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
0056.5656.5656, VLAN 1304, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 19: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.30.14
a266.0102.0001, VLAN 1303, seq 3, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 19: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.30.14
001b.0100.0002, VLAN 1301, seq 20, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 19: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.30.14
```

## show vxlan flood vtep domain local

```text
          VXLAN Flood VTEP Table
--------------------------------------------------------------------------------

VLANS                            Ip Address
-----------------------------   ------------------------------------------------
1203,4094                       100.0.0.203    
1301,1303-1304                  100.0.0.22      100.0.0.201     100.0.0.203    
                                100.0.30.14    
1302                            100.0.0.22      100.0.0.201     100.0.0.203    
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
Router identifier 100.0.0.204, local AS number 65204
```

## show bgp evpn instance

```text
EVPN instance: SBD tenant-a
  Route distinguisher: 100.0.0.204:1000
  Route target import: Route-Target-AS:1000:1000
  Route target export: Route-Target-AS:1000:1000
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.204
  VXLAN: enabled
  MPLS: disabled
EVPN instance: VLAN 1203
  Route distinguisher: 100.0.0.204:1203
  Route target import: Route-Target-AS:1203:1203
  Route target export: Route-Target-AS:1203:1203
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.204
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
  Route distinguisher: 100.0.0.204:1301
  Route target import: Route-Target-AS:1301:1301
  Route target export: Route-Target-AS:1301:1301
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.204
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:1111:1111:1111:1111
    Active TEPs: 100.0.0.201, 100.0.30.14
    ESI: 0000:2222:2222:2222:1111
    Active TEPs: 100.0.30.14
    ESI: 0500:00ff:2200:0005:1500
    Active TEPs: 100.0.30.14
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
  Route distinguisher: 100.0.0.204:1302
  Route target import: Route-Target-AS:1302:1302
  Route target export: Route-Target-AS:1302:1302
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.204
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:1111:1111:1111:1111
    Active TEPs: 100.0.0.201
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
  Route distinguisher: 100.0.0.204:1303
  Route target import: Route-Target-AS:1303:1303
  Route target export: Route-Target-AS:1303:1303
  Service interface: VLAN-aware bundle
  Local VXLAN IP address: 100.0.0.204
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:1111:1111:1111:1111
    Active TEPs: 100.0.0.201, 100.0.30.14
    ESI: 0000:2222:2222:2222:1111
    Active TEPs: 100.0.30.14
    ESI: 0500:00ff:2200:0005:1700
    Active TEPs: 100.0.30.14
    ESI: 0500:00ff:2200:0005:1800
    Active TEPs: 100.0.30.14
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
Ma1                    0:05      0.1   0.0%        0      0.2   0.0%        0
```

