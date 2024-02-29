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
  Description              Neighbor V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.202, local AS number 65202
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  NODE200.EVPN             2000::200 4 65000           2026       565    0    0 00:09:25 Estab   202    202
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
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
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan
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
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
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
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
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
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
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
BGP routing table entry for mac-ip 1301 0022.0000.0001 1000:3000:1::22, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65022
    2000::22 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:3 EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 1303 0022.0000.0003 fe80::222:ff:fe00:3, Route Distinguisher: 100.0.0.23:1303
 Paths: 1 available
  65000 65023
    2000::23 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:77:7d
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
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
Router identifier 100.0.0.202, local AS number 65202
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
      Extended Community: Route-Target-AS:3301:64514 TunnelEncap:tunnelTypeVxlan
      VNI: 3301
      PMSI Tunnel: Ingress Replication, MPLS Label: 3301, Leaf Information Required: false, Tunnel ID: 100.0.0.206
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
      PMSI Tunnel: Ingress Replication, MPLS Label: 1201, Leaf Information Required: false, Tunnel ID: 2000::202
BGP routing table entry for imet 2000::202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::202
BGP routing table entry for imet 2000::202, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 2000::201
BGP routing table entry for imet 1303 2000::202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 2000::201
BGP routing table entry for imet 1304 2000::202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
Router identifier 100.0.0.202, local AS number 65202
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
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
  65000 65201
    2000::201 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
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
BGP routing table entry for ip-prefix 30.30.1.0/24, Route Distinguisher: 100.0.0.26:1000
 Paths: 1 available
  65000 65206
    100.0.0.206 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1023:1023 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:c4:02:71
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
1301  1301   VXLAN 1000:3000:1:0:245: 0045.0100.0001  2000::100          -   
                   1ff:fe00:1                                                
1301  1301   VXLAN 1000:3000:1:0:245: 0045.0100.0001  2000::100          -   
                   1ff:fe00:1                                                
1301  1301   VXLAN 1000:3000:1::42    0042.0100.0001  2000::42           -   
1301  1301   VXLAN 1000:3000:1::45    0045.0100.0001  2000::100          -   
1301  1301   VXLAN 1000:3000:1::45    0045.0100.0001  2000::100          -   
1301  1301   VXLAN 1000:3000:1::22    0022.0000.0001  2000::22           3   
1301  1301   VXLAN fe80::222:ff:fe00: 0022.0000.0001  2000::23           7   
                   1                                                         
1301  1301   VXLAN 1000:3000:1::40    0040.0100.0001  2000::40           -   
1301  1301   VXLAN 1000:3000:1:0:242: 0042.0100.0001  2000::42           -   
                   1ff:fe00:1                                                
1301  1301   VXLAN 1000:3000:1:0:240: 0040.0100.0001  2000::40           -   
                   1ff:fe00:1                                                
1302  1302   VXLAN 1000:3000:2::22    0022.0000.0002  2000::23           9   
1302  1302   VXLAN fe80::256:ff:fe00: 0056.0000.0002  2000::56           -   
                   2                                                         
1302  1302   VXLAN 1000:3000:2::56    0056.0000.0002  2000::56           -   
1302  1302   VXLAN 1000:3000:2:0:242: 0042.0100.0002  2000::42           -   
                   1ff:fe00:2                                                
1302  1302   VXLAN fe80::222:ff:fe00: 0022.0000.0002  2000::23           2   
                   2                                                         
1302  1302   VXLAN 1000:3000:2::45    0045.0100.0002  2000::100          -   
1302  1302   VXLAN 1000:3000:2::45    0045.0100.0002  2000::100          -   
1302  1302   VXLAN 1000:3000:2::42    0042.0100.0002  2000::42           -   
1302  1302   VXLAN fe80::2aa:aaff:fea 00aa.aaaa.aaaa  2000::56           Stic
                   a:aaaa                                                ky  
1302  1302   VXLAN 1000:3000:2::254   00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1302  1302   VXLAN 1000:3000:2:0:245: 0045.0100.0002  2000::100          -   
                   1ff:fe00:2                                                
1302  1302   VXLAN 1000:3000:2:0:245: 0045.0100.0002  2000::100          -   
                   1ff:fe00:2                                                
