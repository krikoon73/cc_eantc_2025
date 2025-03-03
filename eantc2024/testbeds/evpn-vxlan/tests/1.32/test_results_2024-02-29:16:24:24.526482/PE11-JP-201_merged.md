# Test results for PE11-JP-201

## show hostname

```text
Hostname: PE11-JP-201
FQDN:     PE11-JP-201.ns.eantc.de
```

## show ip bgp summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.201, local AS number 65201
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.201, local AS number 65201
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  NODE200.EVPN             2000::200 4 65000           8367      2492    0    0    1d00h Estab   214    214
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.201, local AS number 65201
BGP routing table entry for auto-discovery 0 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
BGP routing table entry for auto-discovery 0 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 0 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1022
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
BGP routing table entry for auto-discovery 0 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1301
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1302
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1303
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1304
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1022
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1301
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1302
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1303
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1304
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
BGP routing table entry for auto-discovery 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0 0011:1111:2222:2211:1111, Route Distinguisher: 100.0.3.41:3311
 Paths: 1 available
  65000 64512
    100.0.3.41 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:3301:3301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:00:00:00:00:00
      VNI: 3301
BGP routing table entry for auto-discovery 0011:1111:2222:2211:1111, Route Distinguisher: 100.0.3.41:1
 Paths: 1 available
  65000 65056 64512
    100.0.3.41 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:3301:64514 EvpnEsiLabel:24002
      VNI: 0
BGP routing table entry for auto-discovery 0011:1111:2222:2211:1111, Route Distinguisher: 100.0.3.41:2
 Paths: 1 available
  65000 64512
    100.0.3.41 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:3301:3301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:24002 1111:0x11 0x11 0x11 0x00 0x00 0x00
      VNI: 0
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.201, local AS number 65201
BGP routing table entry for mac-ip 0000.0181.0181, Route Distinguisher: 100.0.3.41:3311
 Paths: 1 available
  65000 64512
    100.0.3.41 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Community: 1:5641
      Extended Community: Route-Target-AS:3301:3301 TunnelEncap:tunnelTypeVxlan TunnelEncap:tunnelTypeMpls EvpnMacMobility:sticky EvpnRouterMac:00:00:00:00:00:00
      VNI: 3301 ESI: 0011:1111:2222:2211:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 0000.0206.0206, Route Distinguisher: 100.0.0.206:3301
 Paths: 1 available
  65000 65206
    100.0.0.206 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:3301:3301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 3301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0020.1000.0001, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0001 1000:3000:1::201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0001 1000:3000:1::201, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0002, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0002, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0002 1000:3000:2::201, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0002 1000:3000:2::201, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0005, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0005 1000:1000:201::201, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1201:1201 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan
      VNI: 1201 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0005 1000:1000:201::201, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7 EvpnNdFlags:pflag
      VNI: 1201 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.3000.0001, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0001 1000:3000:1::203, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0001 1000:3000:1::203, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0002, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0002 1000:3000:2::203, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0002 1000:3000:2::203, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0005, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0005 1000:1000:203::203, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f EvpnNdFlags:pflag
      VNI: 1203 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0005 1000:1000:203::203, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1203 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0022.0000.0001, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 0022.0000.0001 1000:3000:1::22, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31 EvpnNdFlags:oflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 0022.0000.0002, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 0022.0000.0005, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 0022.0000.0005 1000:1000:22::22, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1022 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 0022.0000.0005 fe80::222:ff:fe00:5, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1022 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 0040.0100.0001, Route Distinguisher: 100.0.0.40:34068
 Paths: 1 available
  65000 65040
    2000::40 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0040.0100.0001 1000:3000:1::40, Route Distinguisher: 100.0.0.40:34068
 Paths: 1 available
  65000 65040
    2000::40 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0040.0100.0001 1000:3000:1:0:240:1ff:fe00:1, Route Distinguisher: 100.0.0.40:34068
 Paths: 1 available
  65000 65040
    2000::40 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0040.0100.0002, Route Distinguisher: 100.0.0.40:34069
 Paths: 1 available
  65000 65040
    2000::40 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0040.0100.0002 1000:3000:2::40, Route Distinguisher: 100.0.0.40:34069
 Paths: 1 available
  65000 65040
    2000::40 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0040.0100.0002 1000:3000:2:0:240:1ff:fe00:2, Route Distinguisher: 100.0.0.40:34069
 Paths: 1 available
  65000 65040
    2000::40 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0040.0100.0003, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65000 65040
    2000::40 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan
      VNI: 1040 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0040.0100.0003 1000:1000:40::40, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65000 65040
    2000::40 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1040 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0040.0100.0003 1000:1000:40:0:240:1ff:fe00:3, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65000 65040
    2000::40 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1040 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0001, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0001 1000:3000:1::56, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0001 fe80::256:ff:fe00:1, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0002, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0002 1000:3000:2::56, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0002 fe80::256:ff:fe00:2, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0005, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0005 1000:1000:56::56, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0005 fe80::256:ff:fe00:5, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.56.254, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.2.254, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 1000:1000:56::254, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 1000:3000:1::254, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 1000:3000:2::254, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa fe80::2aa:aaff:feaa:aaaa, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa fe80::2aa:aaff:feaa:aaaa, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa fe80::2aa:aaff:feaa:aaaa, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 0020.1000.0003, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0020.1000.0003, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0020.1000.0003 1000:3000:3::201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0020.1000.0003 1000:3000:3::201, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0020.3000.0003, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0020.3000.0003 1000:3000:3::203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0020.3000.0003 1000:3000:3::203, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0022.0000.0003, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 1303 0022.0000.0003 1000:3000:3::22, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31 EvpnNdFlags:oflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 1303 0022.0000.0003 fe80::222:ff:fe00:3, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 1303 0056.0000.0003, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 0056.0000.0003 1000:3000:3::56, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 0056.0000.0003 fe80::256:ff:fe00:3, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 1000:3000:3::254, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa fe80::2aa:aaff:feaa:aaaa, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 0020.1000.0004, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0020.1000.0004, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0020.1000.0004 1000:3000:4::201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0020.1000.0004 1000:3000:4::201, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0020.3000.0004, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 0020.3000.0004 1000:3000:4::203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 0020.3000.0004 1000:3000:4::203, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 0022.0000.0004, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 1304 0022.0000.0004 1000:3000:4::22, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31 EvpnNdFlags:oflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 1304 0022.0000.0004 fe80::222:ff:fe00:4, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 1304 0056.0000.0004, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 0056.0000.0004 1000:3000:4::56, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 0056.0000.0004 fe80::256:ff:fe00:4, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 1000:3000:4::254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa fe80::2aa:aaff:feaa:aaaa, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
