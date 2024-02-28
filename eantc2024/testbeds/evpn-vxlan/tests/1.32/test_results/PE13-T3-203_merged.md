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
  Description              Neighbor V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.203, local AS number 65203
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  NODE200.EVPN             2000::200 4 65000            907       162    0    0 01:39:02 Estab   238    238
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
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
BGP routing table entry for auto-discovery 1022 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
BGP routing table entry for auto-discovery 1301 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 1302 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan
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
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan
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
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1203:1203 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
BGP routing table entry for auto-discovery 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
BGP routing table entry for mac-ip 0020.1000.0001, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0001 1000:3000:1::201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83 EvpnNdFlags:pflag
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0002 1000:3000:2::201, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0005, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0005, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0005 1000:1000:201::201, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1201:1201 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1201 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0005 1000:1000:201::201, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7 EvpnNdFlags:pflag
      VNI: 1201 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.3000.0001, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0001 1000:3000:1::203, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0001 1000:3000:1::203, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0002, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0002 1000:3000:2::203, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0002 1000:3000:2::203, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0005, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0005 1000:1000:203::203, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1203 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0005 1000:1000:203::203, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1203 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0022.0000.0001, Route Distinguisher: 100.0.0.23:1301
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:11
      VNI: 1301 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 0022.0000.0001 fe80::222:ff:fe00:1, Route Distinguisher: 100.0.0.23:1301
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:7 EvpnRouterMac:c4:07:78:0a:77:7d
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 0022.0000.0002 1000:3000:2::22, Route Distinguisher: 100.0.0.23:1302
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:9 EvpnRouterMac:c4:07:78:0a:77:7d
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 0022.0000.0002 fe80::222:ff:fe00:2, Route Distinguisher: 100.0.0.23:1302
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:2 EvpnRouterMac:c4:07:78:0a:77:7d
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
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
BGP routing table entry for mac-ip 0042.0100.0001, Route Distinguisher: 100.0.0.42:34068
 Paths: 1 available
  65000 65042
    2000::42 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0042.0100.0001 1000:3000:1::42, Route Distinguisher: 100.0.0.42:34068
 Paths: 1 available
  65000 65042
    2000::42 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0042.0100.0001 1000:3000:1:0:242:1ff:fe00:1, Route Distinguisher: 100.0.0.42:34068
 Paths: 1 available
  65000 65042
    2000::42 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0042.0100.0002, Route Distinguisher: 100.0.0.42:34069
 Paths: 1 available
  65000 65042
    2000::42 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0042.0100.0002 1000:3000:2::42, Route Distinguisher: 100.0.0.42:34069
 Paths: 1 available
  65000 65042
    2000::42 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0042.0100.0002 1000:3000:2:0:242:1ff:fe00:2, Route Distinguisher: 100.0.0.42:34069
 Paths: 1 available
  65000 65042
    2000::42 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0042.0100.0003, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65000 65042
    2000::42 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan
      VNI: 1042 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0042.0100.0003 1000:1000:42::42, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65000 65042
    2000::42 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1042 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0042.0100.0003 1000:1000:42:0:242:1ff:fe00:3, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65000 65042
    2000::42 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1042 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0001, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0001, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0001 1000:3000:1::45, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0001 1000:3000:1::45, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0001 1000:3000:1:0:245:1ff:fe00:1, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0001 1000:3000:1:0:245:1ff:fe00:1, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0002, Route Distinguisher: 100.0.0.45:34069
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0002, Route Distinguisher: 100.0.0.46:34069
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0002 1000:3000:2::45, Route Distinguisher: 100.0.0.45:34069
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0002 1000:3000:2::45, Route Distinguisher: 100.0.0.46:34069
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0002 1000:3000:2:0:245:1ff:fe00:2, Route Distinguisher: 100.0.0.45:34069
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0002 1000:3000:2:0:245:1ff:fe00:2, Route Distinguisher: 100.0.0.46:34069
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0003, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0003, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0003 1000:1000:45::45, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0003 1000:1000:45::45, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0003 1000:1000:45:0:245:1ff:fe00:3, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0003 1000:1000:45:0:245:1ff:fe00:3, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
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
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.2.254, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 1000:1000:22::254, Route Distinguisher: 100.0.0.23:1022
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:77:7d
      VNI: 1022 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 1000:1000:56::254, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
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
BGP routing table entry for mac-ip 00aa.aaaa.aaaa fe80::2aa:aaff:feaa:aaaa, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    2000::56 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1022 0022.0000.0005, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:35
      VNI: 1022 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 1022 0022.0000.0005 1000:1000:22::22, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:35 EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1022 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 1022 0022.0000.0005 fe80::222:ff:fe00:5, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:34 EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1022 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 1301 0022.0000.0001 1000:3000:1::22, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:3 EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 1302 0022.0000.0002, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:44
      VNI: 1302 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 1303 0020.1000.0003, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0020.1000.0003 1000:3000:3::201, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0020.3000.0003, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0020.3000.0003 1000:3000:3::203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0020.3000.0003 1000:3000:3::203, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0022.0000.0003, Route Distinguisher: 100.0.0.23:1303
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 1303 0022.0000.0003 fe80::222:ff:fe00:3, Route Distinguisher: 100.0.0.23:1303
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:77:7d
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 1304 0020.1000.0004, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 0020.3000.0004 1000:3000:4::203, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 0022.0000.0004, Route Distinguisher: 100.0.0.23:1304
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 1304 0022.0000.0004 1000:3000:4::22, Route Distinguisher: 100.0.0.23:1304
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:77:7d EvpnNdFlags:oflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 1304 0022.0000.0004 fe80::222:ff:fe00:4, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
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
Router identifier 100.0.0.203, local AS number 65203
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
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
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
BGP routing table entry for imet 2000::42, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65000 65042
    2000::42 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan
      VNI: 1042
      PMSI Tunnel: Ingress Replication, MPLS Label: 1042, Leaf Information Required: false, Tunnel ID: 2000::42
BGP routing table entry for imet 2000::42, Route Distinguisher: 100.0.0.42:34068
 Paths: 1 available
  65000 65042
    2000::42 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::42
BGP routing table entry for imet 2000::42, Route Distinguisher: 100.0.0.42:34069
 Paths: 1 available
  65000 65042
    2000::42 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::42
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
BGP routing table entry for imet 2000::100, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan
      VNI: 1045
      PMSI Tunnel: Ingress Replication, MPLS Label: 1045, Leaf Information Required: false, Tunnel ID: 2000::100