1302  1302   VXLAN 10.30.2.254        00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1303  1303   VXLAN fe80::222:ff:fe00: 0022.0000.0003  2000::23           -   
                   3                                                         
1304  1304   VXLAN fe80::256:ff:fe00: 0056.0000.0004  2000::56           -   
                   4                                                         
1304  1304   VXLAN fe80::222:ff:fe00: 0022.0000.0004  2000::22           -   
                   4                                                         
1304  1304   VXLAN 1000:3000:4::56    0056.0000.0004  2000::56           -   
1304  1304   VXLAN fe80::2aa:aaff:fea 00aa.aaaa.aaaa  2000::56           Stic
                   a:aaaa                                                ky  
1304  1304   VXLAN 1000:3000:4::22    0022.0000.0004  2000::23           -   
1304  1304   VXLAN 10.30.4.254        00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1304  1304   VXLAN 1000:3000:4::254   00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
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
192.168.20.2      0:01:16  bcea.fa02.6ce2  Management1
192.168.20.19     0:03:18  c407.7858.8001  Management1
192.168.20.20     0:04:43  e484.29d0.4001  Management1
192.168.20.23     0:03:12  c407.780a.7750  Management1
192.168.20.24     0:01:47  6c87.2089.ede5  Management1
192.168.20.26     0:01:53  04a9.59d5.df66  Management1
192.168.20.27     0:01:41  04a9.59d5.dfe6  Management1
192.168.20.28     0:01:53  98a9.2d59.bae6  Management1
192.168.20.29     0:00:52  90f7.b223.d466  Management1
192.168.21.50     0:01:35  a84f.b1a5.5221  Management1
192.168.21.59     0:04:25  6607.f5d1.ae16  Management1

VRF: tenant-a
Address         Age (sec)  Hardware Addr   Interface
```

## show vxlan address-table

```text
          Vxlan Mac Address Table
----------------------------------------------------------------------

VLAN  Mac Address     Type      Prt  VTEP             Moves   Last Move
----  -----------     ----      ---  ----             -----   ---------
1301  0022.0000.0001  EVPN      Vx1  2000::23         1       0:09:26 ago
1301  0042.0100.0001  EVPN      Vx1  2000::42         1       0:09:15 ago
1301  0045.0100.0001  EVPN      Vx1  2000::100        1       0:09:15 ago
1302  0022.0000.0002  EVPN      Vx1  2000::23         1       0:09:26 ago
1302  0042.0100.0002  EVPN      Vx1  2000::42         1       0:09:15 ago
1302  0045.0100.0002  EVPN      Vx1  2000::100        1       0:09:15 ago
1302  0056.0000.0002  EVPN      Vx1  2000::56         1       0:04:25 ago
1303  0022.0000.0003  EVPN      Vx1  2000::22         2       0:09:26 ago
                                     2000::23       
1304  0022.0000.0004  EVPN      Vx1  2000::22         2       0:09:26 ago
                                     2000::23       
1304  0056.0000.0004  EVPN      Vx1  2000::56         1       0:04:25 ago
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
1301    0022.0000.0001    DYNAMIC     Vx1        1       0:09:26 ago
1301    0042.0100.0001    DYNAMIC     Vx1        1       0:09:15 ago
1301    0045.0100.0001    DYNAMIC     Vx1        1       0:09:15 ago
1301    00aa.aaaa.aaaa    STATIC      Router
1301    2cdd.e90b.25b7    STATIC      Router
1302    0022.0000.0002    DYNAMIC     Vx1        1       0:09:26 ago
1302    0042.0100.0002    DYNAMIC     Vx1        1       0:09:15 ago
1302    0045.0100.0002    DYNAMIC     Vx1        1       0:09:15 ago
1302    0056.0000.0002    DYNAMIC     Vx1        1       0:04:25 ago
1302    00aa.aaaa.aaaa    STATIC      Router
1302    2cdd.e90b.25b7    STATIC      Router
1303    0022.0000.0003    DYNAMIC     Vx1        2       0:09:26 ago
1303    00aa.aaaa.aaaa    STATIC      Router
1303    2cdd.e90b.25b7    STATIC      Router
1304    0022.0000.0004    DYNAMIC     Vx1        2       0:09:26 ago
1304    0056.0000.0004    DYNAMIC     Vx1        1       0:04:25 ago
1304    00aa.aaaa.aaaa    STATIC      Router
1304    2cdd.e90b.25b7    STATIC      Router
4092    00aa.aaaa.aaaa    STATIC      Router
4092    2cdd.e90b.25b7    STATIC      Router
Total Mac Addresses for this criterion: 22

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
0056.0000.0004, VLAN 1304, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::56
0045.0100.0001, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::100
0042.0100.0001, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::42
0045.0100.0002, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::100
0022.0000.0001, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::23
0022.0000.0004, VLAN 1304, seq 2, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 110: 2-way
      VTEP 2000::22
      VTEP 2000::23