```

## show bgp evpn route-type imet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.201, local AS number 65201
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
      PMSI Tunnel: Ingress Replication, MPLS Label: 1022, Leaf Information Required: false, Tunnel ID: 2000::22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::22
BGP routing table entry for imet 100.0.0.23, Route Distinguisher: 100.0.0.23:1022
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
      PMSI Tunnel: Ingress Replication, MPLS Label: 1022, Leaf Information Required: false, Tunnel ID: 2000::23
BGP routing table entry for imet 100.0.0.23, Route Distinguisher: 100.0.0.23:1301
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::23
BGP routing table entry for imet 100.0.0.23, Route Distinguisher: 100.0.0.23:1302
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::23
BGP routing table entry for imet 100.0.0.206, Route Distinguisher: 100.0.0.206:3301
 Paths: 1 available
  65000 65206
    100.0.0.206 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:3301:3301 TunnelEncap:tunnelTypeVxlan
      VNI: 3301
      PMSI Tunnel: Ingress Replication, MPLS Label: 3301, Leaf Information Required: false, Tunnel ID: 100.0.0.206
BGP routing table entry for imet 100.0.3.41, Route Distinguisher: 100.0.3.41:3311
 Paths: 1 available
  65000 64512
    100.0.3.41 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:3301:3301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:00:00:00:00:00 L2 Attributes: control word
      VNI: 3301
      PMSI Tunnel: Ingress Replication, MPLS Label: 3301, Leaf Information Required: false, Tunnel ID: 100.0.3.41
BGP routing table entry for imet 2000::40, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65000 65040
    2000::40 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan
      VNI: 1040
      PMSI Tunnel: Ingress Replication, MPLS Label: 1040, Leaf Information Required: false, Tunnel ID: 2000::40
BGP routing table entry for imet 2000::40, Route Distinguisher: 100.0.0.40:34068
 Paths: 1 available
  65000 65040
    2000::40 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::40
BGP routing table entry for imet 2000::40, Route Distinguisher: 100.0.0.40:34069
 Paths: 1 available
  65000 65040
    2000::40 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::40
BGP routing table entry for imet 2000::56, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan
      VNI: 1056
      PMSI Tunnel: Ingress Replication, MPLS Label: 1056, Leaf Information Required: false, Tunnel ID: 2000::56
BGP routing table entry for imet 2000::56, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::56
BGP routing table entry for imet 2000::56, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::56
BGP routing table entry for imet 2000::201, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
      PMSI Tunnel: Ingress Replication, MPLS Label: 1201, Leaf Information Required: false, Tunnel ID: 2000::201
BGP routing table entry for imet 2000::201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::201
BGP routing table entry for imet 2000::201, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::201
BGP routing table entry for imet 2000::202, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
      PMSI Tunnel: Ingress Replication, MPLS Label: 1201, Leaf Information Required: false, Tunnel ID: 2000::202
BGP routing table entry for imet 2000::202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::202
BGP routing table entry for imet 2000::202, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::202
BGP routing table entry for imet 2000::203, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
      PMSI Tunnel: Ingress Replication, MPLS Label: 1203, Leaf Information Required: false, Tunnel ID: 2000::203
BGP routing table entry for imet 2000::203, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::203
BGP routing table entry for imet 2000::203, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::203
BGP routing table entry for imet 2000::204, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
      PMSI Tunnel: Ingress Replication, MPLS Label: 1203, Leaf Information Required: false, Tunnel ID: 2000::204
BGP routing table entry for imet 2000::204, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::204
BGP routing table entry for imet 2000::204, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::204
BGP routing table entry for imet 1303 100.0.0.22, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 2000::22
BGP routing table entry for imet 1303 100.0.0.23, Route Distinguisher: 100.0.0.23:1303
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 2000::23
BGP routing table entry for imet 1303 2000::56, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 2000::56
BGP routing table entry for imet 1303 2000::201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 2000::201
BGP routing table entry for imet 1303 2000::202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 2000::202
BGP routing table entry for imet 1303 2000::203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 2000::203
BGP routing table entry for imet 1303 2000::204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 2000::204
BGP routing table entry for imet 1304 100.0.0.22, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 2000::22
BGP routing table entry for imet 1304 100.0.0.23, Route Distinguisher: 100.0.0.23:1304
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 2000::23
BGP routing table entry for imet 1304 2000::56, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 2000::56
BGP routing table entry for imet 1304 2000::201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 2000::201
BGP routing table entry for imet 1304 2000::202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 2000::202
BGP routing table entry for imet 1304 2000::203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 2000::203
BGP routing table entry for imet 1304 2000::204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 2000::204
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.201, local AS number 65201
BGP routing table entry for ethernet-segment 0000:0000:0000:0022:0023 100.0.0.22, Route Distinguisher: 100.0.0.22:0
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: EvpnEsImportRt:00:00:00:00:00:00 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0022:0023 100.0.0.23, Route Distinguisher: 100.0.0.23:0
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: EvpnEsImportRt:00:00:00:00:00:00 DF Election: Preference 100
BGP routing table entry for ethernet-segment 0000:0000:0000:0201:0202 2000::201, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:10:02:02 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0201:0202 2000::202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:10:02:02 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0203:0204 2000::203, Route Distinguisher: 100.0.0.203:1
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:30:02:04 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0203:0204 2000::204, Route Distinguisher: 100.0.0.204:1
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:30:02:04 DF Election: Preference 100
BGP routing table entry for ethernet-segment 0011:1111:2222:2211:1111 100.0.3.41, Route Distinguisher: 100.0.3.41:0
 Paths: 1 available
  65000 64512
    100.0.3.41 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: EvpnEsImportRt:11:11:11:22:22:22 DF Election: Modulus-based
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.201, local AS number 65201
BGP routing table entry for ip-prefix 10.10.56.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 30.30.1.0/24, Route Distinguisher: 100.0.3.41:0
 Paths: 1 available
  65000 64512
    100.0.3.41 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Community: 1:5641
      Extended Community: Route-Target-AS:1023:1023 TunnelEncap:tunnelTypeVxlan TunnelEncap:tunnelTypeMpls EvpnRouterMac:f8:7a:41:6d:d0:f0
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 30.30.2.0/24, Route Distinguisher: 100.0.3.41:0
 Paths: 1 available
  65000 64512
    100.0.3.41 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Community: 1:5641
      Extended Community: Route-Target-AS:1023:1023 TunnelEncap:tunnelTypeVxlan TunnelEncap:tunnelTypeMpls EvpnRouterMac:f8:7a:41:6d:d0:f0
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 30.30.5.0/24, Route Distinguisher: 100.0.0.206:1023
 Paths: 1 available
  65000 65206
    100.0.0.206 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1023:1023 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:c4:02:71
      VNI: 1023
```