BGP routing table entry for imet 2000::100, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::100
BGP routing table entry for imet 2000::100, Route Distinguisher: 100.0.0.45:34069
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::100
BGP routing table entry for imet 2000::100, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan
      VNI: 1045
      PMSI Tunnel: Ingress Replication, MPLS Label: 1045, Leaf Information Required: false, Tunnel ID: 2000::100
BGP routing table entry for imet 2000::100, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::100
BGP routing table entry for imet 2000::100, Route Distinguisher: 100.0.0.46:34069
 Paths: 1 available
  65000 65045
    2000::100 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::100
BGP routing table entry for imet 2000::201, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
      PMSI Tunnel: Ingress Replication, MPLS Label: 1201, Leaf Information Required: false, Tunnel ID: 2000::201
BGP routing table entry for imet 2000::201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::201
BGP routing table entry for imet 2000::201, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
      PMSI Tunnel: Ingress Replication, MPLS Label: 1203, Leaf Information Required: false, Tunnel ID: 2000::203
BGP routing table entry for imet 2000::203, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::203
BGP routing table entry for imet 2000::203, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
Router identifier 100.0.0.203, local AS number 65203
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:10:02:02 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0201:0202 2000::202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  65000 65202
    2000::202 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:10:02:02 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0203:0204 2000::203, Route Distinguisher: 100.0.0.203:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:30:02:04 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0203:0204 2000::204, Route Distinguisher: 100.0.0.204:1
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:30:02:04 DF Election: Preference 100
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    2000::204 from 2000::200 (100.0.0.200)
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
0     1103   VXLAN 10.10.103.103      a222.0100.0001  100.0.30.14        -   
1203  1203   VXLAN 1000:1000:203::203 0020.3000.0005  2000::204          -   
1203  1203   VXLAN 1000:1000:203::203 0020.3000.0005  Local              -   
1203  1203   VXLAN 10.10.203.203      001b.0100.0001  100.0.0.204        -   
1203  1203   VXLAN 10.10.203.203      6666.6666.0001  100.0.0.103        -   
1301  1301   VXLAN 10.30.1.123        a244.0100.0019  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.178        a244.0100.0050  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.152      a222.0100.0032  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.121      a222.0100.0013  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.106      a222.0100.0004  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.143      a222.0100.0029  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.118        a244.0100.0014  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.201        001b.0100.0002  100.0.0.204        2   
1301  1301   VXLAN 10.10.103.167      a222.0100.0041  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.202      a222.0100.0064  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.193      a222.0100.005b  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.145      a222.0100.002b  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.209        001b.0100.003b  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.205        001b.0100.0037  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.197      a222.0100.005f  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.173      a222.0100.0047  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.226        001b.0100.004c  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.129        a244.0100.001f  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.117      a222.0100.000f  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.185      a222.0100.0053  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.249        001b.0100.0063  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.246        001b.0100.0060  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.110        a244.0100.000c  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.161        a244.0100.003f  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.176        a244.0100.004e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.183        a244.0100.0055  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.135      a222.0100.0021  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.179      a222.0100.004d  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.203        001b.0100.0002  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.123      a222.0100.0015  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.221        001b.0100.0047  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.169      a222.0100.0043  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.148        a244.0100.0032  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.103        a244.0101.0001  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.159        a244.0100.003d  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.107      a222.0100.0005  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.112        a244.0100.000e  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.195      a222.0100.005d  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.146        a244.0100.0030  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.179        a244.0100.0051  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.160      a222.0100.003a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.240        001b.0100.005a  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.181        a244.0100.0053  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.127      a222.0100.0019  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.201      a222.0100.0063  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.174        a244.0100.004c  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.171        a244.0100.0049  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.203        001b.0100.0035  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.157      a222.0100.0037  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.196      a222.0100.005e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.245        001b.0100.005f  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.235        001b.0100.0055  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.146      a222.0100.002c  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.118      a222.0100.0010  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.239        001b.0100.0059  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.159      a222.0100.0039  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.191      a222.0100.0059  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.228        001b.0100.004e  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.156        a244.0100.003a  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.111      a222.0100.0009  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.211        001b.0100.003d  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.107        a244.0100.0009  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.187        a244.0100.0059  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.155      a222.0100.0035  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.187      a222.0100.0055  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.131      a222.0100.001d  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.128        a244.0100.001e  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.115      a222.0100.000d  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.140        a244.0100.002a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.111        a244.0100.000d  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.165      a222.0100.003f  100.0.0.201        -   
1301  1301   VXLAN fe80::222:ff:fe00: 0022.0000.0001  2000::23           7   
                   1                                                         
