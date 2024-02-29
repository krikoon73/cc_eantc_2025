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
  Description              Neighbor V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.204, local AS number 65204
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  NODE200.EVPN             2000::200 4 65000           2085       483    0    0 00:09:26 Estab   202    202
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.204, local AS number 65204
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
    2000::203 from 2000::200 (100.0.0.200)
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
    2000::203 from 2000::200 (100.0.0.200)
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
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1203:1203 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.204, local AS number 65204
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
Router identifier 100.0.0.204, local AS number 65204
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
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
      PMSI Tunnel: Ingress Replication, MPLS Label: 1203, Leaf Information Required: false, Tunnel ID: 2000::204
BGP routing table entry for imet 2000::204, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::204
BGP routing table entry for imet 2000::204, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 2000::203
BGP routing table entry for imet 1303 2000::204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 2000::203
BGP routing table entry for imet 1304 2000::204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 2000::204
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.204, local AS number 65204
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
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:30:02:04 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0203:0204 2000::204, Route Distinguisher: 100.0.0.204:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:30:02:04 DF Election: Preference 100
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.204, local AS number 65204
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
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
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
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
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
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
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
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
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
  65000 65203
    2000::203 from 2000::200 (100.0.0.200)
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
1203  1203   VXLAN 10.10.203.203      6666.6666.0001  100.0.0.103        -   
1203  1203   VXLAN 10.10.203.204      444c.a873.5c75  100.0.0.203        -   
1203  1203   VXLAN 10.10.203.203      001b.0100.0001  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.190      a222.0100.0058  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.204      a222.0100.0066  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.202        444c.a873.5c75  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.133      a222.0100.001f  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.182      a222.0100.0050  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.199      a222.0100.0061  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.179        a244.0100.0051  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.188      a222.0100.0056  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.146        a244.0100.0030  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.130        a244.0100.0020  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.128        a244.0100.001e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.185        a244.0100.0057  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.133        a244.0100.0023  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.162      a222.0100.003c  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.153        a244.0100.0037  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.155      a222.0100.0035  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.106        a244.0100.0008  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.147        a244.0100.0031  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.105      a222.0100.0003  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.238        001b.0100.0058  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.135        a244.0100.0025  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.232        001b.0100.0052  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.128      a222.0100.001a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.221        001b.0100.0047  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.103        a244.0101.0001  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.208        001b.0100.003a  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.131      a222.0100.001d  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.156      a222.0100.0036  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.245        001b.0100.005f  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.209        001b.0100.003b  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.122        a244.0100.0018  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.192      a222.0100.005a  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.145      a222.0100.002b  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.236        001b.0100.0056  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.237        001b.0100.0057  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.244        001b.0100.005e  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.131        a244.0100.0021  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.183      a222.0100.0051  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.105        a244.0100.0007  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.239        001b.0100.0059  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.157        a244.0100.003b  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.197      a222.0100.005f  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.159      a222.0100.0039  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.176      a222.0100.004a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.216        001b.0100.0042  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.189      a222.0100.0057  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.186        a244.0100.0058  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.177        a244.0100.004f  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.173        a244.0100.004b  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.240        001b.0100.005a  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.165      a222.0100.003f  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.145        a244.0100.002f  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.118        a244.0100.0014  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.241        001b.0100.005b  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.132        a244.0100.0022  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.139      a222.0100.0025  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.169        a244.0100.0047  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.152        a244.0100.0036  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.114        a244.0100.0010  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.171      a222.0100.0045  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.246        001b.0100.0060  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.203        001b.0100.0035  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.173      a222.0100.0047  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.118      a222.0100.0010  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.182        a244.0100.0054  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.149      a222.0100.002f  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.167      a222.0100.0041  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.183        a244.0100.0055  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.101        a244.0100.0003  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.125        a244.0100.001b  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.125      a222.0100.0017  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.168      a222.0100.0042  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.196        a244.0100.0062  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.177      a222.0100.004b  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.229        001b.0100.004f  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.222        001b.0100.0048  100.0.0.203        -   
1301  1301   VXLAN 1000:3000:1::45    0045.0100.0001  2000::100          -   
1301  1301   VXLAN 1000:3000:1::45    0045.0100.0001  2000::100          -   
1301  1301   VXLAN 10.30.1.204        001b.0100.0036  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.242        001b.0100.005c  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.190        a244.0100.005c  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.115      a222.0100.000d  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.108      a222.0100.0006  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.127        a244.0100.001d  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.123        a244.0100.0019  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.121      a222.0100.0013  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.123      a222.0100.0015  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.136      a222.0100.0022  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.121        a244.0100.0017  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.187      a222.0100.0055  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.180        a244.0100.0052  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.137        a244.0100.0027  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.226        001b.0100.004c  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.115        a244.0100.0011  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.114      a222.0100.000c  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.206        001b.0100.0038  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.195        a244.0100.0061  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.179      a222.0100.004d  100.0.0.201        -   
1301  1301   VXLAN 1000:3000:1:0:245: 0045.0100.0001  2000::100          -   
                   1ff:fe00:1                                                