## show bgp evpn route-type smet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.201, local AS number 65201
```

## show bgp evpn route-type spmsi detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.201, local AS number 65201
```

## show bgp evpn arp

```text
VLAN  Label  Encap IP                 MAC             Tunnel Endpoint    Seq#
----- ------ ----- ------------------ --------------- ------------------ ----
0     1022   VXLAN 1000:1000:22::22   0022.0000.0005  2000::22           -   
0     1022   VXLAN 1000:1000:22::22   0022.0000.0005  2000::22           -   
0     1022   VXLAN fe80::222:ff:fe00: 0022.0000.0005  2000::22           -   
                   5                                                         
0     1022   VXLAN fe80::222:ff:fe00: 0022.0000.0005  2000::22           -   
                   5                                                         
1201  1201   VXLAN 1000:1000:201::201 0020.1000.0005  Local              -   
1201  1201   VXLAN 1000:1000:201::201 0020.1000.0005  2000::202          -   
1301  1301   VXLAN 1000:3000:1::22    0022.0000.0001  2000::22           -   
1301  1301   VXLAN 1000:3000:1::45    0045.0100.0001  2000::100          -   
1301  1301   VXLAN 10.30.1.254        00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1301  1301   VXLAN 1000:3000:1::254   00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1301  1301   VXLAN 1000:3000:1::42    0042.0100.0001  2000::42           -   
1301  1301   VXLAN 1000:3000:1:0:242: 0042.0100.0001  2000::42           -   
                   1ff:fe00:1                                                
1301  1301   VXLAN fe80::2aa:aaff:fea 00aa.aaaa.aaaa  2000::56           Stic
                   a:aaaa                                                ky  
1301  1301   VXLAN fe80::222:ff:fe00: 0022.0000.0001  2000::22           -   
                   1                                                         
1301  1301   VXLAN 1000:3000:1:0:245: 0045.0100.0001  2000::100          -   
                   1ff:fe00:1                                                
1301  1301   VXLAN 1000:3000:1::203   0020.3000.0001  2000::204          -   
1301  1301   VXLAN 1000:3000:1::203   0020.3000.0001  2000::203          -   
1301  1301   VXLAN 1000:3000:1::22    0022.0000.0001  2000::22           -   
1301  1301   VXLAN 1000:3000:1::40    0040.0100.0001  2000::40           -   
1301  1301   VXLAN 1000:3000:1::56    0056.0000.0001  2000::56           -   
1301  1301   VXLAN fe80::256:ff:fe00: 0056.0000.0001  2000::56           -   
                   1                                                         
1301  1301   VXLAN 1000:3000:1:0:240: 0040.0100.0001  2000::40           -   
                   1ff:fe00:1                                                
1301  1301   VXLAN 1000:3000:1::201   0020.1000.0001  Local              -   
1301  1301   VXLAN 1000:3000:1::201   0020.1000.0001  2000::202          -   
1302  1302   VXLAN 1000:3000:2::201   0020.1000.0002  2000::202          -   
1302  1302   VXLAN 1000:3000:2::201   0020.1000.0002  Local              -   
1302  1302   VXLAN fe80::222:ff:fe00: 0022.0000.0002  2000::22           -   
                   2                                                         
1302  1302   VXLAN 1000:3000:2::22    0022.0000.0002  2000::22           -   
1302  1302   VXLAN fe80::256:ff:fe00: 0056.0000.0002  2000::56           -   
                   2                                                         
1302  1302   VXLAN 1000:3000:2::56    0056.0000.0002  2000::56           -   
1302  1302   VXLAN 1000:3000:2::203   0020.3000.0002  2000::203          -   
1302  1302   VXLAN 1000:3000:2::203   0020.3000.0002  2000::204          -   
1302  1302   VXLAN 1000:3000:2::254   00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1302  1302   VXLAN 10.30.2.254        00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1302  1302   VXLAN 1000:3000:2::22    0022.0000.0002  2000::22           -   
1302  1302   VXLAN fe80::222:ff:fe00: 0022.0000.0002  2000::22           -   
                   2                                                         
1302  1302   VXLAN fe80::2aa:aaff:fea 00aa.aaaa.aaaa  2000::56           Stic
                   a:aaaa                                                ky  
1302  1302   VXLAN 1000:3000:2::40    0040.0100.0002  2000::40           -   
1302  1302   VXLAN 1000:3000:2:0:240: 0040.0100.0002  2000::40           -   
                   1ff:fe00:2                                                
1303  1303   VXLAN 1000:3000:3::203   0020.3000.0003  2000::204          -   
1303  1303   VXLAN 1000:3000:3::203   0020.3000.0003  2000::203          -   
1303  1303   VXLAN 1000:3000:3::201   0020.1000.0003  Local              -   
1303  1303   VXLAN 1000:3000:3::201   0020.1000.0003  2000::202          -   
1303  1303   VXLAN fe80::222:ff:fe00: 0022.0000.0003  2000::22           -   
                   3                                                         
1303  1303   VXLAN fe80::2aa:aaff:fea 00aa.aaaa.aaaa  2000::56           Stic
                   a:aaaa                                                ky  
1303  1303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1303  1303   VXLAN 1000:3000:3::22    0022.0000.0003  2000::22           -   
1303  1303   VXLAN 1000:3000:3::56    0056.0000.0003  2000::56           -   
1303  1303   VXLAN fe80::256:ff:fe00: 0056.0000.0003  2000::56           -   
                   3                                                         
1303  1303   VXLAN 1000:3000:3::254   00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1304  1304   VXLAN 1000:3000:4::22    0022.0000.0004  2000::22           -   
1304  1304   VXLAN fe80::256:ff:fe00: 0056.0000.0004  2000::56           -   
                   4                                                         
1304  1304   VXLAN 1000:3000:4::201   0020.1000.0004  Local              -   
1304  1304   VXLAN 1000:3000:4::201   0020.1000.0004  2000::202          -   
1304  1304   VXLAN 1000:3000:4::254   00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1304  1304   VXLAN fe80::222:ff:fe00: 0022.0000.0004  2000::22           -   
                   4                                                         
1304  1304   VXLAN 10.30.4.254        00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1304  1304   VXLAN 1000:3000:4::203   0020.3000.0004  2000::204          -   
1304  1304   VXLAN 1000:3000:4::203   0020.3000.0004  2000::203          -   
1304  1304   VXLAN fe80::2aa:aaff:fea 00aa.aaaa.aaaa  2000::56           Stic
                   a:aaaa                                                ky  
1304  1304   VXLAN 1000:3000:4::56    0056.0000.0004  2000::56           -   
0     2303   VXLAN 10.30.3.254        0056.5656.5656  100.0.0.56         Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.254        0056.5656.5656  100.0.0.56         Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.203        001b.0100.0003  100.0.30.14        -   
0     2303   VXLAN 10.30.3.254        0056.5656.5656  100.0.30.14        Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.0.56         Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.0.56         Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.203        001b.0100.0003  100.0.30.14        -   
1303  1303   VXLAN 10.30.3.203        001b.0100.0003  100.0.30.14        -   
0     2303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.30.14        Stic
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

 B E      10.10.56.0/24 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 C        10.10.201.0/24
           directly connected, Vlan1201
 B E      10.10.203.0/24 [20/0]
           via VTEP 2000::204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 2000::203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 C        10.30.1.0/24
           directly connected, Vlan1301
 C        10.30.2.0/24
           directly connected, Vlan1302
 C        10.30.3.0/24
           directly connected, Vlan1303
 C        10.30.4.0/24
           directly connected, Vlan1304

```