0022.0000.0003, VLAN 1303, seq 2, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 110: 2-way
      VTEP 2000::22
      VTEP 2000::23
0022.0000.0002, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::23
0042.0100.0002, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::42
0056.0000.0002, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 2000::56
00aa.aaaa.aaaa, VLAN 1304, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 2000::56
00aa.aaaa.aaaa, VLAN 1302, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 2000::56
```

## show vxlan flood vtep domain local

```text
          VXLAN Flood VTEP Table
--------------------------------------------------------------------------------

VLANS                            Ip Address
-----------------------------   ------------------------------------------------
1201                            2000::201      
1301-1302                       2000::22        2000::23        2000::42       
                                2000::56        2000::100       2000::201      
                                2000::203       2000::204      
1303-1304                       2000::22        2000::23        2000::56       
                                2000::201       2000::203       2000::204      
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
  Local VXLAN IP address: 2000::202
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
  Route distinguisher: 100.0.0.202:1301
  Route target import: Route-Target-AS:1301:1301
  Route target export: Route-Target-AS:1301:1301
  Service interface: VLAN-based
  Local VXLAN IP address: 2000::202
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
  Route distinguisher: 100.0.0.202:1302
  Route target import: Route-Target-AS:1302:1302
  Route target export: Route-Target-AS:1302:1302
  Service interface: VLAN-based
  Local VXLAN IP address: 2000::202
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
  Route distinguisher: 100.0.0.202:1303
  Route target import: Route-Target-AS:1303:1303
  Route target export: Route-Target-AS:1303:1303
  Service interface: VLAN-aware bundle
  Local VXLAN IP address: 2000::202
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
Et1        up       1500  fe80::2edd:e9ff:fe0b:25b7/64  up          link local 
Lo0        up      65535  fe80::ff:fe00:0/64            up          link local 
                          2000::202/128                 up          config     
Vl1201     up       1500  fe80::2edd:e9ff:fe0b:25b7/64  up          link local 
                          1000:1000:201::254/64         up          config     
Vl1301     up       1500  fe80::2edd:e9ff:fe0b:25b7/64  up          link local 
                          1000:3000:1::254/64           up          config     
Vl1302     up       1500  fe80::2edd:e9ff:fe0b:25b7/64  up          link local 
                          1000:3000:2::254/64           up          config     
Vl1303     up       1500  fe80::2edd:e9ff:fe0b:25b7/64  up          link local 
                          1000:3000:3::254/64           up          config     
Vl1304     up       1500  fe80::2edd:e9ff:fe0b:25b7/64  up          link local 
                          1000:3000:4::254/64           up          config     
Vl4092     up       9164  fe80::2edd:e9ff:fe0b:25b7/64  up          link local 

```

## show ipv6 bgp summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.202, local AS number 65202
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor                      V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
                           fe80::464c:a8ff:fe73:5c75%Et1 4 65000            355       263    0    0 00:09:31 Estab   12     12
```

## show ipv6 bgp

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
RPKI Origin Validation codes: V - valid, I - invalid, U - unknown
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
 * >      2000::22/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65022 i
 * >      2000::23/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65023 i
 * >      2000::42/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65042 ?
 * >      2000::45/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65045 ?
 * >      2000::46/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65045 ?
 * >      2000::56/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65056 ?
 * >      2000::100/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65045 ?
 * >      2000::200/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 i
 * >      2000::201/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65201 i
 * >      2000::202/128          -                     -       -          -       0       i
 * >      2000::203/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65203 i
 * >      2000::204/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65204 i
 * >      2001::56/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65056 i