1301  1301   VXLAN 10.30.1.164        a244.0100.0042  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.207        001b.0100.0039  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.197        a244.0100.0063  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.177        a244.0100.004f  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.195        a244.0100.0061  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.178      a222.0100.004c  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.192        a244.0100.005e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.241        001b.0100.005b  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.149        a244.0100.0033  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.224        001b.0100.004a  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.99         a244.0100.0001  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.174      a222.0100.0048  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.160        a244.0100.003e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.225        001b.0100.004b  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.140      a222.0100.0026  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.112      a222.0100.000a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.122        a244.0100.0018  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.244        001b.0100.005e  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.124        a244.0100.001a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.196        a244.0100.0062  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.105      a222.0100.0003  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.186        a244.0100.0058  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.157        a244.0100.003b  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.162      a222.0100.003c  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.113      a222.0100.000b  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.114      a222.0100.000c  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.217        001b.0100.0043  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.102        a244.0100.0004  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.149      a222.0100.002f  100.0.0.201        -   
1301  1301   VXLAN 1000:3000:1::201   0020.1000.0001  2000::201          -   
1301  1301   VXLAN 1000:3000:1::201   0020.1000.0001  2000::202          -   
1301  1301   VXLAN 10.30.1.134        a244.0100.0024  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.199      a222.0100.0061  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.231        001b.0100.0051  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.151      a222.0100.0031  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.168        a244.0100.0046  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.170      a222.0100.0044  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.152        a244.0100.0036  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.232        001b.0100.0052  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.50         3333.3333.3333  100.0.0.201        Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.175        a244.0100.004d  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.213        001b.0100.003f  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.198        a244.0100.0064  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.176      a222.0100.004a  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.122      a222.0100.0014  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.185        a244.0100.0057  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.219        001b.0100.0045  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.164      a222.0100.003e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.104        a244.0100.0006  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.177      a222.0100.004b  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.154        a244.0100.0038  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.109      a222.0100.0007  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.158        a244.0100.003c  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.229        001b.0100.004f  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.158      a222.0100.0038  100.0.0.201        -   
1301  1301   VXLAN 1000:3000:1::40    0040.0100.0001  2000::40           -   
1301  1301   VXLAN 10.10.103.203      a222.0100.0065  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.155        a244.0100.0039  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.199        a244.0100.0065  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.139        a244.0100.0029  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.131        a244.0100.0021  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.150        a244.0100.0034  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.200        a244.0100.0066  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.208        001b.0100.003a  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.222        001b.0100.0048  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.248        001b.0100.0062  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.184      a222.0100.0052  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.100        a244.0100.0002  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.153        a244.0100.0037  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.173        a244.0100.004b  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.154      a222.0100.0034  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.172        a244.0100.004a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.147        a244.0100.0031  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.194      a222.0100.005c  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.130        a244.0100.0020  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.188      a222.0100.0056  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.44         001c.0100.0002  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.243        001b.0100.005d  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.130      a222.0100.001c  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.125        a244.0100.001b  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.143        a244.0100.002d  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.121        a244.0100.0017  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.156      a222.0100.0036  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.238        001b.0100.0058  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.190      a222.0100.0058  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.151        a244.0100.0035  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.186      a222.0100.0054  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.200      a222.0100.0062  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.132      a222.0100.001e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.137        a244.0100.0027  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.166      a222.0100.0040  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.190        a244.0100.005c  100.0.0.201        -   
1301  1301   VXLAN 1000:3000:1::203   0020.3000.0001  2000::204          -   
1301  1301   VXLAN 1000:3000:1::203   0020.3000.0001  Local              -   
1301  1301   VXLAN 10.30.1.180        a244.0100.0052  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.144      a222.0100.002a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.218        001b.0100.0044  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.206        001b.0100.0038  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.136      a222.0100.0022  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.117        a244.0100.0013  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.119      a222.0100.0011  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.188        a244.0100.005a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.236        001b.0100.0056  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.172      a222.0100.0046  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.114        a244.0100.0010  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.127        a244.0100.001d  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.110      a222.0100.0008  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.234        001b.0100.0054  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.170        a244.0100.0048  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.105        a244.0100.0007  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.212        001b.0100.003e  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.134      a222.0100.0020  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.250        001b.0100.0064  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.175      a222.0100.0049  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.126      a222.0100.0018  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.215        001b.0100.0041  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.166        a244.0100.0044  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.139      a222.0100.0025  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.109        a244.0100.000b  100.0.0.201        -   
1301  1301   VXLAN 1000:3000:1:0:240: 0040.0100.0001  2000::40           -   
                   1ff:fe00:1                                                
1301  1301   VXLAN 10.10.103.142      a222.0100.0028  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.150      a222.0100.0030  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.101        a244.0100.0003  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.237        001b.0100.0057  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.126        a244.0100.001c  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.138      a222.0100.0024  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.182        a244.0100.0054  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.233        001b.0100.0053  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.144        a244.0100.002e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.191        a244.0100.005d  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.194        a244.0100.0060  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.201        001b.0100.0033  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.104      a222.0100.0002  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.189      a222.0100.0057  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.168      a222.0100.0042  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.184        a244.0100.0056  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.204        001b.0100.0036  100.0.0.204        -   
1301  1301   VXLAN 1000:3000:1::22    0022.0000.0001  2000::22           3   
1301  1301   VXLAN 10.10.103.103      a222.0100.0001  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.129      a222.0100.001b  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.133        a244.0100.0023  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.165        a244.0100.0043  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.108      a222.0100.0006  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.180      a222.0100.004e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.167        a244.0100.0045  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.128      a222.0100.001a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.120        a244.0100.0016  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.203        6666.6668.0001  100.0.0.103        -   
1301  1301   VXLAN 10.30.1.142        a244.0100.002c  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.138        a244.0100.0028  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.163        a244.0100.0041  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.189        a244.0100.005b  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.115        a244.0100.0011  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.216        001b.0100.0042  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.141      a222.0100.0027  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.116      a222.0100.000e  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.192      a222.0100.005a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.103        a244.0100.0005  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.120      a222.0100.0012  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.214        001b.0100.0040  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.116        a244.0100.0012  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.230        001b.0100.0050  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.108        a244.0100.000a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.145        a244.0100.002f  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.124      a222.0100.0016  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.227        001b.0100.004d  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.193        a244.0100.005f  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.147      a222.0100.002d  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.137      a222.0100.0023  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.242        001b.0100.005c  100.0.0.204        -   
1301  1301   VXLAN 1000:3000:1:0:245: 0045.0100.0001  2000::100          -   
                   1ff:fe00:1                                                
1301  1301   VXLAN 1000:3000:1:0:245: 0045.0100.0001  2000::100          -   
                   1ff:fe00:1                                                
1301  1301   VXLAN 10.30.1.141        a244.0100.002b  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.182      a222.0100.0050  100.0.0.201        -   
1301  1301   VXLAN 1000:3000:1::42    0042.0100.0001  2000::42           -   
1301  1301   VXLAN 1000:3000:1::45    0045.0100.0001  2000::100          -   
1301  1301   VXLAN 1000:3000:1::45    0045.0100.0001  2000::100          -   
1301  1301   VXLAN 10.30.1.135        a244.0100.0025  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.106        a244.0100.0008  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.153      a222.0100.0033  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.133      a222.0100.001f  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.202        001b.0100.0034  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.223        001b.0100.0049  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.181      a222.0100.004f  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.183      a222.0100.0051  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.136        a244.0100.0026  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.113        a244.0100.000f  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.204      a222.0100.0066  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.161      a222.0100.003b  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.220        001b.0100.0046  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.169        a244.0100.0047  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.162        a244.0100.0040  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.125      a222.0100.0017  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.132        a244.0100.0022  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.163      a222.0100.003d  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.247        001b.0100.0061  100.0.0.204        -   
1301  1301   VXLAN 10.10.103.148      a222.0100.002e  100.0.0.201        -   
1301  1301   VXLAN 1000:3000:1:0:242: 0042.0100.0001  2000::42           -   
                   1ff:fe00:1                                                
1301  1301   VXLAN 10.30.1.119        a244.0100.0015  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.171      a222.0100.0045  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.198      a222.0100.0060  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.210        001b.0100.003c  100.0.0.204        -   
1302  1302   VXLAN fe80::222:ff:fe00: 0022.0000.0002  2000::23           2   
                   2                                                         
1302  1302   VXLAN 1000:3000:2::56    0056.0000.0002  2000::56           -   
1302  1302   VXLAN 1000:3000:2::254   00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1302  1302   VXLAN fe80::2aa:aaff:fea 00aa.aaaa.aaaa  2000::56           Stic
                   a:aaaa                                                ky  