1301  1301   VXLAN 1000:3000:1:0:245: 0045.0100.0001  2000::100          -   
                   1ff:fe00:1                                                
1301  1301   VXLAN 10.30.1.174        a244.0100.004c  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.117      a222.0100.000f  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.203        001b.0100.0002  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.124      a222.0100.0016  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.225        001b.0100.004b  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.122      a222.0100.0014  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.109      a222.0100.0007  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.217        001b.0100.0043  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.134        a244.0100.0024  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.184      a222.0100.0052  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.163      a222.0100.003d  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.200      a222.0100.0062  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.106      a222.0100.0004  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.104        a244.0100.0006  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.152      a222.0100.0032  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.170        a244.0100.0048  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.116      a222.0100.000e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.116        a244.0100.0012  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.224        001b.0100.004a  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.220        001b.0100.0046  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.170      a222.0100.0044  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.99         a244.0100.0001  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.214        001b.0100.0040  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.120      a222.0100.0012  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.149        a244.0100.0033  100.0.0.201        -   
1301  1301   VXLAN fe80::222:ff:fe00: 0022.0000.0001  2000::23           7   
                   1                                                         
1301  1301   VXLAN 10.30.1.223        001b.0100.0049  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.249        001b.0100.0063  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.138        a244.0100.0028  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.171        a244.0100.0049  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.194        a244.0100.0060  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.113        a244.0100.000f  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.129      a222.0100.001b  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.200        a244.0100.0066  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.144        a244.0100.002e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.100        a244.0100.0002  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.164      a222.0100.003e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.230        001b.0100.0050  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.169      a222.0100.0043  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.201      a222.0100.0063  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.136        a244.0100.0026  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.193        a244.0100.005f  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.134      a222.0100.0020  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.211        001b.0100.003d  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.162        a244.0100.0040  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.103        a244.0100.0005  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.127      a222.0100.0019  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.107        a244.0100.0009  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.186      a222.0100.0054  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.146      a222.0100.002c  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.193      a222.0100.005b  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.104      a222.0100.0002  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.175        a244.0100.004d  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.140        a244.0100.002a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.156        a244.0100.003a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.247        001b.0100.0061  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.147      a222.0100.002d  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.210        001b.0100.003c  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.250        001b.0100.0064  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.248        001b.0100.0062  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.154      a222.0100.0034  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.143        a244.0100.002d  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.197        a244.0100.0063  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.140      a222.0100.0026  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.231        001b.0100.0051  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.148      a222.0100.002e  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.194      a222.0100.005c  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.130      a222.0100.001c  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.141      a222.0100.0027  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.166        a244.0100.0044  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.192        a244.0100.005e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.112        a244.0100.000e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.187        a244.0100.0059  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.175      a222.0100.0049  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.212        001b.0100.003e  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.126        a244.0100.001c  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.132      a222.0100.001e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.207        001b.0100.0039  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.124        a244.0100.001a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.155        a244.0100.0039  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.176        a244.0100.004e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.102        a244.0100.0004  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.195      a222.0100.005d  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.167        a244.0100.0045  100.0.0.201        -   
1301  1301   VXLAN 1000:3000:1::42    0042.0100.0001  2000::42           -   
1301  1301   VXLAN 10.10.103.166      a222.0100.0040  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.218        001b.0100.0044  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.215        001b.0100.0041  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.139        a244.0100.0029  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.119      a222.0100.0011  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.110        a244.0100.000c  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.191        a244.0100.005d  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.201        001b.0100.0033  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.233        001b.0100.0053  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.188        a244.0100.005a  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.144      a222.0100.002a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.235        001b.0100.0055  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.107      a222.0100.0005  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.103      a222.0100.0001  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.113      a222.0100.000b  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.158        a244.0100.003c  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.189        a244.0100.005b  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.234        001b.0100.0054  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.181      a222.0100.004f  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.160      a222.0100.003a  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.151      a222.0100.0031  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.135      a222.0100.0021  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.184        a244.0100.0056  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.172      a222.0100.0046  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.126      a222.0100.0018  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.201        001b.0100.0002  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.142      a222.0100.0028  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.198        a244.0100.0064  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.151        a244.0100.0035  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.137      a222.0100.0023  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.161      a222.0100.003b  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.165        a244.0100.0043  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.228        001b.0100.004e  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.203      a222.0100.0065  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.172        a244.0100.004a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.150        a244.0100.0034  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.196      a222.0100.005e  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.111      a222.0100.0009  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.185      a222.0100.0053  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.227        001b.0100.004d  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.143      a222.0100.0029  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.178      a222.0100.004c  100.0.0.201        -   
1301  1301   VXLAN 1000:3000:1:0:242: 0042.0100.0001  2000::42           -   
                   1ff:fe00:1                                                