## show ip arp vrf all

```text

VRF: default
Address         Age (sec)  Hardware Addr   Interface

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.20.2      0:03:57  bcea.fa02.6ce2  Management1
192.168.20.19     0:00:30  c407.7858.8001  Management1
192.168.20.23     0:04:03  c407.780a.7750  Management1
192.168.20.24     0:03:39  6c87.2089.ede5  Management1
192.168.20.26     0:00:48  04a9.59d5.df66  Management1
192.168.20.27     0:02:13  04a9.59d5.dfe6  Management1
192.168.20.28     0:02:19  98a9.2d59.bae6  Management1
192.168.20.29     0:02:31  90f7.b223.d466  Management1
192.168.20.183    0:00:48  c4ca.2b45.ef6c  Management1
192.168.20.200    0:00:42  444c.a873.5c74  Management1
192.168.21.50     0:03:39  a84f.b1a5.5221  Management1
192.168.21.59     0:03:02  6607.f5d1.ae16  Management1

VRF: tenant-a
Address         Age (sec)  Hardware Addr   Interface
```

## show vxlan address-table

```text
          Vxlan Mac Address Table
----------------------------------------------------------------------

VLAN  Mac Address     Type      Prt  VTEP             Moves   Last Move
----  -----------     ----      ---  ----             -----   ---------
1301  0020.3000.0001  EVPN      Vx1  2000::203        1       0:11:08 ago
                                     2000::204      
1301  0022.0000.0001  EVPN      Vx1  2000::22         3       0:00:31 ago
                                     2000::23       
1301  0040.0100.0001  EVPN      Vx1  2000::40         1       0:25:40 ago
1301  0056.0000.0001  EVPN      Vx1  2000::56         1       0:52:41 ago
1302  0020.3000.0002  EVPN      Vx1  2000::203        1       0:26:09 ago
                                     2000::204      
1302  0022.0000.0002  EVPN      Vx1  2000::22         2       0:00:31 ago
                                     2000::23       
1302  0040.0100.0002  EVPN      Vx1  2000::40         1       0:25:40 ago
1302  0056.0000.0002  EVPN      Vx1  2000::56         1       0:52:41 ago
1303  0020.3000.0003  EVPN      Vx1  2000::203        1       0:11:08 ago
                                     2000::204      
1303  0022.0000.0003  EVPN      Vx1  2000::22         4       0:00:31 ago
                                     2000::23       
1303  0056.0000.0003  EVPN      Vx1  2000::56         1       0:52:41 ago
1304  0020.3000.0004  EVPN      Vx1  2000::203        1       0:26:08 ago
                                     2000::204      
1304  0022.0000.0004  EVPN      Vx1  2000::22         4       0:00:31 ago
                                     2000::23       
1304  0056.0000.0004  EVPN      Vx1  2000::56         1       0:52:41 ago
Total Remote Mac Addresses for this criterion: 14
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
1201    0020.1000.0005    DYNAMIC     Po100      1       0:02:25 ago
1201    00aa.aaaa.aaaa    STATIC      Router
1201    2cdd.e90b.2283    STATIC      Router
1301    0020.1000.0001    DYNAMIC     Po100      1       0:02:46 ago
1301    0020.3000.0001    DYNAMIC     Vx1        1       0:11:08 ago
1301    0022.0000.0001    DYNAMIC     Vx1        3       0:00:31 ago
1301    0040.0100.0001    DYNAMIC     Vx1        1       0:25:40 ago
1301    0056.0000.0001    DYNAMIC     Vx1        1       0:52:41 ago
1301    00aa.aaaa.aaaa    STATIC      Router
1301    2cdd.e90b.2283    STATIC      Router
1302    0020.1000.0002    DYNAMIC     Po100      2       0:02:24 ago
1302    0020.3000.0002    DYNAMIC     Vx1        1       0:26:09 ago
1302    0022.0000.0002    DYNAMIC     Vx1        2       0:00:31 ago
1302    0040.0100.0002    DYNAMIC     Vx1        1       0:25:40 ago
1302    0056.0000.0002    DYNAMIC     Vx1        1       0:52:41 ago
1302    00aa.aaaa.aaaa    STATIC      Router
1302    2cdd.e90b.2283    STATIC      Router
1303    0020.1000.0003    DYNAMIC     Po100      2       0:02:24 ago
1303    0020.3000.0003    DYNAMIC     Vx1        1       0:11:08 ago
1303    0022.0000.0003    DYNAMIC     Vx1        4       0:00:31 ago
1303    0056.0000.0003    DYNAMIC     Vx1        1       0:52:41 ago
1303    00aa.aaaa.aaaa    STATIC      Router
1303    2cdd.e90b.2283    STATIC      Router
1304    0020.1000.0004    DYNAMIC     Po100      1       0:02:46 ago
1304    0020.3000.0004    DYNAMIC     Vx1        1       0:26:08 ago
1304    0022.0000.0004    DYNAMIC     Vx1        4       0:00:31 ago
1304    0056.0000.0004    DYNAMIC     Vx1        1       0:52:41 ago
1304    00aa.aaaa.aaaa    STATIC      Router
1304    2cdd.e90b.2283    STATIC      Router
4094    00aa.aaaa.aaaa    STATIC      Router
4094    2cdd.e90b.2283    STATIC      Router
Total Mac Addresses for this criterion: 31

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
00aa.aaaa.aaaa, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 2000::56
0020.3000.0004, VLAN 1304, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 322: 2-way
      VTEP 2000::203
      VTEP 2000::204
0056.0000.0004, VLAN 1304, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::56
00aa.aaaa.aaaa, VLAN 1303, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 2000::56
0056.0000.0001, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::56
0020.3000.0002, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 322: 2-way
      VTEP 2000::203
      VTEP 2000::204
0022.0000.0001, VLAN 1301, seq 3, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 324: 2-way
      VTEP 2000::22
      VTEP 2000::23
0022.0000.0004, VLAN 1304, seq 4, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 324: 2-way
      VTEP 2000::22
      VTEP 2000::23
0020.3000.0003, VLAN 1303, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 322: 2-way
      VTEP 2000::203
      VTEP 2000::204
0022.0000.0003, VLAN 1303, seq 4, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 324: 2-way
      VTEP 2000::22
      VTEP 2000::23
0022.0000.0002, VLAN 1302, seq 2, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 324: 2-way
      VTEP 2000::22
      VTEP 2000::23
0040.0100.0002, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::40
0020.1000.0001, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0020.3000.0001, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 322: 2-way
      VTEP 2000::203
      VTEP 2000::204
0020.1000.0005, VLAN 1201, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel100
0056.0000.0002, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::56
0020.1000.0004, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
00aa.aaaa.aaaa, VLAN 1304, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 2000::56
00aa.aaaa.aaaa, VLAN 1302, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 2000::56
0056.0000.0003, VLAN 1303, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::56
0040.0100.0001, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::40
0020.1000.0003, VLAN 1303, seq 2, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0020.1000.0002, VLAN 1302, seq 2, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
```