1302  1302   VXLAN fe80::256:ff:fe00: 0056.0000.0002  2000::56           -   
                   2                                                         
1302  1302   VXLAN 1000:3000:2:0:242: 0042.0100.0002  2000::42           -   
                   1ff:fe00:2                                                
1302  1302   VXLAN 1000:3000:2::203   0020.3000.0002  2000::204          -   
1302  1302   VXLAN 1000:3000:2::203   0020.3000.0002  Local              -   
1302  1302   VXLAN 1000:3000:2::22    0022.0000.0002  2000::23           9   
1302  1302   VXLAN 1000:3000:2::201   0020.1000.0002  2000::202          -   
1302  1302   VXLAN 1000:3000:2::201   0020.1000.0002  2000::201          -   
1302  1302   VXLAN 10.30.2.254        00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1302  1302   VXLAN 1000:3000:2::42    0042.0100.0002  2000::42           -   
1302  1302   VXLAN 1000:3000:2::45    0045.0100.0002  2000::100          -   
1302  1302   VXLAN 1000:3000:2::45    0045.0100.0002  2000::100          -   
1302  1302   VXLAN 1000:3000:2:0:240: 0040.0100.0002  2000::40           -   
                   1ff:fe00:2                                                
1302  1302   VXLAN 1000:3000:2::40    0040.0100.0002  2000::40           -   
1302  1302   VXLAN 1000:3000:2:0:245: 0045.0100.0002  2000::100          -   
                   1ff:fe00:2                                                
1302  1302   VXLAN 1000:3000:2:0:245: 0045.0100.0002  2000::100          -   
                   1ff:fe00:2                                                
1303  1303   VXLAN 1000:3000:3::203   0020.3000.0003  2000::204          -   
1303  1303   VXLAN 1000:3000:3::203   0020.3000.0003  Local              -   
1303  1303   VXLAN fe80::222:ff:fe00: 0022.0000.0003  2000::23           -   
                   3                                                         
1303  1303   VXLAN 1000:3000:3::201   0020.1000.0003  2000::201          -   
1303  1303   VXLAN 1000:3000:3::201   0020.1000.0003  2000::202          -   
1304  1304   VXLAN 1000:3000:4::203   0020.3000.0004  2000::204          -   
1304  1304   VXLAN 1000:3000:4::203   0020.3000.0004  Local              -   
1304  1304   VXLAN fe80::222:ff:fe00: 0022.0000.0004  2000::22           -   
                   4                                                         
1304  1304   VXLAN fe80::2aa:aaff:fea 00aa.aaaa.aaaa  2000::56           Stic
                   a:aaaa                                                ky  
1304  1304   VXLAN 1000:3000:4::254   00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.254        00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1304  1304   VXLAN fe80::256:ff:fe00: 0056.0000.0004  2000::56           -   
                   4                                                         
1304  1304   VXLAN 1000:3000:4::56    0056.0000.0004  2000::56           -   
1304  1304   VXLAN 1000:3000:4::22    0022.0000.0004  2000::23           -   
1304  1304   VXLAN 1000:3000:4::201   0020.1000.0004  2000::201          -   
1304  1304   VXLAN 1000:3000:4::201   0020.1000.0004  2000::202          -   
0     2303   VXLAN 10.30.3.203        001b.0100.0003  100.0.30.14        6   
0     2303   VXLAN 10.30.3.254        0056.5656.5656  100.0.30.14        Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.14         f8c1.1604.3007  100.0.30.14        Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.14         f8c1.1604.3007  100.0.30.14        Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.103        a266.0102.0001  100.0.30.14        -   
0     2303   VXLAN 10.30.3.250        001b.0100.0096  100.0.30.14        2   
0     2303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.30.14        Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.30.14        -   
0     2304   VXLAN 10.30.4.250        001b.0100.00c8  100.0.30.14        1   
0     2304   VXLAN 10.30.4.103        a288.0103.0001  100.0.30.14        -   
0     2304   VXLAN 10.30.4.254        00aa.aaaa.aaaa  100.0.30.14        Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.254        00aa.aaaa.aaaa  100.0.30.14        -   
0     2304   VXLAN 10.30.4.14         f8c1.1604.3007  100.0.30.14        Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.14         f8c1.1604.3007  100.0.30.14        Stic
                                                                         ky  
0     2304   VXLAN 10.30.4.203        001b.0100.0004  100.0.30.14        22  
0     2304   VXLAN 10.30.4.254        0056.5656.5656  100.0.30.14        Stic
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
 B E      10.10.201.0/24 [20/0]
           via VTEP 2000::202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 2000::201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 C        10.10.203.0/24
           directly connected, Vlan1203
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
192.168.21.50     0:03:57  a84f.b1a5.5221  Management1
192.168.21.59     0:02:07  6607.f5d1.ae16  Management1

VRF: tenant-a
Address         Age (sec)  Hardware Addr   Interface
```

## show vxlan address-table

```text
          Vxlan Mac Address Table
----------------------------------------------------------------------

VLAN  Mac Address     Type      Prt  VTEP             Moves   Last Move
----  -----------     ----      ---  ----             -----   ---------
1301  0020.1000.0001  EVPN      Vx1  2000::201        1       0:16:00 ago
                                     2000::202      
1301  0022.0000.0001  EVPN      Vx1  2000::23         1       0:05:40 ago
1301  0040.0100.0001  EVPN      Vx1  2000::40         1       0:30:58 ago
1301  0042.0100.0001  EVPN      Vx1  2000::42         1       0:30:37 ago
1301  0045.0100.0001  EVPN      Vx1  2000::100        1       0:17:37 ago
1302  0020.1000.0002  EVPN      Vx1  2000::201        1       0:15:59 ago
                                     2000::202      
1302  0022.0000.0002  EVPN      Vx1  2000::23         3       0:28:51 ago
1302  0040.0100.0002  EVPN      Vx1  2000::40         1       0:30:58 ago
1302  0042.0100.0002  EVPN      Vx1  2000::42         1       0:30:37 ago
1302  0045.0100.0002  EVPN      Vx1  2000::100        1       0:17:19 ago
1302  0056.0000.0002  EVPN      Vx1  2000::56         1       0:16:01 ago
1303  0020.1000.0003  EVPN      Vx1  2000::201        1       0:15:59 ago
                                     2000::202      
1303  0022.0000.0003  EVPN      Vx1  2000::22         5       0:16:13 ago
                                     2000::23       