1301  1301   VXLAN 10.10.103.157      a222.0100.0037  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.174      a222.0100.0048  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.117        a244.0100.0013  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.164        a244.0100.0042  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.181        a244.0100.0053  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.138      a222.0100.0024  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.202        001b.0100.0034  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.202      a222.0100.0064  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.141        a244.0100.002b  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.111        a244.0100.000d  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.109        a244.0100.000b  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.108        a244.0100.000a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.119        a244.0100.0015  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.148        a244.0100.0032  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.180      a222.0100.004e  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.153      a222.0100.0033  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.158      a222.0100.0038  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.198      a222.0100.0060  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.110      a222.0100.0008  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.203        6666.6668.0001  100.0.0.103        -   
1301  1301   VXLAN 10.30.1.120        a244.0100.0016  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.178        a244.0100.0050  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.163        a244.0100.0041  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.50         3333.3333.3333  100.0.0.201        Stic
                                                                         ky  
1301  1301   VXLAN 1000:3000:1::22    0022.0000.0001  2000::22           3   
1301  1301   VXLAN 10.30.1.213        001b.0100.003f  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.243        001b.0100.005d  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.205        001b.0100.0037  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.150      a222.0100.0030  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.168        a244.0100.0046  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.112      a222.0100.000a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.159        a244.0100.003d  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.44         001c.0100.0002  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.191      a222.0100.0059  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.161        a244.0100.003f  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.154        a244.0100.0038  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.160        a244.0100.003e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.129        a244.0100.001f  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.219        001b.0100.0045  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.199        a244.0100.0065  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.142        a244.0100.002c  100.0.0.201        -   
1302  1302   VXLAN 1000:3000:2::56    0056.0000.0002  2000::56           -   
1302  1302   VXLAN 1000:3000:2:0:242: 0042.0100.0002  2000::42           -   
                   1ff:fe00:2                                                
1302  1302   VXLAN fe80::222:ff:fe00: 0022.0000.0002  2000::23           2   
                   2                                                         
1302  1302   VXLAN 1000:3000:2:0:245: 0045.0100.0002  2000::100          -   
                   1ff:fe00:2                                                
1302  1302   VXLAN 1000:3000:2:0:245: 0045.0100.0002  2000::100          -   
                   1ff:fe00:2                                                
1302  1302   VXLAN fe80::256:ff:fe00: 0056.0000.0002  2000::56           -   
                   2                                                         