## show vxlan flood vtep domain local

```text
          VXLAN Flood VTEP Table
--------------------------------------------------------------------------------

VLANS                            Ip Address
-----------------------------   ------------------------------------------------
1201                            2000::202      
1301-1302                       2000::22        2000::23        2000::40       
                                2000::56        2000::202       2000::203      
                                2000::204      
1303-1304                       2000::22        2000::23        2000::56       
                                2000::202       2000::203       2000::204      
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
Router identifier 100.0.0.201, local AS number 65201
```

## show bgp evpn instance

```text
EVPN instance: VLAN 1201
  Route distinguisher: 100.0.0.201:1201
  Route target import: Route-Target-AS:1201:1201
  Route target export: Route-Target-AS:1201:1201
  Service interface: VLAN-based
  Local VXLAN IP address: 2000::201
  VXLAN: enabled
  MPLS: disabled
  Local ethernet segment:
    ESI: 0000:0000:0000:0201:0202
      Interface: Port-Channel100
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:10:02:02
      DF election algorithm: preference
      Designated forwarder: 2000::201
      Non-Designated forwarder: 2000::202
EVPN instance: VLAN 1301
  Route distinguisher: 100.0.0.201:1301
  Route target import: Route-Target-AS:1301:1301
  Route target export: Route-Target-AS:1301:1301
  Service interface: VLAN-based
  Local VXLAN IP address: 2000::201
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:0000:0000:0022:0023
    Active TEPs: 2000::22, 2000::23
    ESI: 0000:0000:0000:0203:0204
    Active TEPs: 2000::203, 2000::204
  Local ethernet segment:
    ESI: 0000:0000:0000:0201:0202
      Interface: Port-Channel100
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:10:02:02
      DF election algorithm: preference
      Designated forwarder: 2000::201
      Non-Designated forwarder: 2000::202
EVPN instance: VLAN 1302
  Route distinguisher: 100.0.0.201:1302
  Route target import: Route-Target-AS:1302:1302
  Route target export: Route-Target-AS:1302:1302
  Service interface: VLAN-based
  Local VXLAN IP address: 2000::201
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:0000:0000:0022:0023
    Active TEPs: 2000::22, 2000::23
    ESI: 0000:0000:0000:0203:0204
    Active TEPs: 2000::203, 2000::204
  Local ethernet segment:
    ESI: 0000:0000:0000:0201:0202
      Interface: Port-Channel100
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:10:02:02
      DF election algorithm: preference
      Designated forwarder: 2000::201
      Non-Designated forwarder: 2000::202
EVPN instance: VLAN-aware bundle 1303-1304
  Route distinguisher: 100.0.0.201:1303
  Route target import: Route-Target-AS:1303:1303
  Route target export: Route-Target-AS:1303:1303
  Service interface: VLAN-aware bundle
  Local VXLAN IP address: 2000::201
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:0000:0000:0022:0023
    Active TEPs: 2000::22, 2000::23
    ESI: 0000:0000:0000:0203:0204
    Active TEPs: 2000::203, 2000::204
  Local ethernet segment:
    ESI: 0000:0000:0000:0201:0202
      Interface: Port-Channel100
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:10:02:02
      DF election algorithm: preference
      Designated forwarder: 2000::201
      Non-Designated forwarder: 2000::202
```

## show ipv6 interface brief