1304  0020.1000.0004  EVPN      Vx1  2000::201        1       0:15:59 ago
                                     2000::202      
1304  0022.0000.0004  EVPN      Vx1  2000::22         1       0:16:00 ago
                                     2000::23       
1304  0056.0000.0004  EVPN      Vx1  2000::56         1       0:16:01 ago
4094  0001.0000.0056  EVPN      Vx1  2000::56                 0:57:18 ago
4094  0600.0000.0100  EVPN      Vx1  2000::100                0:17:37 ago
4094  246c.8474.8ddb  EVPN      Vx1  2000::40                 0:31:44 ago
4094  2cdd.e90b.2283  EVPN      Vx1  2000::201                1:06:47 ago
4094  2cdd.e90b.25b7  EVPN      Vx1  2000::202                1:06:48 ago
4094  4014.827b.84ab  EVPN      Vx1  2000::42                 0:31:33 ago
4094  985d.82a2.04f9  EVPN      Vx1  2000::204                1:06:50 ago
4094  c407.780a.777d  EVPN      Vx1  2000::23                 1:21:57 ago
4094  c407.780a.9f31  EVPN      Vx1  2000::22                 0:16:13 ago
Total Remote Mac Addresses for this criterion: 25
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
1203    0020.3000.0005    DYNAMIC     Po200      1       0:09:35 ago
1203    00aa.aaaa.aaaa    STATIC      Router
1301    0020.1000.0001    DYNAMIC     Vx1        1       0:16:00 ago
1301    0020.3000.0001    DYNAMIC     Po200      1       0:15:56 ago
1301    0022.0000.0001    DYNAMIC     Vx1        1       0:05:40 ago
1301    0040.0100.0001    DYNAMIC     Vx1        1       0:30:58 ago
1301    0042.0100.0001    DYNAMIC     Vx1        1       0:30:37 ago
1301    0045.0100.0001    DYNAMIC     Vx1        1       0:17:37 ago
1301    00aa.aaaa.aaaa    STATIC      Router
1302    0020.1000.0002    DYNAMIC     Vx1        1       0:15:59 ago
1302    0020.3000.0002    DYNAMIC     Po200      1       0:15:57 ago
1302    0022.0000.0002    DYNAMIC     Vx1        3       0:28:51 ago
1302    0040.0100.0002    DYNAMIC     Vx1        1       0:30:58 ago
1302    0042.0100.0002    DYNAMIC     Vx1        1       0:30:37 ago
1302    0045.0100.0002    DYNAMIC     Vx1        1       0:17:19 ago
1302    0056.0000.0002    DYNAMIC     Vx1        1       0:16:01 ago
1302    00aa.aaaa.aaaa    STATIC      Router
1303    0020.1000.0003    DYNAMIC     Vx1        1       0:15:59 ago
1303    0020.3000.0003    DYNAMIC     Po200      1       0:15:57 ago
1303    0022.0000.0003    DYNAMIC     Vx1        5       0:16:13 ago
1303    00aa.aaaa.aaaa    STATIC      Router
1304    0020.1000.0004    DYNAMIC     Vx1        1       0:15:59 ago
1304    0020.3000.0004    DYNAMIC     Po200      1       0:09:35 ago
1304    0022.0000.0004    DYNAMIC     Vx1        1       0:16:00 ago
1304    0056.0000.0004    DYNAMIC     Vx1        1       0:16:01 ago
1304    00aa.aaaa.aaaa    STATIC      Router
4094    0001.0000.0056    DYNAMIC     Vx1        0       0:57:18 ago
4094    00aa.aaaa.aaaa    STATIC      Router
4094    0600.0000.0100    DYNAMIC     Vx1        0       0:17:37 ago
4094    246c.8474.8ddb    DYNAMIC     Vx1        0       0:31:44 ago
4094    2cdd.e90b.2283    DYNAMIC     Vx1        0       1:06:47 ago
4094    2cdd.e90b.25b7    DYNAMIC     Vx1        0       1:06:48 ago
4094    4014.827b.84ab    DYNAMIC     Vx1        0       0:31:33 ago
4094    985d.82a2.04f9    DYNAMIC     Vx1        0       1:06:50 ago
4094    c407.780a.777d    DYNAMIC     Vx1        0       1:21:57 ago
4094    c407.780a.9f31    DYNAMIC     Vx1        0       0:16:13 ago
Total Mac Addresses for this criterion: 36

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
0020.3000.0004, VLAN 1304, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
0056.0000.0004, VLAN 1304, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::56
0045.0100.0001, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::100
0042.0100.0001, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::42
0045.0100.0002, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::100
0020.3000.0002, VLAN 1302, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
0022.0000.0001, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::23
0022.0000.0004, VLAN 1304, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 42: 2-way
      VTEP 2000::22
      VTEP 2000::23
0020.3000.0003, VLAN 1303, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
0022.0000.0003, VLAN 1303, seq 5, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 42: 2-way
      VTEP 2000::22
      VTEP 2000::23
0022.0000.0002, VLAN 1302, seq 3, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::23
0040.0100.0002, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::40
0020.1000.0001, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 43: 2-way
      VTEP 2000::201
      VTEP 2000::202
0020.3000.0001, VLAN 1301, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
0042.0100.0002, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::42
0056.0000.0002, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::56
0020.1000.0004, VLAN 1304, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 43: 2-way
      VTEP 2000::201
      VTEP 2000::202
00aa.aaaa.aaaa, VLAN 1304, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 2000::56
00aa.aaaa.aaaa, VLAN 1302, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 2000::56
0040.0100.0001, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::40
0020.1000.0003, VLAN 1303, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 43: 2-way
      VTEP 2000::201
      VTEP 2000::202
0020.3000.0005, VLAN 1203, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
0020.1000.0002, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 43: 2-way
      VTEP 2000::201
      VTEP 2000::202
```

## show vxlan flood vtep domain local

```text
          VXLAN Flood VTEP Table
--------------------------------------------------------------------------------

VLANS                            Ip Address
-----------------------------   ------------------------------------------------
1203                            2000::204      
1301-1302                       2000::22        2000::23        2000::40       
                                2000::42        2000::56        2000::100      
                                2000::201       2000::202       2000::204      
1303-1304                       2000::22        2000::23        2000::56       
                                2000::201       2000::202       2000::204      
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
EVPN instance: VLAN 1203
  Route distinguisher: 100.0.0.203:1203
  Route target import: Route-Target-AS:1203:1203
  Route target export: Route-Target-AS:1203:1203
  Service interface: VLAN-based
  Local VXLAN IP address: 2000::203
  VXLAN: enabled
  MPLS: disabled
  Local ethernet segment:
    ESI: 0000:0000:0000:0203:0204
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:30:02:04
      DF election algorithm: preference
      Designated forwarder: 2000::203
      Non-Designated forwarder: 2000::204