1302  1302   VXLAN 10.30.2.202        444c.a873.5c75  100.0.0.203        -   
1302  1302   VXLAN 1000:3000:2::42    0042.0100.0002  2000::42           -   
1302  1302   VXLAN 1000:3000:2::45    0045.0100.0002  2000::100          -   
1302  1302   VXLAN 1000:3000:2::45    0045.0100.0002  2000::100          -   
1302  1302   VXLAN 10.30.2.254        00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1302  1302   VXLAN fe80::2aa:aaff:fea 00aa.aaaa.aaaa  2000::56           Stic
                   a:aaaa                                                ky  
1302  1302   VXLAN 1000:3000:2::254   00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1302  1302   VXLAN 1000:3000:2::22    0022.0000.0002  2000::23           9   
1303  1303   VXLAN fe80::222:ff:fe00: 0022.0000.0003  2000::23           -   
                   3                                                         
1304  1304   VXLAN 1000:3000:4::254   00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1304  1304   VXLAN fe80::256:ff:fe00: 0056.0000.0004  2000::56           -   
                   4                                                         
1304  1304   VXLAN 1000:3000:4::22    0022.0000.0004  2000::23           -   
1304  1304   VXLAN 10.30.4.254        00aa.aaaa.aaaa  2000::56           Stic
                                                                         ky  
1304  1304   VXLAN fe80::222:ff:fe00: 0022.0000.0004  2000::22           -   
                   4                                                         
1304  1304   VXLAN 1000:3000:4::56    0056.0000.0004  2000::56           -   
1304  1304   VXLAN fe80::2aa:aaff:fea 00aa.aaaa.aaaa  2000::56           Stic
                   a:aaaa                                                ky  
0     2303   VXLAN 10.30.3.14         f8c1.1604.3007  100.0.30.14        Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.14         f8c1.1604.3007  100.0.30.14        Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.103        a266.0102.0001  100.0.30.14        -   
0     2303   VXLAN 10.30.3.250        001b.0100.0096  100.0.30.14        2   
0     2303   VXLAN 10.30.3.203        001b.0100.0003  100.0.30.14        6   
0     2303   VXLAN 10.30.3.254        0056.5656.5656  100.0.30.14        Stic
                                                                         ky  
0     2303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.30.14        Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.30.14        -   
0     2304   VXLAN 10.30.4.103        a288.0103.0001  100.0.30.14        -   
0     2304   VXLAN 10.30.4.254        0056.5656.5656  100.0.30.14        Stic
                                                                         ky  
0     2304   VXLAN 10.30.4.250        001b.0100.00c8  100.0.30.14        1   
0     2304   VXLAN 10.30.4.254        00aa.aaaa.aaaa  100.0.30.14        Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.254        00aa.aaaa.aaaa  100.0.30.14        -   
0     2304   VXLAN 10.30.4.14         f8c1.1604.3007  100.0.30.14        Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.14         f8c1.1604.3007  100.0.30.14        Stic
                                                                         ky  
0     2304   VXLAN 10.30.4.203        001b.0100.0004  100.0.30.14        22  
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
192.168.20.2      0:02:14  bcea.fa02.6ce2  Management1
192.168.20.19     0:00:12  c407.7858.8001  Management1
192.168.20.20     0:03:27  e484.29d0.4001  Management1
192.168.20.21     0:00:36  7081.85c1.b801  Management1
192.168.20.23     0:04:10  c407.780a.7750  Management1
192.168.20.24     0:04:16  6c87.2089.ede5  Management1
192.168.20.25     0:00:43  6c87.2089.ece5  Management1
192.168.20.26     0:00:36  04a9.59d5.df66  Management1
192.168.20.27     0:04:40  04a9.59d5.dfe6  Management1
192.168.20.28     0:00:55  98a9.2d59.bae6  Management1
192.168.20.29     0:03:39  90f7.b223.d466  Management1

VRF: tenant-a
Address         Age (sec)  Hardware Addr   Interface
```

## show vxlan address-table

```text
          Vxlan Mac Address Table
----------------------------------------------------------------------