```text
Interface  Status    MTU  IPv6 Address                  Addr State  Addr Source
---------- ------- ------ ----------------------------- ----------- -----------
Et1        up       1500  fe80::2edd:e9ff:fe0b:2283/64  up          link local 
Lo0        up      65535  fe80::ff:fe00:0/64            up          link local 
                          2000::201/128                 up          config     
Vl1201     up       1500  fe80::2edd:e9ff:fe0b:2283/64  up          link local 
                          1000:1000:201::254/64         up          config     
Vl1301     up       1500  fe80::2edd:e9ff:fe0b:2283/64  up          link local 
                          1000:3000:1::254/64           up          config     
Vl1302     up       1500  fe80::2edd:e9ff:fe0b:2283/64  up          link local 
                          1000:3000:2::254/64           up          config     
Vl1303     up       1500  fe80::2edd:e9ff:fe0b:2283/64  up          link local 
                          1000:3000:3::254/64           up          config     
Vl1304     up       1500  fe80::2edd:e9ff:fe0b:2283/64  up          link local 
                          1000:3000:4::254/64           up          config     
Vl4094     up      10168  fe80::2edd:e9ff:fe0b:2283/64  up          link local 

```

## show ipv6 bgp summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.201, local AS number 65201
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor                      V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
                           fe80::464c:a8ff:fe73:5c75%Et1 4 65000           2046      1948    0    0    1d00h Estab   9      9
```

## show ipv6 bgp

```text
BGP routing table information for VRF default
Router identifier 100.0.0.201, local AS number 65201
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
RPKI Origin Validation codes: V - valid, I - invalid, U - unknown
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
 * >      2000::22/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65022 i
 * >      2000::23/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65023 i
 * >      2000::40/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65040 ?
 * >      2000::56/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65056 ?
 * >      2000::200/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 i
 * >      2000::201/128          -                     -       -          -       0       i
 * >      2000::202/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65202 i
 * >      2000::203/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65203 i
 * >      2000::204/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65204 i
 * >      2001::56/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65056 i
```

## show ipv6 route

```text

VRF: default
Displaying 10 of 13 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 B E      2000::22/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::23/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::40/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::56/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::200/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 C        2000::201/128 [0/0]
           via Loopback0, directly connected
 B E      2000::202/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::203/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::204/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2001::56/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1

```

## show ipv6 bgp vrf all

```text
BGP routing table information for VRF default
Router identifier 100.0.0.201, local AS number 65201
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
RPKI Origin Validation codes: V - valid, I - invalid, U - unknown
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
 * >      2000::22/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65022 i
 * >      2000::23/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65023 i
 * >      2000::40/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65040 ?
 * >      2000::56/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65056 ?
 * >      2000::200/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 i
 * >      2000::201/128          -                     -       -          -       0       i
 * >      2000::202/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65202 i
 * >      2000::203/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65203 i
 * >      2000::204/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65204 i
 * >      2001::56/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65056 i
BGP routing table information for VRF tenant-a
Router identifier 100.0.1.201, local AS number 65201
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
RPKI Origin Validation codes: V - valid, I - invalid, U - unknown
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
 * >Ec    1000:1000:22::/64      2000::22              0       -          100     0       65000 65022 i
 *  ec    1000:1000:22::/64      2000::23              0       -          100     0       65000 65023 i
 * >      1000:1000:22::22/128   2000::22              0       -          100     0       65000 65022 i
 * >Ec    1000:1000:22::254/128  2000::22              0       -          100     0       65000 65022 i
 *  ec    1000:1000:22::254/128  2000::23              0       -          100     0       65000 65023 i
 * >      1000:1000:40::/64      2000::40              0       -          100     0       65000 65040 ?
 * >      1000:1000:40::40/128   2000::40              0       -          100     0       65000 65040 i
 * >      1000:1000:40:0:240:1ff:fe00:3/128 2000::40              0       -          100     0       65000 65040 i
 * >      1000:1000:56::/64      2000::56              0       -          100     0       65000 65056 i
 * >      1000:1000:56::56/128   2000::56              0       -          100     0       65000 65056 i
 * >      1000:1000:201::/64     -                     -       -          -       0       i
 *        1000:1000:201::/64     2000::202             0       -          100     0       65000 65202 i
          1000:1000:201::201/128 2000::202             0       -          100     0       65000 65202 i
 * >Ec    1000:1000:203::/64     2000::204             0       -          100     0       65000 65204 i
 *  ec    1000:1000:203::/64     2000::203             0       -          100     0       65000 65203 i
 * >Ec    1000:1000:203::203/128 2000::203             0       -          100     0       65000 65203 i
 *  ec    1000:1000:203::203/128 2000::204             0       -          100     0       65000 65204 i
 * >      1000:3000:1::/64       -                     -       -          -       0       i
 *  Ec    1000:3000:1::/64       2000::203             0       -          100     0       65000 65203 i
 *  ec    1000:3000:1::/64       2000::202             0       -          100     0       65000 65202 i
 *  ec    1000:3000:1::/64       2000::204             0       -          100     0       65000 65204 i
 *  ec    1000:3000:1::/64       2000::56              0       -          100     0       65000 65056 i
 *        1000:3000:1::/64       2000::40              0       -          100     0       65000 65040 ?
 * >      1000:3000:1::22/128    2000::22              0       -          100     0       65000 65022 i
 * >      1000:3000:1::40/128    2000::40              0       -          100     0       65000 65040 i
 * >      1000:3000:1::56/128    2000::56              0       -          100     0       65000 65056 i
          1000:3000:1::201/128   2000::202             0       -          100     0       65000 65202 i
 * >Ec    1000:3000:1::203/128   2000::204             0       -          100     0       65000 65204 i
 *  ec    1000:3000:1::203/128   2000::203             0       -          100     0       65000 65203 i
 * >      1000:3000:1:0:240:1ff:fe00:1/128 2000::40              0       -          100     0       65000 65040 i
 * >      1000:3000:2::/64       -                     -       -          -       0       i
 *  Ec    1000:3000:2::/64       2000::204             0       -          100     0       65000 65204 i
 *  ec    1000:3000:2::/64       2000::202             0       -          100     0       65000 65202 i
 *  ec    1000:3000:2::/64       2000::203             0       -          100     0       65000 65203 i
 *  ec    1000:3000:2::/64       2000::56              0       -          100     0       65000 65056 i
 *        1000:3000:2::/64       2000::40              0       -          100     0       65000 65040 ?
 * >      1000:3000:2::40/128    2000::40              0       -          100     0       65000 65040 i
 * >      1000:3000:2::56/128    2000::56              0       -          100     0       65000 65056 i
          1000:3000:2::201/128   2000::202             0       -          100     0       65000 65202 i
 * >Ec    1000:3000:2::203/128   2000::203             0       -          100     0       65000 65203 i
 *  ec    1000:3000:2::203/128   2000::204             0       -          100     0       65000 65204 i
 * >      1000:3000:2:0:240:1ff:fe00:2/128 2000::40              0       -          100     0       65000 65040 i
 * >      1000:3000:3::/64       -                     -       -          -       0       i
 *  Ec    1000:3000:3::/64       2000::204             0       -          100     0       65000 65204 i
 *  ec    1000:3000:3::/64       2000::203             0       -          100     0       65000 65203 i
 *  ec    1000:3000:3::/64       2000::202             0       -          100     0       65000 65202 i
 *  ec    1000:3000:3::/64       2000::56              0       -          100     0       65000 65056 i
 * >      1000:3000:3::22/128    2000::22              0       -          100     0       65000 65022 i
 * >      1000:3000:3::56/128    2000::56              0       -          100     0       65000 65056 i
          1000:3000:3::201/128   2000::202             0       -          100     0       65000 65202 i
 * >Ec    1000:3000:3::203/128   2000::204             0       -          100     0       65000 65204 i
 *  ec    1000:3000:3::203/128   2000::203             0       -          100     0       65000 65203 i
 * >      1000:3000:4::/64       -                     -       -          -       0       i
 *  Ec    1000:3000:4::/64       2000::202             0       -          100     0       65000 65202 i
 *  ec    1000:3000:4::/64       2000::203             0       -          100     0       65000 65203 i
 *  ec    1000:3000:4::/64       2000::204             0       -          100     0       65000 65204 i
 *  ec    1000:3000:4::/64       2000::56              0       -          100     0       65000 65056 i
 * >      1000:3000:4::22/128    2000::22              0       -          100     0       65000 65022 i
 * >      1000:3000:4::56/128    2000::56              0       -          100     0       65000 65056 i
          1000:3000:4::201/128   2000::202             0       -          100     0       65000 65202 i
 * >Ec    1000:3000:4::203/128   2000::204             0       -          100     0       65000 65204 i
 *  ec    1000:3000:4::203/128   2000::203             0       -          100     0       65000 65203 i