EVPN instance: VLAN 1301
  Route distinguisher: 100.0.0.203:1301
  Route target import: Route-Target-AS:1301:1301
  Route target export: Route-Target-AS:1301:1301
  Service interface: VLAN-based
  Local VXLAN IP address: 2000::203
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:0000:0000:0022:0023
    Active TEPs: 2000::22, 2000::23
    ESI: 0000:0000:0000:0201:0202
    Active TEPs: 2000::201, 2000::202
  Local ethernet segment:
    ESI: 0000:0000:0000:0203:0204
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:30:02:04
      DF election algorithm: preference
      Designated forwarder: 2000::203
      Non-Designated forwarder: 2000::204
EVPN instance: VLAN 1302
  Route distinguisher: 100.0.0.203:1302
  Route target import: Route-Target-AS:1302:1302
  Route target export: Route-Target-AS:1302:1302
  Service interface: VLAN-based
  Local VXLAN IP address: 2000::203
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:0000:0000:0022:0023
    Active TEPs: 2000::22, 2000::23
    ESI: 0000:0000:0000:0201:0202
    Active TEPs: 2000::201, 2000::202
  Local ethernet segment:
    ESI: 0000:0000:0000:0203:0204
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:30:02:04
      DF election algorithm: preference
      Designated forwarder: 2000::203
      Non-Designated forwarder: 2000::204
EVPN instance: VLAN-aware bundle 1303-1304
  Route distinguisher: 100.0.0.203:1303
  Route target import: Route-Target-AS:1303:1303
  Route target export: Route-Target-AS:1303:1303
  Service interface: VLAN-aware bundle
  Local VXLAN IP address: 2000::203
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:0000:0000:0022:0023
    Active TEPs: 2000::22, 2000::23
    ESI: 0000:0000:0000:0201:0202
    Active TEPs: 2000::201, 2000::202
  Local ethernet segment:
    ESI: 0000:0000:0000:0203:0204
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:30:02:04
      DF election algorithm: preference
      Designated forwarder: 2000::203
      Non-Designated forwarder: 2000::204
```

## show ipv6 interface brief

```text
Interface  Status    MTU  IPv6 Address                  Addr State  Addr Source
---------- ------- ------ ----------------------------- ----------- -----------
Et1        up       1500  fe80::3a38:a6ff:fe21:e82f/64  up          link local 
Lo0        up      65535  fe80::ff:fe00:0/64            up          link local 
                          2000::203/128                 up          config     
Vl1203     up       1500  fe80::3a38:a6ff:fe21:e82f/64  up          link local 
                          1000:1000:203::254/64         up          config     
Vl1301     up       1500  fe80::3a38:a6ff:fe21:e82f/64  up          link local 
                          1000:3000:1::254/64           up          config     
Vl1302     up       1500  fe80::3a38:a6ff:fe21:e82f/64  up          link local 
                          1000:3000:2::254/64           up          config     
Vl1303     up       1500  fe80::3a38:a6ff:fe21:e82f/64  up          link local 
                          1000:3000:3::254/64           up          config     
Vl1304     up       1500  fe80::3a38:a6ff:fe21:e82f/64  up          link local 
                          1000:3000:4::254/64           up          config     
Vl4094     up       9164  fe80::3a38:a6ff:fe21:e82f/64  up          link local 

```

## show ipv6 bgp summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.203, local AS number 65203
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor                      V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
                           fe80::464c:a8ff:fe73:5c75%Et1 4 65000            132       120    0    0 01:39:06 Estab   13     13
```

## show ipv6 bgp

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
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
 * >      2000::42/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65042 ?
 * >      2000::45/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65045 ?
 * >      2000::46/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65045 ?
 * >      2000::56/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65056 ?
 * >      2000::100/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65045 ?
 * >      2000::200/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 i
 * >      2000::201/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65201 i
 * >      2000::202/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65202 i
 * >      2000::203/128          -                     -       -          -       0       i
 * >      2000::204/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65204 i
 * >      2001::56/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65056 i
```

## show ipv6 route

```text

VRF: default
Displaying 14 of 17 IPv6 routing table entries
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
 B E      2000::42/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::45/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::46/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::56/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::100/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::200/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::201/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::202/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 C        2000::203/128 [0/0]
           via Loopback0, directly connected
 B E      2000::204/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2001::56/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1