VLAN  Mac Address     Type      Prt  VTEP             Moves   Last Move
----  -----------     ----      ---  ----             -----   ---------
1301  0022.0000.0001  EVPN      Vx1  2000::23         1       0:09:27 ago
1301  0042.0100.0001  EVPN      Vx1  2000::42         1       0:09:15 ago
1301  0045.0100.0001  EVPN      Vx1  2000::100        1       0:09:16 ago
1302  0022.0000.0002  EVPN      Vx1  2000::23         1       0:09:27 ago
1302  0042.0100.0002  EVPN      Vx1  2000::42         1       0:09:15 ago
1302  0045.0100.0002  EVPN      Vx1  2000::100        1       0:09:16 ago
1302  0056.0000.0002  EVPN      Vx1  2000::56         1       0:04:26 ago
1303  0022.0000.0003  EVPN      Vx1  2000::22         2       0:09:26 ago
                                     2000::23       
1304  0022.0000.0004  EVPN      Vx1  2000::22         2       0:09:26 ago
                                     2000::23       
1304  0056.0000.0004  EVPN      Vx1  2000::56         1       0:04:26 ago
4092  0001.0000.0056  EVPN      Vx1  2000::56                 0:09:27 ago
4092  0600.0000.0100  EVPN      Vx1  2000::100                0:09:16 ago
4092  246c.8474.8ddb  EVPN      Vx1  2000::40                 0:09:02 ago
4092  2cdd.e90b.2283  EVPN      Vx1  2000::201                0:09:27 ago
4092  2cdd.e90b.25b7  EVPN      Vx1  2000::202                0:09:27 ago
4092  3838.a621.e82f  EVPN      Vx1  2000::203                0:09:27 ago
4092  4014.827b.84ab  EVPN      Vx1  2000::42                 0:09:15 ago
4092  c407.780a.777d  EVPN      Vx1  2000::23                 0:09:36 ago
4092  c407.780a.9f31  EVPN      Vx1  2000::22                 0:09:26 ago
Total Remote Mac Addresses for this criterion: 19
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
1000       4092       tenant-a       evpn         

```

## show mac address-table

```text
          Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports      Moves   Last Move
----    -----------       ----        -----      -----   ---------
1203    00aa.aaaa.aaaa    STATIC      Router
1301    0022.0000.0001    DYNAMIC     Vx1        1       0:09:27 ago
1301    0042.0100.0001    DYNAMIC     Vx1        1       0:09:16 ago
1301    0045.0100.0001    DYNAMIC     Vx1        1       0:09:16 ago
1301    00aa.aaaa.aaaa    STATIC      Router
1302    0022.0000.0002    DYNAMIC     Vx1        1       0:09:27 ago
1302    0042.0100.0002    DYNAMIC     Vx1        1       0:09:16 ago
1302    0045.0100.0002    DYNAMIC     Vx1        1       0:09:16 ago
1302    0056.0000.0002    DYNAMIC     Vx1        1       0:04:26 ago
1302    00aa.aaaa.aaaa    STATIC      Router
1303    0022.0000.0003    DYNAMIC     Vx1        2       0:09:27 ago
1303    00aa.aaaa.aaaa    STATIC      Router
1304    0022.0000.0004    DYNAMIC     Vx1        2       0:09:27 ago
1304    0056.0000.0004    DYNAMIC     Vx1        1       0:04:26 ago
1304    00aa.aaaa.aaaa    STATIC      Router
4092    0001.0000.0056    DYNAMIC     Vx1        0       0:09:27 ago
4092    00aa.aaaa.aaaa    STATIC      Router
4092    0600.0000.0100    DYNAMIC     Vx1        0       0:09:16 ago
4092    246c.8474.8ddb    DYNAMIC     Vx1        0       0:09:02 ago
4092    2cdd.e90b.2283    DYNAMIC     Vx1        0       0:09:27 ago
4092    2cdd.e90b.25b7    DYNAMIC     Vx1        0       0:09:27 ago
4092    3838.a621.e82f    DYNAMIC     Vx1        0       0:09:27 ago
4092    4014.827b.84ab    DYNAMIC     Vx1        0       0:09:16 ago
4092    c407.780a.777d    DYNAMIC     Vx1        0       0:09:36 ago
4092    c407.780a.9f31    DYNAMIC     Vx1        0       0:09:27 ago
Total Mac Addresses for this criterion: 25

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
   Load Balance entry 51: 2-way
      VTEP 2000::22
      VTEP 2000::23