```

## show ipv6 route vrf all

```text

VRF: default
Displaying 10 of 13 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 B E      2000::22/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::23/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::40/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::56/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::200/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 C        2000::201/128 [0/0]
           via Loopback0, directly connected
 B E      2000::202/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::203/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::204/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2001::56/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1


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

VRF: tenant-a
Displaying 30 of 38 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 B E      1000:1000:22::22/128 [20/0]
           via VTEP 2000::22 VNI 1000 router-mac c4:07:78:0a:9f:31
 B E      1000:1000:22::254/128 [20/0]
           via VTEP 2000::22 VNI 1000 router-mac c4:07:78:0a:9f:31
           via VTEP 2000::23 VNI 1000 router-mac c4:07:78:0a:77:7d
 B E      1000:1000:22::/64 [20/0]
           via VTEP 2000::22 VNI 1000 router-mac c4:07:78:0a:9f:31
           via VTEP 2000::23 VNI 1000 router-mac c4:07:78:0a:77:7d
 B E      1000:1000:40::40/128 [20/0]
           via VTEP 2000::40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      1000:1000:40:0:240:1ff:fe00:3/128 [20/0]
           via VTEP 2000::40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      1000:1000:40::/64 [20/0]
           via VTEP 2000::40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      1000:1000:56::56/128 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      1000:1000:56::/64 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 C        1000:1000:201::/64 [0/0]
           via Vlan1201, directly connected
 B E      1000:1000:203::203/128 [20/0]
           via VTEP 2000::204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 2000::203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 B E      1000:1000:203::/64 [20/0]
           via VTEP 2000::204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 2000::203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 B E      1000:3000:1::22/128 [20/0]
           via VTEP 2000::22 VNI 1000 router-mac c4:07:78:0a:9f:31
 B E      1000:3000:1::40/128 [20/0]
           via VTEP 2000::40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      1000:3000:1::56/128 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      1000:3000:1::203/128 [20/0]
           via VTEP 2000::204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 2000::203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 B E      1000:3000:1:0:240:1ff:fe00:1/128 [20/0]
           via VTEP 2000::40 VNI 1000 router-mac 24:6c:84:74:8d:db
 C        1000:3000:1::/64 [0/0]
           via Vlan1301, directly connected
 B E      1000:3000:2::40/128 [20/0]
           via VTEP 2000::40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      1000:3000:2::56/128 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      1000:3000:2::203/128 [20/0]
           via VTEP 2000::204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 2000::203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 B E      1000:3000:2:0:240:1ff:fe00:2/128 [20/0]
           via VTEP 2000::40 VNI 1000 router-mac 24:6c:84:74:8d:db
 C        1000:3000:2::/64 [0/0]
           via Vlan1302, directly connected
 B E      1000:3000:3::22/128 [20/0]
           via VTEP 2000::22 VNI 1000 router-mac c4:07:78:0a:9f:31
 B E      1000:3000:3::56/128 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      1000:3000:3::203/128 [20/0]
           via VTEP 2000::204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 2000::203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 C        1000:3000:3::/64 [0/0]
           via Vlan1303, directly connected
 B E      1000:3000:4::22/128 [20/0]
           via VTEP 2000::22 VNI 1000 router-mac c4:07:78:0a:9f:31
 B E      1000:3000:4::56/128 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      1000:3000:4::203/128 [20/0]
           via VTEP 2000::204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 2000::203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 C        1000:3000:4::/64 [0/0]
           via Vlan1304, directly connected

```

## show bgp ipv6 unicast summary lldp

```text
BGP summary information for VRF default
Router identifier 100.0.0.201, local AS number 65201
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor                      LLDP Neighbor                  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
                           fe80::464c:a8ff:fe73:5c75%Et1 SPINE1-J-200.ns.eantc.de       4 65000           2046      1948    0    0    1d00h Estab   9      9
```

## show ipv6 neighbors vrf all

```text

VRF: default
IPv6 Address                                  Age Hardware Addr   Interface
fe80::464c:a8ff:fe73:5c75                 0:00:33 444c.a873.5c75  Et1

VRF: mgmt
IPv6 Address                                  Age Hardware Addr   Interface