```

## show ipv6 bgp vrf all

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
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
 * >      2000::42/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65042 ?
 * >      2000::45/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65045 ?
 * >      2000::46/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65045 ?
 * >      2000::56/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65056 ?
 * >      2000::100/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65045 ?
 * >      2000::200/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 i
 * >      2000::201/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65201 i
 * >      2000::202/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65202 i
 * >      2000::203/128          -                     -       -          -       0       i
 * >      2000::204/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65204 i
 * >      2001::56/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65056 i
BGP routing table information for VRF tenant-a
Router identifier 100.0.1.203, local AS number 65203
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
RPKI Origin Validation codes: V - valid, I - invalid, U - unknown
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
 * >      1000:1000:22::/64      2000::22              0       -          100     0       65000 65022 i
 * >      1000:1000:22::22/128   2000::22              0       -          100     0       65000 65022 i
 * >Ec    1000:1000:22::254/128  2000::23              0       -          100     0       65000 65023 i
 *  ec    1000:1000:22::254/128  2000::22              0       -          100     0       65000 65022 i
 * >      1000:1000:40::40/128   2000::40              0       -          100     0       65000 65040 i
 * >      1000:1000:40:0:240:1ff:fe00:3/128 2000::40              0       -          100     0       65000 65040 i
 * >      1000:1000:42::42/128   2000::42              0       -          100     0       65000 65042 i
 * >      1000:1000:42:0:242:1ff:fe00:3/128 2000::42              0       -          100     0       65000 65042 i
 * >Ec    1000:1000:45::45/128   2000::100             0       -          100     0       65000 65045 i
 *  ec    1000:1000:45::45/128   2000::100             0       -          100     0       65000 65045 i
 * >Ec    1000:1000:45:0:245:1ff:fe00:3/128 2000::100             0       -          100     0       65000 65045 i
 *  ec    1000:1000:45:0:245:1ff:fe00:3/128 2000::100             0       -          100     0       65000 65045 i
 * >      1000:1000:56::/64      2000::56              0       -          100     0       65000 65056 i
 * >      1000:1000:56::56/128   2000::56              0       -          100     0       65000 65056 i
 * >Ec    1000:1000:201::/64     2000::202             0       -          100     0       65000 65202 i
 *  ec    1000:1000:201::/64     2000::201             0       -          100     0       65000 65201 i
 * >Ec    1000:1000:201::201/128 2000::201             0       -          100     0       65000 65201 i
 *  ec    1000:1000:201::201/128 2000::202             0       -          100     0       65000 65202 i
 * >      1000:1000:203::/64     -                     -       -          -       0       i
 *        1000:1000:203::/64     2000::204             0       -          100     0       65000 65204 i
          1000:1000:203::203/128 2000::204             0       -          100     0       65000 65204 i
 * >      1000:3000:1::/64       -                     -       -          -       0       i
 *  Ec    1000:3000:1::/64       2000::23              0       -          100     0       65000 65023 i
 *  ec    1000:3000:1::/64       2000::204             0       -          100     0       65000 65204 i
 *  ec    1000:3000:1::/64       2000::202             0       -          100     0       65000 65202 i
 *  ec    1000:3000:1::/64       2000::201             0       -          100     0       65000 65201 i
 *  ec    1000:3000:1::/64       2000::56              0       -          100     0       65000 65056 i
 *  ec    1000:3000:1::/64       2000::22              0       -          100     0       65000 65022 i
 * >      1000:3000:1::22/128    2000::22              0       -          100     0       65000 65022 i
 * >      1000:3000:1::40/128    2000::40              0       -          100     0       65000 65040 i
 * >      1000:3000:1::42/128    2000::42              0       -          100     0       65000 65042 i
 * >Ec    1000:3000:1::45/128    2000::100             0       -          100     0       65000 65045 i
 *  ec    1000:3000:1::45/128    2000::100             0       -          100     0       65000 65045 i
 * >      1000:3000:1::56/128    2000::56              0       -          100     0       65000 65056 i
 * >Ec    1000:3000:1::201/128   2000::201             0       -          100     0       65000 65201 i
 *  ec    1000:3000:1::201/128   2000::202             0       -          100     0       65000 65202 i
          1000:3000:1::203/128   2000::204             0       -          100     0       65000 65204 i
 * >Ec    1000:3000:1::254/128   2000::23              0       -          100     0       65000 65023 i
 *  ec    1000:3000:1::254/128   2000::22              0       -          100     0       65000 65022 i
 * >      1000:3000:1:0:240:1ff:fe00:1/128 2000::40              0       -          100     0       65000 65040 i
 * >      1000:3000:1:0:242:1ff:fe00:1/128 2000::42              0       -          100     0       65000 65042 i
 * >Ec    1000:3000:1:0:245:1ff:fe00:1/128 2000::100             0       -          100     0       65000 65045 i
 *  ec    1000:3000:1:0:245:1ff:fe00:1/128 2000::100             0       -          100     0       65000 65045 i
 * >      1000:3000:2::/64       -                     -       -          -       0       i
 *  Ec    1000:3000:2::/64       2000::204             0       -          100     0       65000 65204 i
 *  ec    1000:3000:2::/64       2000::202             0       -          100     0       65000 65202 i
 *  ec    1000:3000:2::/64       2000::201             0       -          100     0       65000 65201 i
 *  ec    1000:3000:2::/64       2000::56              0       -          100     0       65000 65056 i
 * >      1000:3000:2::22/128    2000::23              0       -          100     0       65000 65023 i
 * >      1000:3000:2::40/128    2000::40              0       -          100     0       65000 65040 i
 * >      1000:3000:2::42/128    2000::42              0       -          100     0       65000 65042 i
 * >Ec    1000:3000:2::45/128    2000::100             0       -          100     0       65000 65045 i
 *  ec    1000:3000:2::45/128    2000::100             0       -          100     0       65000 65045 i
 * >      1000:3000:2::56/128    2000::56              0       -          100     0       65000 65056 i
 * >Ec    1000:3000:2::201/128   2000::202             0       -          100     0       65000 65202 i
 *  ec    1000:3000:2::201/128   2000::201             0       -          100     0       65000 65201 i
          1000:3000:2::203/128   2000::204             0       -          100     0       65000 65204 i
 * >      1000:3000:2:0:240:1ff:fe00:2/128 2000::40              0       -          100     0       65000 65040 i
 * >      1000:3000:2:0:242:1ff:fe00:2/128 2000::42              0       -          100     0       65000 65042 i
 * >Ec    1000:3000:2:0:245:1ff:fe00:2/128 2000::100             0       -          100     0       65000 65045 i
 *  ec    1000:3000:2:0:245:1ff:fe00:2/128 2000::100             0       -          100     0       65000 65045 i
 * >      1000:3000:3::/64       -                     -       -          -       0       i
 *  Ec    1000:3000:3::/64       2000::23              0       -          100     0       65000 65023 i
 *  ec    1000:3000:3::/64       2000::204             0       -          100     0       65000 65204 i
 *  ec    1000:3000:3::/64       2000::202             0       -          100     0       65000 65202 i
 *  ec    1000:3000:3::/64       2000::201             0       -          100     0       65000 65201 i
 *  ec    1000:3000:3::/64       2000::56              0       -          100     0       65000 65056 i
 *  ec    1000:3000:3::/64       2000::22              0       -          100     0       65000 65022 i
 * >      1000:3000:3::56/128    2000::56              0       -          100     0       65000 65056 i
 * >Ec    1000:3000:3::201/128   2000::202             0       -          100     0       65000 65202 i
 *  ec    1000:3000:3::201/128   2000::201             0       -          100     0       65000 65201 i
          1000:3000:3::203/128   2000::204             0       -          100     0       65000 65204 i
 * >Ec    1000:3000:3::254/128   2000::23              0       -          100     0       65000 65023 i
 *  ec    1000:3000:3::254/128   2000::22              0       -          100     0       65000 65022 i
 * >      1000:3000:4::/64       -                     -       -          -       0       i
 *  Ec    1000:3000:4::/64       2000::204             0       -          100     0       65000 65204 i
 *  ec    1000:3000:4::/64       2000::202             0       -          100     0       65000 65202 i
 *  ec    1000:3000:4::/64       2000::201             0       -          100     0       65000 65201 i
 *  ec    1000:3000:4::/64       2000::56              0       -          100     0       65000 65056 i
 * >      1000:3000:4::22/128    2000::23              0       -          100     0       65000 65023 i
 * >      1000:3000:4::56/128    2000::56              0       -          100     0       65000 65056 i
 * >Ec    1000:3000:4::201/128   2000::201             0       -          100     0       65000 65201 i
 *  ec    1000:3000:4::201/128   2000::202             0       -          100     0       65000 65202 i
          1000:3000:4::203/128   2000::204             0       -          100     0       65000 65204 i
```