```

## show ipv6 route

```text

VRF: default
Displaying 13 of 16 IPv6 routing table entries
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
 C        2000::202/128 [0/0]
           via Loopback0, directly connected
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
Router identifier 100.0.0.202, local AS number 65202
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
RPKI Origin Validation codes: V - valid, I - invalid, U - unknown
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
 * >      2000::22/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65022 i
 * >      2000::23/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65023 i
 * >      2000::42/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65042 ?
 * >      2000::45/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65045 ?
 * >      2000::46/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65045 ?
 * >      2000::56/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65056 ?
 * >      2000::100/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65045 ?
 * >      2000::200/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 i
 * >      2000::201/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65201 i
 * >      2000::202/128          -                     -       -          -       0       i
 * >      2000::203/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65203 i
 * >      2000::204/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65204 i
 * >      2001::56/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65056 i
BGP routing table information for VRF tenant-a
Router identifier 100.0.1.202, local AS number 65202
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
RPKI Origin Validation codes: V - valid, I - invalid, U - unknown
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
 * >Ec    1000:1000:22::/64      2000::23              0       -          100     0       65000 65023 i
 *  ec    1000:1000:22::/64      2000::22              0       -          100     0       65000 65022 i
 * >Ec    1000:1000:22::254/128  2000::23              0       -          100     0       65000 65023 i
 *  ec    1000:1000:22::254/128  2000::22              0       -          100     0       65000 65022 i
 * >      1000:1000:42::/64      2000::42              0       -          100     0       65000 65042 ?
 * >      1000:1000:42::42/128   2000::42              0       -          100     0       65000 65042 i
 * >      1000:1000:42:0:242:1ff:fe00:3/128 2000::42              0       -          100     0       65000 65042 i
 * >Ec    1000:1000:45::/64      2000::100             0       -          100     0       65000 65045 ?
 *  ec    1000:1000:45::/64      2000::100             0       -          100     0       65000 65045 ?
 * >Ec    1000:1000:45::45/128   2000::100             0       -          100     0       65000 65045 i
 *  ec    1000:1000:45::45/128   2000::100             0       -          100     0       65000 65045 i
 * >Ec    1000:1000:45:0:245:1ff:fe00:3/128 2000::100             0       -          100     0       65000 65045 i
 *  ec    1000:1000:45:0:245:1ff:fe00:3/128 2000::100             0       -          100     0       65000 65045 i
 * >      1000:1000:56::/64      2000::56              0       -          100     0       65000 65056 i
 * >      1000:1000:56::56/128   2000::56              0       -          100     0       65000 65056 i
 * >      1000:1000:201::/64     -                     -       -          -       0       i
 *        1000:1000:201::/64     2000::201             0       -          100     0       65000 65201 i
 * >Ec    1000:1000:203::/64     2000::204             0       -          100     0       65000 65204 i
 *  ec    1000:1000:203::/64     2000::203             0       -          100     0       65000 65203 i
 * >      1000:3000:1::/64       -                     -       -          -       0       i
 *  Ec    1000:3000:1::/64       2000::204             0       -          100     0       65000 65204 i
 *  ec    1000:3000:1::/64       2000::23              0       -          100     0       65000 65023 i
 *  ec    1000:3000:1::/64       2000::203             0       -          100     0       65000 65203 i
 *  ec    1000:3000:1::/64       2000::201             0       -          100     0       65000 65201 i
 *  ec    1000:3000:1::/64       2000::56              0       -          100     0       65000 65056 i
 *  ec    1000:3000:1::/64       2000::22              0       -          100     0       65000 65022 i
 *        1000:3000:1::/64       2000::42              0       -          100     0       65000 65042 ?
 *        1000:3000:1::/64       2000::100             0       -          100     0       65000 65045 ?
 *        1000:3000:1::/64       2000::100             0       -          100     0       65000 65045 ?
 * >      1000:3000:1::22/128    2000::22              0       -          100     0       65000 65022 i
 * >      1000:3000:1::42/128    2000::42              0       -          100     0       65000 65042 i
 * >Ec    1000:3000:1::45/128    2000::100             0       -          100     0       65000 65045 i
 *  ec    1000:3000:1::45/128    2000::100             0       -          100     0       65000 65045 i
 * >      1000:3000:1::56/128    2000::56              0       -          100     0       65000 65056 i
 * >Ec    1000:3000:1::254/128   2000::23              0       -          100     0       65000 65023 i
 *  ec    1000:3000:1::254/128   2000::22              0       -          100     0       65000 65022 i
 * >      1000:3000:1:0:242:1ff:fe00:1/128 2000::42              0       -          100     0       65000 65042 i
 * >Ec    1000:3000:1:0:245:1ff:fe00:1/128 2000::100             0       -          100     0       65000 65045 i
 *  ec    1000:3000:1:0:245:1ff:fe00:1/128 2000::100             0       -          100     0       65000 65045 i
 * >      1000:3000:2::/64       -                     -       -          -       0       i
 *  Ec    1000:3000:2::/64       2000::204             0       -          100     0       65000 65204 i
 *  ec    1000:3000:2::/64       2000::203             0       -          100     0       65000 65203 i
 *  ec    1000:3000:2::/64       2000::201             0       -          100     0       65000 65201 i
 *  ec    1000:3000:2::/64       2000::56              0       -          100     0       65000 65056 i
 *        1000:3000:2::/64       2000::42              0       -          100     0       65000 65042 ?
 *        1000:3000:2::/64       2000::100             0       -          100     0       65000 65045 ?
 *        1000:3000:2::/64       2000::100             0       -          100     0       65000 65045 ?
 * >      1000:3000:2::22/128    2000::23              0       -          100     0       65000 65023 i
 * >      1000:3000:2::42/128    2000::42              0       -          100     0       65000 65042 i
 * >Ec    1000:3000:2::45/128    2000::100             0       -          100     0       65000 65045 i
 *  ec    1000:3000:2::45/128    2000::100             0       -          100     0       65000 65045 i
 * >      1000:3000:2::56/128    2000::56              0       -          100     0       65000 65056 i
 * >      1000:3000:2:0:242:1ff:fe00:2/128 2000::42              0       -          100     0       65000 65042 i
 * >Ec    1000:3000:2:0:245:1ff:fe00:2/128 2000::100             0       -          100     0       65000 65045 i
 *  ec    1000:3000:2:0:245:1ff:fe00:2/128 2000::100             0       -          100     0       65000 65045 i
 * >      1000:3000:3::/64       -                     -       -          -       0       i
 *  Ec    1000:3000:3::/64       2000::204             0       -          100     0       65000 65204 i
 *  ec    1000:3000:3::/64       2000::23              0       -          100     0       65000 65023 i
 *  ec    1000:3000:3::/64       2000::203             0       -          100     0       65000 65203 i
 *  ec    1000:3000:3::/64       2000::201             0       -          100     0       65000 65201 i
 *  ec    1000:3000:3::/64       2000::56              0       -          100     0       65000 65056 i
 *  ec    1000:3000:3::/64       2000::22              0       -          100     0       65000 65022 i
 * >      1000:3000:3::56/128    2000::56              0       -          100     0       65000 65056 i
 * >Ec    1000:3000:3::254/128   2000::23              0       -          100     0       65000 65023 i
 *  ec    1000:3000:3::254/128   2000::22              0       -          100     0       65000 65022 i
 * >      1000:3000:4::/64       -                     -       -          -       0       i
 *  Ec    1000:3000:4::/64       2000::204             0       -          100     0       65000 65204 i
 *  ec    1000:3000:4::/64       2000::203             0       -          100     0       65000 65203 i
 *  ec    1000:3000:4::/64       2000::201             0       -          100     0       65000 65201 i
 *  ec    1000:3000:4::/64       2000::56              0       -          100     0       65000 65056 i
 * >      1000:3000:4::22/128    2000::23              0       -          100     0       65000 65023 i
 * >      1000:3000:4::56/128    2000::56              0       -          100     0       65000 65056 i