0022.0000.0003, VLAN 1303, seq 2, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 51: 2-way
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
1203                            2000::203      
1301-1302                       2000::22        2000::23        2000::42       
                                2000::56        2000::100       2000::201      
                                2000::202       2000::203      
1303-1304                       2000::22        2000::23        2000::56       
                                2000::201       2000::202       2000::203      
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
EVPN instance: VLAN 1203
  Route distinguisher: 100.0.0.204:1203
  Route target import: Route-Target-AS:1203:1203
  Route target export: Route-Target-AS:1203:1203
  Service interface: VLAN-based
  Local VXLAN IP address: 2000::204
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
  Route distinguisher: 100.0.0.204:1301
  Route target import: Route-Target-AS:1301:1301
  Route target export: Route-Target-AS:1301:1301
  Service interface: VLAN-based
  Local VXLAN IP address: 2000::204
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
  Route distinguisher: 100.0.0.204:1302
  Route target import: Route-Target-AS:1302:1302
  Route target export: Route-Target-AS:1302:1302
  Service interface: VLAN-based
  Local VXLAN IP address: 2000::204
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
  Route distinguisher: 100.0.0.204:1303
  Route target import: Route-Target-AS:1303:1303
  Route target export: Route-Target-AS:1303:1303
  Service interface: VLAN-aware bundle
  Local VXLAN IP address: 2000::204
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
---------- ------- ------ ---------------------------- ------------ -----------
Et1        up       1500  fe80::9a5d:82ff:fea2:4f9/64   up          link local 
Lo0        up      65535  fe80::ff:fe00:0/64            up          link local 
                          2000::204/128                 up          config     
Vl1203     up       1500  fe80::9a5d:82ff:fea2:4f9/64   up          link local 
                          1000:1000:203::254/64         up          config     
Vl1301     up       1500  fe80::9a5d:82ff:fea2:4f9/64   up          link local 
                          1000:3000:1::254/64           up          config     
Vl1302     up       1500  fe80::9a5d:82ff:fea2:4f9/64   up          link local 
                          1000:3000:2::254/64           up          config     
Vl1303     up       1500  fe80::9a5d:82ff:fea2:4f9/64   up          link local 
                          1000:3000:3::254/64           up          config     
Vl1304     up       1500  fe80::9a5d:82ff:fea2:4f9/64   up          link local 
                          1000:3000:4::254/64           up          config     
Vl4092     up       9164  fe80::9a5d:82ff:fea2:4f9/64   up          link local 

```

## show ipv6 bgp summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.204, local AS number 65204
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor                      V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
                           fe80::464c:a8ff:fe73:5c75%Et1 4 65000            346       258    0    0 00:09:31 Estab   12     12
```

## show ipv6 bgp

```text
BGP routing table information for VRF default
Router identifier 100.0.0.204, local AS number 65204
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
 * >      2000::202/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65202 i
 * >      2000::203/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65203 i
 * >      2000::204/128          -                     -       -          -       0       i
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
 B E      2000::202/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::203/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 C        2000::204/128 [0/0]
           via Loopback0, directly connected
 B E      2001::56/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1

```

## show ipv6 bgp vrf all