## show ipv6 route vrf all

```text

VRF: default
Displaying 14 of 17 IPv6 routing table entries
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
 B E      2000::42/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::45/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::46/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::56/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::100/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::200/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::201/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::202/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 C        2000::203/128 [0/0]
           via Loopback0, directly connected
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
Displaying 41 of 49 IPv6 routing table entries
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
           via VTEP 2000::23 VNI 1000 router-mac c4:07:78:0a:77:7d
           via VTEP 2000::22 VNI 1000 router-mac c4:07:78:0a:9f:31
 B E      1000:1000:22::/64 [20/0]
           via VTEP 2000::22 VNI 1000 router-mac c4:07:78:0a:9f:31
 B E      1000:1000:40::40/128 [20/0]
           via VTEP 2000::40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      1000:1000:40:0:240:1ff:fe00:3/128 [20/0]
           via VTEP 2000::40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      1000:1000:42::42/128 [20/0]
           via VTEP 2000::42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      1000:1000:42:0:242:1ff:fe00:3/128 [20/0]
           via VTEP 2000::42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      1000:1000:45::45/128 [20/0]
           via VTEP 2000::100 VNI 1000 router-mac 06:00:00:00:01:00
 B E      1000:1000:45:0:245:1ff:fe00:3/128 [20/0]
           via VTEP 2000::100 VNI 1000 router-mac 06:00:00:00:01:00
 B E      1000:1000:56::56/128 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      1000:1000:56::/64 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      1000:1000:201::201/128 [20/0]
           via VTEP 2000::202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 2000::201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      1000:1000:201::/64 [20/0]
           via VTEP 2000::202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 2000::201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 C        1000:1000:203::/64 [0/0]
           via Vlan1203, directly connected
 B E      1000:3000:1::22/128 [20/0]
           via VTEP 2000::22 VNI 1000 router-mac c4:07:78:0a:9f:31
 B E      1000:3000:1::40/128 [20/0]
           via VTEP 2000::40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      1000:3000:1::42/128 [20/0]
           via VTEP 2000::42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      1000:3000:1::45/128 [20/0]
           via VTEP 2000::100 VNI 1000 router-mac 06:00:00:00:01:00
 B E      1000:3000:1::56/128 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      1000:3000:1::201/128 [20/0]
           via VTEP 2000::202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 2000::201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      1000:3000:1:0:240:1ff:fe00:1/128 [20/0]
           via VTEP 2000::40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      1000:3000:1:0:242:1ff:fe00:1/128 [20/0]
           via VTEP 2000::42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      1000:3000:1:0:245:1ff:fe00:1/128 [20/0]
           via VTEP 2000::100 VNI 1000 router-mac 06:00:00:00:01:00
 C        1000:3000:1::/64 [0/0]
           via Vlan1301, directly connected
 B E      1000:3000:2::22/128 [20/0]
           via VTEP 2000::23 VNI 1000 router-mac c4:07:78:0a:77:7d
 B E      1000:3000:2::40/128 [20/0]
           via VTEP 2000::40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      1000:3000:2::42/128 [20/0]
           via VTEP 2000::42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      1000:3000:2::45/128 [20/0]
           via VTEP 2000::100 VNI 1000 router-mac 06:00:00:00:01:00
 B E      1000:3000:2::56/128 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      1000:3000:2::201/128 [20/0]
           via VTEP 2000::202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 2000::201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 B E      1000:3000:2:0:240:1ff:fe00:2/128 [20/0]
           via VTEP 2000::40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      1000:3000:2:0:242:1ff:fe00:2/128 [20/0]
           via VTEP 2000::42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      1000:3000:2:0:245:1ff:fe00:2/128 [20/0]
           via VTEP 2000::100 VNI 1000 router-mac 06:00:00:00:01:00
 C        1000:3000:2::/64 [0/0]
           via Vlan1302, directly connected
 B E      1000:3000:3::56/128 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      1000:3000:3::201/128 [20/0]
           via VTEP 2000::202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 2000::201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 C        1000:3000:3::/64 [0/0]
           via Vlan1303, directly connected
 B E      1000:3000:4::22/128 [20/0]
           via VTEP 2000::23 VNI 1000 router-mac c4:07:78:0a:77:7d
 B E      1000:3000:4::56/128 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      1000:3000:4::201/128 [20/0]
           via VTEP 2000::202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 2000::201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 C        1000:3000:4::/64 [0/0]
           via Vlan1304, directly connected

```

## show bgp ipv6 unicast summary lldp

```text
BGP summary information for VRF default
Router identifier 100.0.0.203, local AS number 65203
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor                      LLDP Neighbor                  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
                           fe80::464c:a8ff:fe73:5c75%Et1 SPINE1-J-200.ns.eantc.de       4 65000            132       120    0    0 01:39:06 Estab   13     13
```

## show ipv6 neighbors

```text
IPv6 Address                                  Age Hardware Addr   Interface
fe80::464c:a8ff:fe73:5c75                 0:00:01 444c.a873.5c75  Et1
```

## show ipv6 nd ra neighbors

```text
VRF: default
   Interface             IPv6 Address           Last RA Received
--------------- ------------------------------- ----------------
   Ethernet1       fe80::464c:a8ff:fe73:5c75      0:01:27 ago   

```

## show ipv6 nd ra neighbors vrf tenant-a

```text
VRF: tenant-a
   Interface             IPv6 Address          Last RA Received
--------------- ------------------------------ ----------------
   Vlan1203        fe80::2aa:aaff:feaa:aaaa      0:02:37 ago   
   Vlan1301        fe80::2aa:aaff:feaa:aaaa      0:00:03 ago   
   Vlan1302        fe80::2aa:aaff:feaa:aaaa      0:00:06 ago   
   Vlan1303        fe80::2aa:aaff:feaa:aaaa      0:00:50 ago   
   Vlan1304        fe80::2aa:aaff:feaa:aaaa      0:01:09 ago   

```

## show interfaces counters rates | nz

```text
Port      Name       Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Et1       ANET 200    0:01      0.1   0.0%        0      0.1   0.0%        0
Et5       A-Harn-205  0:01      0.1   0.0%        0      0.1   0.0%        0
Ma1                   0:05      0.1   0.0%        0      0.3   0.0%        0
Po200                 0:01      0.1   0.0%        0      0.1   0.0%        0
```