```

## show ipv6 route vrf all

```text

VRF: default
Displaying 13 of 16 IPv6 routing table entries
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
 C        2000::202/128 [0/0]
           via Loopback0, directly connected
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
Displaying 31 of 39 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 B E      1000:1000:22::254/128 [20/0]
           via VTEP 2000::23 VNI 1000 router-mac c4:07:78:0a:77:7d
           via VTEP 2000::22 VNI 1000 router-mac c4:07:78:0a:9f:31
 B E      1000:1000:22::/64 [20/0]
           via VTEP 2000::23 VNI 1000 router-mac c4:07:78:0a:77:7d
           via VTEP 2000::22 VNI 1000 router-mac c4:07:78:0a:9f:31
 B E      1000:1000:42::42/128 [20/0]
           via VTEP 2000::42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      1000:1000:42:0:242:1ff:fe00:3/128 [20/0]
           via VTEP 2000::42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      1000:1000:42::/64 [20/0]
           via VTEP 2000::42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      1000:1000:45::45/128 [20/0]
           via VTEP 2000::100 VNI 1000 router-mac 06:00:00:00:01:00
 B E      1000:1000:45:0:245:1ff:fe00:3/128 [20/0]
           via VTEP 2000::100 VNI 1000 router-mac 06:00:00:00:01:00
 B E      1000:1000:45::/64 [20/0]
           via VTEP 2000::100 VNI 1000 router-mac 06:00:00:00:01:00
 B E      1000:1000:56::56/128 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      1000:1000:56::/64 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 C        1000:1000:201::/64 [0/0]
           via Vlan1201, directly connected
 B E      1000:1000:203::/64 [20/0]
           via VTEP 2000::204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 2000::203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 B E      1000:3000:1::22/128 [20/0]
           via VTEP 2000::22 VNI 1000 router-mac c4:07:78:0a:9f:31
 B E      1000:3000:1::42/128 [20/0]
           via VTEP 2000::42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      1000:3000:1::45/128 [20/0]
           via VTEP 2000::100 VNI 1000 router-mac 06:00:00:00:01:00
 B E      1000:3000:1::56/128 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      1000:3000:1:0:242:1ff:fe00:1/128 [20/0]
           via VTEP 2000::42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      1000:3000:1:0:245:1ff:fe00:1/128 [20/0]
           via VTEP 2000::100 VNI 1000 router-mac 06:00:00:00:01:00
 C        1000:3000:1::/64 [0/0]
           via Vlan1301, directly connected
 B E      1000:3000:2::22/128 [20/0]
           via VTEP 2000::23 VNI 1000 router-mac c4:07:78:0a:77:7d
 B E      1000:3000:2::42/128 [20/0]
           via VTEP 2000::42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      1000:3000:2::45/128 [20/0]
           via VTEP 2000::100 VNI 1000 router-mac 06:00:00:00:01:00
 B E      1000:3000:2::56/128 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      1000:3000:2:0:242:1ff:fe00:2/128 [20/0]
           via VTEP 2000::42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      1000:3000:2:0:245:1ff:fe00:2/128 [20/0]
           via VTEP 2000::100 VNI 1000 router-mac 06:00:00:00:01:00
 C        1000:3000:2::/64 [0/0]
           via Vlan1302, directly connected
 B E      1000:3000:3::56/128 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 C        1000:3000:3::/64 [0/0]
           via Vlan1303, directly connected
 B E      1000:3000:4::22/128 [20/0]
           via VTEP 2000::23 VNI 1000 router-mac c4:07:78:0a:77:7d
 B E      1000:3000:4::56/128 [20/0]
           via VTEP 2000::56 VNI 1000 router-mac 00:01:00:00:00:56
 C        1000:3000:4::/64 [0/0]
           via Vlan1304, directly connected