```text
BGP routing table information for VRF default
Router identifier 100.0.0.204, local AS number 65204
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
 * >      2000::202/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65202 i
 * >      2000::203/128          fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65203 i
 * >      2000::204/128          -                     -       -          -       0       i
 * >      2001::56/128           fe80::464c:a8ff:fe73:5c75%Et1 0       -          100     0       65000 65056 i
BGP routing table information for VRF tenant-a
Router identifier 100.0.1.204, local AS number 65204
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
 * >Ec    1000:1000:201::/64     2000::202             0       -          100     0       65000 65202 i
 *  ec    1000:1000:201::/64     2000::201             0       -          100     0       65000 65201 i
 * >      1000:1000:203::/64     -                     -       -          -       0       i
 *        1000:1000:203::/64     2000::203             0       -          100     0       65000 65203 i
 * >      1000:3000:1::/64       -                     -       -          -       0       i
 *  Ec    1000:3000:1::/64       2000::202             0       -          100     0       65000 65202 i
 *  ec    1000:3000:1::/64       2000::203             0       -          100     0       65000 65203 i
 *  ec    1000:3000:1::/64       2000::23              0       -          100     0       65000 65023 i
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
 *  Ec    1000:3000:2::/64       2000::202             0       -          100     0       65000 65202 i
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
 *  Ec    1000:3000:3::/64       2000::202             0       -          100     0       65000 65202 i
 *  ec    1000:3000:3::/64       2000::23              0       -          100     0       65000 65023 i
 *  ec    1000:3000:3::/64       2000::203             0       -          100     0       65000 65203 i
 *  ec    1000:3000:3::/64       2000::201             0       -          100     0       65000 65201 i
 *  ec    1000:3000:3::/64       2000::56              0       -          100     0       65000 65056 i
 *  ec    1000:3000:3::/64       2000::22              0       -          100     0       65000 65022 i
 * >      1000:3000:3::56/128    2000::56              0       -          100     0       65000 65056 i
 * >Ec    1000:3000:3::254/128   2000::23              0       -          100     0       65000 65023 i
 *  ec    1000:3000:3::254/128   2000::22              0       -          100     0       65000 65022 i
 * >      1000:3000:4::/64       -                     -       -          -       0       i
 *  Ec    1000:3000:4::/64       2000::202             0       -          100     0       65000 65202 i
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
 B E      2000::202/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 B E      2000::203/128 [20/0]
           via fe80::464c:a8ff:fe73:5c75, Ethernet1
 C        2000::204/128 [0/0]
           via Loopback0, directly connected
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
 B E      1000:1000:201::/64 [20/0]
           via VTEP 2000::202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
           via VTEP 2000::201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
 C        1000:1000:203::/64 [0/0]
           via Vlan1203, directly connected
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
Router identifier 100.0.0.204, local AS number 65204
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor                      LLDP Neighbor                  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
                           fe80::464c:a8ff:fe73:5c75%Et1 SPINE1-J-200.ns.eantc.de       4 65000            346       258    0    0 00:09:32 Estab   12     12
```

## show ipv6 neighbors vrf all