VRF: tenant-a
IPv6 Address                                  Age Hardware Addr   Interface
1000:1000:201::201                        0:34:02 0020.1000.0005  Vl1201, Port-Channel100
fe80::220:10ff:fe00:5                     1:42:17 0020.1000.0005  Vl1201, Port-Channel100
fe80::2aa:aaff:feaa:aaaa                  0:01:37 00aa.aaaa.aaaa  Vl1201, Router
1000:3000:1::40                                 - 0040.0100.0001  Vl1301, Vxlan1
1000:3000:1::56                                 - 0056.0000.0001  Vl1301, Vxlan1
1000:3000:1::201                          0:34:02 0020.1000.0001  Vl1301, Port-Channel100
1000:3000:1::203                                - 0020.3000.0001  Vl1301, Vxlan1
1000:3000:1:0:240:1ff:fe00:1                    - 0040.0100.0001  Vl1301, Vxlan1
fe80::2aa:aaff:feaa:aaaa                  0:02:43 00aa.aaaa.aaaa  Vl1301, Router
1000:3000:2::22                           2:01:58 0022.0000.0002  Vl1302, Vxlan1
1000:3000:2::40                                 - 0040.0100.0002  Vl1302, Vxlan1
1000:3000:2::56                                 - 0056.0000.0002  Vl1302, Vxlan1
1000:3000:2::201                                - 0020.1000.0002  Vl1302, Port-Channel100
1000:3000:2::203                                - 0020.3000.0002  Vl1302, Vxlan1
1000:3000:2:0:240:1ff:fe00:2                    - 0040.0100.0002  Vl1302, Vxlan1
fe80::2aa:aaff:feaa:aaaa                  0:03:17 00aa.aaaa.aaaa  Vl1302, Router
1000:3000:3::22                           2:01:58 0022.0000.0003  Vl1303, Vxlan1
1000:3000:3::56                                 - 0056.0000.0003  Vl1303, Vxlan1
1000:3000:3::201                          0:34:02 0020.1000.0003  Vl1303, Port-Channel100
1000:3000:3::203                                - 0020.3000.0003  Vl1303, Vxlan1
fe80::2aa:aaff:feaa:aaaa                  0:16:52 00aa.aaaa.aaaa  Vl1303, Router
1000:3000:4::22                           2:01:58 0022.0000.0004  Vl1304, Vxlan1
1000:3000:4::56                                 - 0056.0000.0004  Vl1304, Vxlan1
1000:3000:4::201                          0:34:02 0020.1000.0004  Vl1304, Port-Channel100
1000:3000:4::203                                - 0020.3000.0004  Vl1304, Vxlan1
fe80::2aa:aaff:feaa:aaaa                  4:01:06 00aa.aaaa.aaaa  Vl1304, Router
```

## show ipv6 neighbors remote

```text
ARP remote bindings
VLAN IP Address                   MAC Address    Source         
---- ---------------------------- -------------- ---------------
1301 1000:3000:1::40              0040.0100.0001 EVPN remote    
1301 1000:3000:1::56              0056.0000.0001 EVPN remote    
1301 1000:3000:1::203             0020.3000.0001 EVPN remote    
1301 1000:3000:1::254             00aa.aaaa.aaaa EVPN remote    
1301 1000:3000:1:0:240:1ff:fe00:1 0040.0100.0001 EVPN remote    
1301 fe80::256:ff:fe00:1          0056.0000.0001 EVPN remote    
1301 fe80::2aa:aaff:feaa:aaaa     00aa.aaaa.aaaa EVPN remote    
1302 1000:3000:2::40              0040.0100.0002 EVPN remote    
1302 1000:3000:2::56              0056.0000.0002 EVPN remote    
1302 1000:3000:2::201             0020.1000.0002 EVPN multihomed
1302 1000:3000:2::203             0020.3000.0002 EVPN remote    
1302 1000:3000:2::254             00aa.aaaa.aaaa EVPN remote    
1302 1000:3000:2:0:240:1ff:fe00:2 0040.0100.0002 EVPN remote    
1302 fe80::256:ff:fe00:2          0056.0000.0002 EVPN remote    
1302 fe80::2aa:aaff:feaa:aaaa     00aa.aaaa.aaaa EVPN remote    
1303 1000:3000:3::56              0056.0000.0003 EVPN remote    
1303 1000:3000:3::203             0020.3000.0003 EVPN remote    
1303 1000:3000:3::254             00aa.aaaa.aaaa EVPN remote    
1303 fe80::222:ff:fe00:3          0022.0000.0003 EVPN remote    
1303 fe80::256:ff:fe00:3          0056.0000.0003 EVPN remote    
1303 fe80::2aa:aaff:feaa:aaaa     00aa.aaaa.aaaa EVPN remote    
1304 1000:3000:4::56              0056.0000.0004 EVPN remote    
1304 1000:3000:4::203             0020.3000.0004 EVPN remote    
1304 1000:3000:4::254             00aa.aaaa.aaaa EVPN remote    
1304 fe80::222:ff:fe00:4          0022.0000.0004 EVPN remote    
1304 fe80::256:ff:fe00:4          0056.0000.0004 EVPN remote    
1304 fe80::2aa:aaff:feaa:aaaa     00aa.aaaa.aaaa EVPN remote    
```

## show ipv6 nd ra neighbors

```text
VRF: default
   Interface             IPv6 Address           Last RA Received
--------------- ------------------------------- ----------------
   Ethernet1       fe80::464c:a8ff:fe73:5c75      0:02:19 ago   

```

## show ipv6 nd ra neighbors vrf tenant-a

```text
VRF: tenant-a
   Interface             IPv6 Address          Last RA Received
--------------- ------------------------------ ----------------
   Vlan1201        fe80::2aa:aaff:feaa:aaaa      0:01:37 ago   
   Vlan1301        fe80::2aa:aaff:feaa:aaaa      0:01:09 ago   
   Vlan1302        fe80::2aa:aaff:feaa:aaaa      0:00:13 ago   
   Vlan1303        fe80::2aa:aaff:feaa:aaaa      0:00:18 ago   
   Vlan1304        fe80::2aa:aaff:feaa:aaaa      0:00:46 ago   

```

## show interfaces counters rates | nz

```text
Port      Name       Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Et1       ANET 201    0:01      0.0   0.0%        0      0.2   0.0%        0
Et5       A-Harn-205  0:01      0.1   0.0%        0      0.0   0.0%        0
Ma1                   0:05      0.1   0.0%        0      0.3   0.0%        0
Po100                 0:01      0.1   0.0%        0      0.0   0.0%        0
```