```

## show bgp ipv6 unicast summary lldp

```text
BGP summary information for VRF default
Router identifier 100.0.0.202, local AS number 65202
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor                      LLDP Neighbor                  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
                           fe80::464c:a8ff:fe73:5c75%Et1 SPINE1-J-200.ns.eantc.de       4 65000            355       263    0    0 00:09:31 Estab   12     12
```

## show ipv6 neighbors vrf all

```text

VRF: default
IPv6 Address                                  Age Hardware Addr   Interface
fe80::464c:a8ff:fe73:5c75                 0:00:32 444c.a873.5c75  Et1

VRF: mgmt
IPv6 Address                                  Age Hardware Addr   Interface

VRF: tenant-a
IPv6 Address                                  Age Hardware Addr   Interface
fe80::220:30ff:fe00:5                     1:59:53 0020.3000.0005  Vl1201, not learned
1000:3000:1::42                                 - 0042.0100.0001  Vl1301, Vxlan1
1000:3000:1::45                                 - 0045.0100.0001  Vl1301, Vxlan1
1000:3000:1::201                          0:48:13 0020.1000.0001  Vl1301, not learned
1000:3000:1:0:242:1ff:fe00:1                    - 0042.0100.0001  Vl1301, Vxlan1
1000:3000:1:0:245:1ff:fe00:1                    - 0045.0100.0001  Vl1301, Vxlan1
fe80::220:10ff:fe00:1                     1:59:53 0020.1000.0001  Vl1301, not learned
fe80::220:30ff:fe00:1                     1:59:53 0020.3000.0001  Vl1301, not learned
1000:3000:2::22                                 - 0022.0000.0002  Vl1302, Vxlan1
1000:3000:2::42                                 - 0042.0100.0002  Vl1302, Vxlan1
1000:3000:2::45                                 - 0045.0100.0002  Vl1302, Vxlan1
1000:3000:2::56                                 - 0056.0000.0002  Vl1302, Vxlan1
1000:3000:2:0:242:1ff:fe00:2                    - 0042.0100.0002  Vl1302, Vxlan1
1000:3000:2:0:245:1ff:fe00:2                    - 0045.0100.0002  Vl1302, Vxlan1
1000:3000:4::56                                 - 0056.0000.0004  Vl1304, Vxlan1
fe80::220:10ff:fe00:4                     1:59:52 0020.1000.0004  Vl1304, not learned
fe80::220:30ff:fe00:4                     1:59:53 0020.3000.0004  Vl1304, not learned
```

## show ipv6 neighbors remote

```text
ARP remote bindings
VLAN IP Address                   MAC Address    Source         
---- ---------------------------- -------------- ---------------
1301 1000:3000:1::42              0042.0100.0001 EVPN remote    
1301 1000:3000:1::45              0045.0100.0001 EVPN remote    
1301 1000:3000:1:0:242:1ff:fe00:1 0042.0100.0001 EVPN remote    
1301 1000:3000:1:0:245:1ff:fe00:1 0045.0100.0001 EVPN remote    
1301 fe80::222:ff:fe00:1          0022.0000.0001 EVPN remote    
1302 1000:3000:2::22              0022.0000.0002 EVPN remote    
1302 1000:3000:2::42              0042.0100.0002 EVPN remote    
1302 1000:3000:2::45              0045.0100.0002 EVPN remote    
1302 1000:3000:2::56              0056.0000.0002 EVPN remote    
1302 1000:3000:2::254             00aa.aaaa.aaaa EVPN remote    
1302 1000:3000:2:0:242:1ff:fe00:2 0042.0100.0002 EVPN remote    
1302 1000:3000:2:0:245:1ff:fe00:2 0045.0100.0002 EVPN remote    
1302 fe80::222:ff:fe00:2          0022.0000.0002 EVPN remote    
1302 fe80::256:ff:fe00:2          0056.0000.0002 EVPN remote    
1302 fe80::2aa:aaff:feaa:aaaa     00aa.aaaa.aaaa EVPN remote    
1303 fe80::222:ff:fe00:3          0022.0000.0003 EVPN remote    
1304 1000:3000:4::56              0056.0000.0004 EVPN remote    
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
   Ethernet1       fe80::464c:a8ff:fe73:5c75      0:00:55 ago   

```

## show ipv6 nd ra neighbors vrf tenant-a

```text
VRF: tenant-a
```

## show interfaces counters rates | nz

```text
Port      Name       Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Et1       ANET 200    0:01      0.0   0.0%        0      0.0   0.0%        0
Ma1                   0:05      0.1   0.0%        0      0.2   0.0%        0
```