```text

VRF: default
IPv6 Address                                  Age Hardware Addr   Interface
fe80::464c:a8ff:fe73:5c75                 0:00:19 444c.a873.5c75  Et1

VRF: mgmt
IPv6 Address                                  Age Hardware Addr   Interface

VRF: tenant-a
IPv6 Address                                  Age Hardware Addr   Interface
1000:1000:203::203                        0:28:38 0020.3000.0005  Vl1203, not learned
fe80::220:30ff:fe00:5                     1:44:06 0020.3000.0005  Vl1203, not learned
fe80::2aa:aaff:feaa:aaaa                  3:04:40 00aa.aaaa.aaaa  Vl1203, Router
1000:3000:1::22                           0:29:58 0022.0000.0001  Vl1301, Vxlan1
1000:3000:1::42                                 - 0042.0100.0001  Vl1301, Vxlan1
1000:3000:1::45                                 - 0045.0100.0001  Vl1301, Vxlan1
1000:3000:1::203                          0:28:38 0020.3000.0001  Vl1301, not learned
1000:3000:1:0:242:1ff:fe00:1                    - 0042.0100.0001  Vl1301, Vxlan1
1000:3000:1:0:245:1ff:fe00:1                    - 0045.0100.0001  Vl1301, Vxlan1
fe80::220:30ff:fe00:1                     1:44:06 0020.3000.0001  Vl1301, not learned
fe80::222:ff:fe00:1                       1:33:50 0022.0000.0001  Vl1301, Vxlan1
fe80::240:1ff:fe00:1                      1:54:25 0040.0100.0001  Vl1301, not learned
fe80::242:1ff:fe00:1                      1:54:25 0042.0100.0001  Vl1301, Vxlan1
fe80::245:1ff:fe00:1                      1:44:06 0045.0100.0001  Vl1301, Vxlan1
fe80::2aa:aaff:feaa:aaaa                  3:04:38 00aa.aaaa.aaaa  Vl1301, Router
1000:3000:2::22                                 - 0022.0000.0002  Vl1302, Vxlan1
1000:3000:2::42                                 - 0042.0100.0002  Vl1302, Vxlan1
1000:3000:2::45                                 - 0045.0100.0002  Vl1302, Vxlan1
1000:3000:2::56                                 - 0056.0000.0002  Vl1302, Vxlan1
1000:3000:2:0:242:1ff:fe00:2                    - 0042.0100.0002  Vl1302, Vxlan1
1000:3000:2:0:245:1ff:fe00:2                    - 0045.0100.0002  Vl1302, Vxlan1
fe80::220:30ff:fe00:2                     1:44:06 0020.3000.0002  Vl1302, not learned
fe80::222:ff:fe00:2                       1:33:49 0022.0000.0002  Vl1302, Vxlan1
fe80::240:1ff:fe00:2                      1:54:25 0040.0100.0002  Vl1302, not learned
fe80::242:1ff:fe00:2                      1:54:26 0042.0100.0002  Vl1302, Vxlan1
fe80::245:1ff:fe00:2                      1:44:06 0045.0100.0002  Vl1302, Vxlan1
fe80::256:ff:fe00:2                       1:44:06 0056.0000.0002  Vl1302, Vxlan1
fe80::2aa:aaff:feaa:aaaa                  3:05:41 00aa.aaaa.aaaa  Vl1302, Router
1000:3000:3::22                           0:29:58 0022.0000.0003  Vl1303, Vxlan1
1000:3000:3::203                          0:28:38 0020.3000.0003  Vl1303, not learned
fe80::220:30ff:fe00:3                     1:44:06 0020.3000.0003  Vl1303, not learned
fe80::222:ff:fe00:3                       2:03:45 0022.0000.0003  Vl1303, Vxlan1
fe80::2aa:aaff:feaa:aaaa                  3:05:41 00aa.aaaa.aaaa  Vl1303, Router
1000:3000:4::22                           0:29:58 0022.0000.0004  Vl1304, Vxlan1
1000:3000:4::56                                 - 0056.0000.0004  Vl1304, Vxlan1
1000:3000:4::203                          0:28:38 0020.3000.0004  Vl1304, not learned
fe80::220:30ff:fe00:4                     1:44:06 0020.3000.0004  Vl1304, not learned
fe80::222:ff:fe00:4                       2:03:44 0022.0000.0004  Vl1304, Vxlan1
fe80::256:ff:fe00:4                       1:44:06 0056.0000.0004  Vl1304, Vxlan1
fe80::2aa:aaff:feaa:aaaa                  3:06:07 00aa.aaaa.aaaa  Vl1304, Router
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
   Ethernet1       fe80::464c:a8ff:fe73:5c75      0:00:51 ago   

```

## show ipv6 nd ra neighbors vrf tenant-a

```text
VRF: tenant-a
   Interface             IPv6 Address          Last RA Received
--------------- ------------------------------ ----------------
   Vlan1203        fe80::2aa:aaff:feaa:aaaa      0:01:25 ago   
   Vlan1301        fe80::2aa:aaff:feaa:aaaa      0:00:12 ago   
   Vlan1302        fe80::2aa:aaff:feaa:aaaa      0:00:03 ago   
   Vlan1303        fe80::2aa:aaff:feaa:aaaa      0:00:23 ago   
   Vlan1304        fe80::2aa:aaff:feaa:aaaa      0:01:41 ago   

```

## show interfaces counters rates | nz

```text
Port      Name       Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Et1       ANET 200    0:01      0.0   0.0%        0      0.0   0.0%        0
Ma1                   0:05      0.1   0.0%        0      0.2   0.0%        0
```

