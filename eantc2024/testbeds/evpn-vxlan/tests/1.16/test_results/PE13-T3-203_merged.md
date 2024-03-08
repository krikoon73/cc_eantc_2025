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
  ANET.IPV4                20.200.203.200 4 65000           1348      1317    0    0 18:36:53 Estab   27     27
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.203, local AS number 65203
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  ANET.EVPN                100.0.0.200 4 65000           2305      1382    0    0 18:36:53 Estab   249    249
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
BGP routing table entry for auto-discovery 0000:0000:0000:0000:0000, Route Distinguisher: 100.0.0.103:20
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1103:1103 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 Route-Target-AS:1304:1304 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
BGP routing table entry for auto-discovery 0 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 0 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.23:1022
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
BGP routing table entry for auto-discovery 0 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.23:1301
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.23:1302
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.23:1303
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.23:1304
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.23:1022
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.23:1301
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.23:1302
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.23:1303
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0023:0022, Route Distinguisher: 100.0.0.23:1304
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1203:1203 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
BGP routing table entry for mac-ip 0013.0100.0001, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0001, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0001 10.10.201.201, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1201 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0001 10.10.201.201, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb EvpnNdFlags:pflag
      VNI: 1201 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0002, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0002, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0002 10.30.1.201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0002 10.30.1.201, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0003, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0003, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0003 10.30.2.201, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0003 10.30.2.201, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb EvpnNdFlags:pflag
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0014.0100.0001, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0014.0100.0001 10.10.56.56, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0014.0100.0002, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0014.0100.0002 10.30.1.56, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0014.0100.0003, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0014.0100.0003 10.30.2.56, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0015.0100.0001, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0015.0100.0001 10.10.203.203, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0015.0100.0002, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0015.0100.0002 10.30.1.203, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0015.0100.0003, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0015.0100.0003 10.30.2.203, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0016.0100.0001, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan
      VNI: 1040 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0001 10.10.40.40, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1040 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0002, Route Distinguisher: 100.0.0.40:34068
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0002 10.30.1.40, Route Distinguisher: 100.0.0.40:34068
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0003, Route Distinguisher: 100.0.0.40:34069
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0003 10.30.2.40, Route Distinguisher: 100.0.0.40:34069
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0001, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan
      VNI: 1042 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0001 10.10.42.42, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1042 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0002, Route Distinguisher: 100.0.0.42:34068
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0002 10.30.1.42, Route Distinguisher: 100.0.0.42:34068
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0003, Route Distinguisher: 100.0.0.42:34069
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0003 10.30.2.42, Route Distinguisher: 100.0.0.42:34069
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0001, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0001, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0001 10.10.45.45, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0001 10.10.45.45, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0002, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0002, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0002 10.30.1.45, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0002 10.30.1.45, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0003, Route Distinguisher: 100.0.0.45:34069
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0003, Route Distinguisher: 100.0.0.46:34069
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0003 10.30.2.45, Route Distinguisher: 100.0.0.45:34069
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0003 10.30.2.45, Route Distinguisher: 100.0.0.46:34069
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0019.0100.0001, Route Distinguisher: 100.0.0.23:1022
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022 ESI: 0000:0000:0000:0023:0022
BGP routing table entry for mac-ip 0019.0100.0001 10.10.22.22, Route Distinguisher: 100.0.0.23:1022
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:77:7d
      VNI: 1022 L3 VNI: 1000 ESI: 0000:0000:0000:0023:0022
BGP routing table entry for mac-ip 0019.0100.0002, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0023:0022
BGP routing table entry for mac-ip 0019.0100.0002 10.30.1.22, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0023:0022
BGP routing table entry for mac-ip 0019.0100.0003, Route Distinguisher: 100.0.0.23:1302
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0023:0022
BGP routing table entry for mac-ip 0019.0100.0003 10.30.2.22, Route Distinguisher: 100.0.0.23:1302
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:77:7d
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0023:0022
BGP routing table entry for mac-ip 0022.2200.0001 10.10.10.103, Route Distinguisher: 0.0.0.0:1103
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1103:1103 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:02:00:00:01
      VNI: 1103 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0022.2200.0002 10.30.1.103, Route Distinguisher: 0.0.0.0:1301
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:02:00:00:01
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0022.2200.0003 10.30.2.103, Route Distinguisher: 0.0.0.0:1302
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:02:00:00:01
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0022.2200.0004 10.30.3.103, Route Distinguisher: 0.0.0.0:1303
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:02:00:00:01
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0022.2200.0005 10.30.4.103, Route Distinguisher: 0.0.0.0:1304
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1304:1304 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:02:00:00:01
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.10.56.253, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.30.1.254, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.30.2.254, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.56.254, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.2.254, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.201.202, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1201 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.201.202, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb EvpnNdFlags:pflag
      VNI: 1201 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.30.1.202, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.30.1.202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.30.2.202, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.30.2.202, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb EvpnNdFlags:pflag
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 5c5a.c773.4abb, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan
      VNI: 1040 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan
      VNI: 1042 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb 10.10.40.25, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1040 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb 10.10.42.25, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1042 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb 10.10.45.25, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb 10.10.45.25, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 0013.0100.0004, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0013.0100.0004, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0013.0100.0004 10.30.3.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0013.0100.0004 10.30.3.201, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0014.0100.0004, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 0014.0100.0004 10.30.3.56, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 0015.0100.0004, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0015.0100.0004 10.30.3.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0019.0100.0004, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0023:0022
BGP routing table entry for mac-ip 1303 0019.0100.0004 10.30.3.22, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0023:0022
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 444c.a873.5c75, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 444c.a873.5c75 10.30.3.202, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 444c.a873.5c75 10.30.3.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0013.0100.0005, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0013.0100.0005, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0013.0100.0005 10.30.4.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0013.0100.0005 10.30.4.201, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0014.0100.0005, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 0014.0100.0005 10.30.4.56, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 0015.0100.0005, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 0015.0100.0005 10.30.4.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 0019.0100.0005, Route Distinguisher: 100.0.0.23:1304
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0023:0022
BGP routing table entry for mac-ip 1304 0019.0100.0005 10.30.4.22, Route Distinguisher: 100.0.0.23:1304
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:77:7d
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0023:0022
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 444c.a873.5c75, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 444c.a873.5c75 10.30.4.202, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 444c.a873.5c75 10.30.4.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
```

## show bgp evpn route-type imet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
      PMSI Tunnel: Ingress Replication, MPLS Label: 1022, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.23, Route Distinguisher: 100.0.0.23:1022
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
      PMSI Tunnel: Ingress Replication, MPLS Label: 1022, Leaf Information Required: false, Tunnel ID: 100.0.0.23
BGP routing table entry for imet 100.0.0.23, Route Distinguisher: 100.0.0.23:1301
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.23
BGP routing table entry for imet 100.0.0.23, Route Distinguisher: 100.0.0.23:1302
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.23
BGP routing table entry for imet 100.0.0.40, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan
      VNI: 1040
      PMSI Tunnel: Ingress Replication, MPLS Label: 1040, Leaf Information Required: false, Tunnel ID: 100.0.0.40
BGP routing table entry for imet 100.0.0.40, Route Distinguisher: 100.0.0.40:34068
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.40
BGP routing table entry for imet 100.0.0.40, Route Distinguisher: 100.0.0.40:34069
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.40
BGP routing table entry for imet 100.0.0.40, Route Distinguisher: 100.0.0.40:34070
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.40
BGP routing table entry for imet 100.0.0.40, Route Distinguisher: 100.0.0.40:34071
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1304:1304 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.40
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan
      VNI: 1045
      PMSI Tunnel: Ingress Replication, MPLS Label: 1045, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.45:34069
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan
      VNI: 1045
      PMSI Tunnel: Ingress Replication, MPLS Label: 1045, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.46:34069
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.42, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan
      VNI: 1042
      PMSI Tunnel: Ingress Replication, MPLS Label: 1042, Leaf Information Required: false, Tunnel ID: 100.0.0.42
BGP routing table entry for imet 100.0.0.42, Route Distinguisher: 100.0.0.42:34068
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.42
BGP routing table entry for imet 100.0.0.42, Route Distinguisher: 100.0.0.42:34069
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.42
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan
      VNI: 1056
      PMSI Tunnel: Ingress Replication, MPLS Label: 1056, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.103, Route Distinguisher: 0.0.0.0:1103
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1103:1103 TunnelEncap:tunnelTypeVxlan
      VNI: 0
      PMSI Tunnel: Ingress Replication, MPLS Label: 0, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 100.0.0.103, Route Distinguisher: 0.0.0.0:1301
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 0
      PMSI Tunnel: Ingress Replication, MPLS Label: 0, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 100.0.0.103, Route Distinguisher: 0.0.0.0:1302
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 0
      PMSI Tunnel: Ingress Replication, MPLS Label: 0, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 100.0.0.103, Route Distinguisher: 0.0.0.0:1303
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 0
      PMSI Tunnel: Ingress Replication, MPLS Label: 0, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 100.0.0.103, Route Distinguisher: 0.0.0.0:1304
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1304:1304 TunnelEncap:tunnelTypeVxlan
      VNI: 0
      PMSI Tunnel: Ingress Replication, MPLS Label: 0, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan Multicast Flags: IGMP proxy, OISM-supported, SBD
      VNI: 1000
      PMSI Tunnel: Ingress Replication, MPLS Label: 1000, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
      PMSI Tunnel: Ingress Replication, MPLS Label: 1201, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.202, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan Multicast Flags: IGMP proxy, OISM-supported, SBD
      VNI: 1000
      PMSI Tunnel: Ingress Replication, MPLS Label: 1000, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 100.0.0.202, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
      PMSI Tunnel: Ingress Replication, MPLS Label: 1201, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 100.0.0.202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 100.0.0.202, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 100.0.0.203, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan Multicast Flags: IGMP proxy, OISM-supported, SBD
      VNI: 1000
      PMSI Tunnel: Ingress Replication, MPLS Label: 1000, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 100.0.0.203, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
      PMSI Tunnel: Ingress Replication, MPLS Label: 1203, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 100.0.0.203, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 100.0.0.203, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 100.0.0.204, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan Multicast Flags: IGMP proxy, OISM-supported, SBD
      VNI: 1000
      PMSI Tunnel: Ingress Replication, MPLS Label: 1000, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 100.0.0.204, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 100.0.0.204, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 1303 100.0.0.22, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 1303 100.0.0.23, Route Distinguisher: 100.0.0.23:1303
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.23
BGP routing table entry for imet 1303 100.0.0.56, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1303 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1303 100.0.0.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1303 100.0.0.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 1303 100.0.0.204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 1304 100.0.0.22, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 1304 100.0.0.23, Route Distinguisher: 100.0.0.23:1304
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.23
BGP routing table entry for imet 1304 100.0.0.56, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1304 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1304 100.0.0.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1304 100.0.0.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 1304 100.0.0.204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.204
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
BGP routing table entry for ethernet-segment 0000:0000:0000:0000:0000 100.0.0.103, Route Distinguisher: 100.0.0.103:1
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:00:00:00:00
BGP routing table entry for ethernet-segment 0000:0000:0000:0023:0022 100.0.0.22, Route Distinguisher: 100.0.0.22:0
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: EvpnEsImportRt:00:00:00:00:00:00 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0023:0022 100.0.0.23, Route Distinguisher: 100.0.0.23:0
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: EvpnEsImportRt:00:00:00:00:00:00 DF Election: Preference 100
BGP routing table entry for ethernet-segment 0000:0000:0000:0201:0202 100.0.0.201, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:10:02:02 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0201:0202 100.0.0.202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:10:02:02 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0203:0204 100.0.0.203, Route Distinguisher: 100.0.0.203:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:30:02:04 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0048:5648:5648:5648:5648 100.0.0.56, Route Distinguisher: 100.0.0.56:0
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: EvpnEsImportRt:48:56:48:56:48:56
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
BGP routing table entry for ip-prefix 10.10.22.0/24, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.22.0/24, Route Distinguisher: 100.0.0.23:1000
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:77:7d
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.22.254/32, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.22.254/32, Route Distinguisher: 100.0.0.23:1000
 Paths: 1 available
  65000 65023
    100.0.0.23 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:77:7d
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.40.0/24, Route Distinguisher: 100.0.0.40:1000
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.42.0/24, Route Distinguisher: 100.0.0.42:1000
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.45.0/24, Route Distinguisher: 100.0.0.45:4
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.45.0/24, Route Distinguisher: 100.0.0.46:4
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.56.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.56.56/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.40:1000
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.42:1000
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.45:4
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.46:4
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.56/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.40:1000
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.42:1000
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.45:4
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.46:4
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.56/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.40:1000
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.56/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.40:1000
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.56/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 100.0.1.201/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1000
BGP routing table entry for ip-prefix 100.0.1.202/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:74:83:ef:0b:a4:fb
      VNI: 1000
BGP routing table entry for ip-prefix 100.0.1.203/32, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 100.0.1.204/32, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
```

## show bgp evpn route-type smet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.203, local AS number 65203
```

## show ip route

```text

VRF: default
Codes: C - connected, S - static, K - kernel, 
       O - OSPF, IA - OSPF inter area, E1 - OSPF external type 1,
       E2 - OSPF external type 2, N1 - OSPF NSSA external type 1,
       N2 - OSPF NSSA external type2, B - Other BGP Routes,
       B I - iBGP, B E - eBGP, R - RIP, I L1 - IS-IS level 1,
       I L2 - IS-IS level 2, O3 - OSPFv3, A B - BGP Aggregate,
       A O - OSPF Summary, NG - Nexthop Group Static Route,
       V - VXLAN Control Service, M - Martian,
       DH - DHCP client installed default route,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route

Gateway of last resort is not set

 B E      20.22.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.23.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.40.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.42.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.44.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.45.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.46.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.56.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.103.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.200.201.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.200.202.0/24 [20/0] via 20.200.203.200, Ethernet1
 C        20.200.203.0/24 is directly connected, Ethernet1
 B E      20.200.204.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.22/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.23/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.40/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.41/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.42/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.44/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.45/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.46/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.56/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.103/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.200/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.201/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.202/32 [20/0] via 20.200.203.200, Ethernet1
 C        100.0.0.203/32 is directly connected, Loopback0
 B E      100.0.0.204/32 [20/0] via 20.200.203.200, Ethernet1

```

## show ip arp

```text
Address         Age (sec)  Hardware Addr   Interface
20.200.203.200    0:00:44  444c.a873.5c75  Ethernet1
```

## show ip route vrf all

```text

VRF: default
Codes: C - connected, S - static, K - kernel, 
       O - OSPF, IA - OSPF inter area, E1 - OSPF external type 1,
       E2 - OSPF external type 2, N1 - OSPF NSSA external type 1,
       N2 - OSPF NSSA external type2, B - Other BGP Routes,
       B I - iBGP, B E - eBGP, R - RIP, I L1 - IS-IS level 1,
       I L2 - IS-IS level 2, O3 - OSPFv3, A B - BGP Aggregate,
       A O - OSPF Summary, NG - Nexthop Group Static Route,
       V - VXLAN Control Service, M - Martian,
       DH - DHCP client installed default route,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route

Gateway of last resort is not set

 B E      20.22.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.23.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.40.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.42.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.44.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.45.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.46.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.56.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.103.200.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.200.201.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      20.200.202.0/24 [20/0] via 20.200.203.200, Ethernet1
 C        20.200.203.0/24 is directly connected, Ethernet1
 B E      20.200.204.0/24 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.22/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.23/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.40/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.41/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.42/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.44/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.45/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.46/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.56/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.103/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.200/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.201/32 [20/0] via 20.200.203.200, Ethernet1
 B E      100.0.0.202/32 [20/0] via 20.200.203.200, Ethernet1
 C        100.0.0.203/32 is directly connected, Loopback0
 B E      100.0.0.204/32 [20/0] via 20.200.203.200, Ethernet1


VRF: mgmt
Codes: C - connected, S - static, K - kernel, 
       O - OSPF, IA - OSPF inter area, E1 - OSPF external type 1,
       E2 - OSPF external type 2, N1 - OSPF NSSA external type 1,
       N2 - OSPF NSSA external type2, B - Other BGP Routes,
       B I - iBGP, B E - eBGP, R - RIP, I L1 - IS-IS level 1,
       I L2 - IS-IS level 2, O3 - OSPFv3, A B - BGP Aggregate,
       A O - OSPF Summary, NG - Nexthop Group Static Route,
       V - VXLAN Control Service, M - Martian,
       DH - DHCP client installed default route,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route

Gateway of last resort:
 S        0.0.0.0/0 [1/0] via 192.168.20.1, Management1

 C        192.168.20.0/23 is directly connected, Management1


VRF: tenant-a
Codes: C - connected, S - static, K - kernel, 
       O - OSPF, IA - OSPF inter area, E1 - OSPF external type 1,
       E2 - OSPF external type 2, N1 - OSPF NSSA external type 1,
       N2 - OSPF NSSA external type2, B - Other BGP Routes,
       B I - iBGP, B E - eBGP, R - RIP, I L1 - IS-IS level 1,
       I L2 - IS-IS level 2, O3 - OSPFv3, A B - BGP Aggregate,
       A O - OSPF Summary, NG - Nexthop Group Static Route,
       V - VXLAN Control Service, M - Martian,
       DH - DHCP client installed default route,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route

Gateway of last resort is not set

 B E      10.10.10.103/32 [20/0] via VTEP 100.0.0.103 VNI 1000 router-mac 00:01:02:00:00:01
 B E      10.10.22.22/32 [20/0] via VTEP 100.0.0.23 VNI 1000 router-mac c4:07:78:0a:77:7d
 B E      10.10.22.254/32 [20/0] via VTEP 100.0.0.23 VNI 1000 router-mac c4:07:78:0a:77:7d
                                 via VTEP 100.0.0.22 VNI 1000 router-mac c4:07:78:0a:9f:31
 B E      10.10.22.0/24 [20/0] via VTEP 100.0.0.23 VNI 1000 router-mac c4:07:78:0a:77:7d
                               via VTEP 100.0.0.22 VNI 1000 router-mac c4:07:78:0a:9f:31
 B E      10.10.40.25/32 [20/0] via VTEP 100.0.0.40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      10.10.40.40/32 [20/0] via VTEP 100.0.0.40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      10.10.40.0/24 [20/0] via VTEP 100.0.0.40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      10.10.42.25/32 [20/0] via VTEP 100.0.0.42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      10.10.42.42/32 [20/0] via VTEP 100.0.0.42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      10.10.42.0/24 [20/0] via VTEP 100.0.0.42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      10.10.45.25/32 [20/0] via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:7b:8b:87
                                via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:b7:50:5f
 B E      10.10.45.45/32 [20/0] via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:7b:8b:87
                                via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:b7:50:5f
 B E      10.10.45.0/24 [20/0] via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:7b:8b:87
                               via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:b7:50:5f
 B E      10.10.56.56/32 [20/0] via VTEP 100.0.0.56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      10.10.56.0/24 [20/0] via VTEP 100.0.0.56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      10.10.201.201/32 [20/0] via VTEP 100.0.0.201 VNI 1000 router-mac 28:99:3a:8f:8f:6f
                                  via VTEP 100.0.0.202 VNI 1000 router-mac 74:83:ef:0b:a4:fb
 B E      10.10.201.202/32 [20/0] via VTEP 100.0.0.201 VNI 1000 router-mac 28:99:3a:8f:8f:6f
                                  via VTEP 100.0.0.202 VNI 1000 router-mac 74:83:ef:0b:a4:fb
 B E      10.10.201.0/24 [20/0] via VTEP 100.0.0.201 VNI 1000 router-mac 28:99:3a:8f:8f:6f
                                via VTEP 100.0.0.202 VNI 1000 router-mac 74:83:ef:0b:a4:fb
 C        10.10.203.0/24 is directly connected, Vlan1203
 B E      10.30.1.22/32 [20/0] via VTEP 100.0.0.22 VNI 1000 router-mac c4:07:78:0a:9f:31
 B E      10.30.1.40/32 [20/0] via VTEP 100.0.0.40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      10.30.1.42/32 [20/0] via VTEP 100.0.0.42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      10.30.1.45/32 [20/0] via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:7b:8b:87
                               via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:b7:50:5f
 B E      10.30.1.56/32 [20/0] via VTEP 100.0.0.56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      10.30.1.103/32 [20/0] via VTEP 100.0.0.103 VNI 1000 router-mac 00:01:02:00:00:01
 B E      10.30.1.201/32 [20/0] via VTEP 100.0.0.201 VNI 1000 router-mac 28:99:3a:8f:8f:6f
                                via VTEP 100.0.0.202 VNI 1000 router-mac 74:83:ef:0b:a4:fb
 B E      10.30.1.202/32 [20/0] via VTEP 100.0.0.201 VNI 1000 router-mac 28:99:3a:8f:8f:6f
                                via VTEP 100.0.0.202 VNI 1000 router-mac 74:83:ef:0b:a4:fb
 C        10.30.1.0/24 is directly connected, Vlan1301
 B E      10.30.2.22/32 [20/0] via VTEP 100.0.0.23 VNI 1000 router-mac c4:07:78:0a:77:7d
 B E      10.30.2.40/32 [20/0] via VTEP 100.0.0.40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      10.30.2.42/32 [20/0] via VTEP 100.0.0.42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      10.30.2.45/32 [20/0] via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:7b:8b:87
                               via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:b7:50:5f
 B E      10.30.2.56/32 [20/0] via VTEP 100.0.0.56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      10.30.2.103/32 [20/0] via VTEP 100.0.0.103 VNI 1000 router-mac 00:01:02:00:00:01
 B E      10.30.2.201/32 [20/0] via VTEP 100.0.0.201 VNI 1000 router-mac 28:99:3a:8f:8f:6f
                                via VTEP 100.0.0.202 VNI 1000 router-mac 74:83:ef:0b:a4:fb
 B E      10.30.2.202/32 [20/0] via VTEP 100.0.0.201 VNI 1000 router-mac 28:99:3a:8f:8f:6f
                                via VTEP 100.0.0.202 VNI 1000 router-mac 74:83:ef:0b:a4:fb
 C        10.30.2.0/24 is directly connected, Vlan1302
 B E      10.30.3.22/32 [20/0] via VTEP 100.0.0.22 VNI 1000 router-mac c4:07:78:0a:9f:31
 B E      10.30.3.56/32 [20/0] via VTEP 100.0.0.56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      10.30.3.103/32 [20/0] via VTEP 100.0.0.103 VNI 1000 router-mac 00:01:02:00:00:01
 B E      10.30.3.201/32 [20/0] via VTEP 100.0.0.201 VNI 1000 router-mac 28:99:3a:8f:8f:6f
                                via VTEP 100.0.0.202 VNI 1000 router-mac 74:83:ef:0b:a4:fb
 B E      10.30.3.202/32 [20/0] via VTEP 100.0.0.201 VNI 1000 router-mac 28:99:3a:8f:8f:6f
                                via VTEP 100.0.0.202 VNI 1000 router-mac 74:83:ef:0b:a4:fb
 C        10.30.3.0/24 is directly connected, Vlan1303
 B E      10.30.4.22/32 [20/0] via VTEP 100.0.0.23 VNI 1000 router-mac c4:07:78:0a:77:7d
 B E      10.30.4.56/32 [20/0] via VTEP 100.0.0.56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      10.30.4.103/32 [20/0] via VTEP 100.0.0.103 VNI 1000 router-mac 00:01:02:00:00:01
 B E      10.30.4.201/32 [20/0] via VTEP 100.0.0.201 VNI 1000 router-mac 28:99:3a:8f:8f:6f
                                via VTEP 100.0.0.202 VNI 1000 router-mac 74:83:ef:0b:a4:fb
 B E      10.30.4.202/32 [20/0] via VTEP 100.0.0.201 VNI 1000 router-mac 28:99:3a:8f:8f:6f
                                via VTEP 100.0.0.202 VNI 1000 router-mac 74:83:ef:0b:a4:fb
 C        10.30.4.0/24 is directly connected, Vlan1304
 B E      100.0.1.201/32 [20/0] via VTEP 100.0.0.201 VNI 1000 router-mac 28:99:3a:8f:8f:6f
 B E      100.0.1.202/32 [20/0] via VTEP 100.0.0.202 VNI 1000 router-mac 74:83:ef:0b:a4:fb
 C        100.0.1.203/32 is directly connected, Loopback100
 B E      100.0.1.204/32 [20/0] via VTEP 100.0.0.204 VNI 1000 router-mac 98:5d:82:a2:04:f9

```

## show ip arp vrf all

```text

VRF: default
Address         Age (sec)  Hardware Addr   Interface
20.200.203.200    0:00:44  444c.a873.5c75  Ethernet1

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.20.2      0:02:21  bcea.fa02.6ce2  Management1
192.168.20.18     0:02:45  e484.29cd.e801  Management1
192.168.20.19     0:02:51  c407.7858.8001  Management1
192.168.20.20     0:02:33  e484.29d0.4001  Management1
192.168.20.21     0:01:15  7081.85c1.b801  Management1
192.168.20.22     0:00:57  c407.780a.9f04  Management1
192.168.20.23     0:02:51  c407.780a.7750  Management1
192.168.20.24     0:04:21  6c87.2089.ede5  Management1
192.168.20.25     0:00:57  6c87.2089.ece5  Management1
192.168.20.26     0:04:09  04a9.59d5.df66  Management1
192.168.20.28     0:00:39  98a9.2d59.bae6  Management1
192.168.20.52     0:04:27  f83e.95dc.1289  Management1
192.168.20.204    0:02:33  985d.82a2.04f8  Management1
192.168.21.50     0:04:39  a84f.b1a5.5221  Management1
192.168.21.59     0:02:33  6607.f5d1.ae16  Management1

VRF: tenant-a
Address         Age (sec)  Hardware Addr   Interface
10.10.203.203     0:18:56  0015.0100.0001  Vlan1203, Port-Channel200
10.10.203.204     0:53:48  444c.a873.5c75  Vlan1203, not learned
10.30.1.22              -  0019.0100.0002  Vlan1301, Vxlan1
10.30.1.40              -  0016.0100.0002  Vlan1301, Vxlan1
10.30.1.42              -  0017.0100.0002  Vlan1301, Vxlan1
10.30.1.45              -  0018.0100.0002  Vlan1301, Vxlan1
10.30.1.56              -  0014.0100.0002  Vlan1301, Vxlan1
10.30.1.103             -  0022.2200.0002  Vlan1301, Vxlan1
10.30.1.201             -  0013.0100.0002  Vlan1301, Vxlan1
10.30.1.202             -  444c.a873.5c75  Vlan1301, Vxlan1
10.30.1.203       0:18:56  0015.0100.0002  Vlan1301, Port-Channel200
10.30.2.22              -  0019.0100.0003  Vlan1302, Vxlan1
10.30.2.40              -  0016.0100.0003  Vlan1302, Vxlan1
10.30.2.42              -  0017.0100.0003  Vlan1302, Vxlan1
10.30.2.45              -  0018.0100.0003  Vlan1302, Vxlan1
10.30.2.56              -  0014.0100.0003  Vlan1302, Vxlan1
10.30.2.103             -  0022.2200.0003  Vlan1302, Vxlan1
10.30.2.201             -  0013.0100.0003  Vlan1302, Vxlan1
10.30.2.202             -  444c.a873.5c75  Vlan1302, Vxlan1
10.30.2.203       0:18:56  0015.0100.0003  Vlan1302, Port-Channel200
10.30.3.22              -  0019.0100.0004  Vlan1303, Vxlan1
10.30.3.56              -  0014.0100.0004  Vlan1303, Vxlan1
10.30.3.201             -  0013.0100.0004  Vlan1303, Vxlan1
10.30.3.202             -  444c.a873.5c75  Vlan1303, Vxlan1
10.30.3.203       0:18:56  0015.0100.0004  Vlan1303, Port-Channel200
10.30.4.22              -  0019.0100.0005  Vlan1304, Vxlan1
10.30.4.56              -  0014.0100.0005  Vlan1304, Vxlan1
10.30.4.201             -  0013.0100.0005  Vlan1304, Vxlan1
10.30.4.202             -  444c.a873.5c75  Vlan1304, Vxlan1
10.30.4.203       0:18:56  0015.0100.0005  Vlan1304, Port-Channel200
```

## show vxlan address-table

```text
          Vxlan Mac Address Table
----------------------------------------------------------------------

VLAN  Mac Address     Type      Prt  VTEP             Moves   Last Move
----  -----------     ----      ---  ----             -----   ---------
1301  0013.0100.0002  EVPN      Vx1  100.0.0.201      1       1:00:26 ago
                                     100.0.0.202    
1301  0014.0100.0002  EVPN      Vx1  100.0.0.56       1       1:00:21 ago
1301  0016.0100.0002  EVPN      Vx1  100.0.0.40       1       18:36:04 ago
1301  0017.0100.0002  EVPN      Vx1  100.0.0.42       1       18:35:46 ago
1301  0018.0100.0002  EVPN      Vx1  100.0.0.41       1       18:36:19 ago
1301  0019.0100.0002  EVPN      Vx1  100.0.0.22       2       1:39:34 ago
                                     100.0.0.23     
1301  0022.2200.0002  EVPN      Vx1  100.0.0.103      1       0:18:48 ago
1301  0056.5656.5656  EVPN      Vx1  100.0.0.56       1       18:35:11 ago
1301  444c.a873.5c75  EVPN      Vx1  100.0.0.201      1       0:00:27 ago
                                     100.0.0.202    
1302  0013.0100.0003  EVPN      Vx1  100.0.0.201      1       1:00:26 ago
                                     100.0.0.202    
1302  0014.0100.0003  EVPN      Vx1  100.0.0.56       1       1:00:21 ago
1302  0016.0100.0003  EVPN      Vx1  100.0.0.40       1       18:36:04 ago
1302  0017.0100.0003  EVPN      Vx1  100.0.0.42       1       18:35:46 ago
1302  0018.0100.0003  EVPN      Vx1  100.0.0.41       1       18:36:19 ago
1302  0019.0100.0003  EVPN      Vx1  100.0.0.22       1       1:39:34 ago
                                     100.0.0.23     
1302  0022.2200.0003  EVPN      Vx1  100.0.0.103      1       0:18:48 ago
1302  0056.5656.5656  EVPN      Vx1  100.0.0.56       1       18:35:11 ago
1302  444c.a873.5c75  EVPN      Vx1  100.0.0.201      1       0:01:53 ago
                                     100.0.0.202    
1303  0013.0100.0004  EVPN      Vx1  100.0.0.201      1       1:00:26 ago
                                     100.0.0.202    
1303  0014.0100.0004  EVPN      Vx1  100.0.0.56       1       1:00:21 ago
1303  0019.0100.0004  EVPN      Vx1  100.0.0.22       1       18:36:31 ago
                                     100.0.0.23     
1303  0056.5656.5656  EVPN      Vx1  100.0.0.56       1       18:35:11 ago
1303  444c.a873.5c75  EVPN      Vx1  100.0.0.201      1       0:01:53 ago
                                     100.0.0.202    
1304  0013.0100.0005  EVPN      Vx1  100.0.0.201      1       1:00:26 ago
                                     100.0.0.202    
1304  0014.0100.0005  EVPN      Vx1  100.0.0.56       1       1:00:21 ago
1304  0019.0100.0005  EVPN      Vx1  100.0.0.22       1       0:37:52 ago
                                     100.0.0.23     
1304  0056.5656.5656  EVPN      Vx1  100.0.0.56       1       18:35:11 ago
1304  444c.a873.5c75  EVPN      Vx1  100.0.0.201      1       0:00:27 ago
                                     100.0.0.202    
4094  0001.0000.0056  EVPN      Vx1  100.0.0.56               18:35:11 ago
4094  0001.0200.0001  EVPN      Vx1  100.0.0.103              0:18:48 ago
4094  246c.8474.8ddb  EVPN      Vx1  100.0.0.40               18:36:04 ago
4094  2899.3a8f.8f6f  EVPN      Vx1  100.0.0.201              18:36:50 ago
4094  4014.827b.84ab  EVPN      Vx1  100.0.0.42               18:35:46 ago
4094  6c31.0e7b.8b87  EVPN      Vx1  100.0.0.41               18:36:19 ago
4094  6c31.0eb7.505f  EVPN      Vx1  100.0.0.41               18:35:41 ago
4094  7483.ef0b.a4fb  EVPN      Vx1  100.0.0.202              18:34:58 ago
4094  985d.82a2.04f9  EVPN      Vx1  100.0.0.204              18:36:50 ago
4094  c407.780a.777d  EVPN      Vx1  100.0.0.23               18:36:35 ago
4094  c407.780a.9f31  EVPN      Vx1  100.0.0.22               18:36:31 ago
Total Remote Mac Addresses for this criterion: 39
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
---------- ---------- -------------- -------------------- 
1000       4094       tenant-a       evpn                 
1201       4094       tenant-a       evpn multicast       
1301       4094       tenant-a       evpn multicast       
1302       4094       tenant-a       evpn multicast       
1303       4094       tenant-a       evpn multicast       
1304       4094       tenant-a       evpn multicast       

```

## show mac address-table

```text
          Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports      Moves   Last Move
----    -----------       ----        -----      -----   ---------
1203    0015.0100.0001    DYNAMIC     Po200      1       2:22:14 ago
1203    00aa.aaaa.aaaa    STATIC      Router
1301    0013.0100.0002    DYNAMIC     Vx1        1       1:00:26 ago
1301    0014.0100.0002    DYNAMIC     Vx1        1       1:00:21 ago
1301    0015.0100.0002    DYNAMIC     Po200      1       2:22:14 ago
1301    0016.0100.0002    DYNAMIC     Vx1        1       18:36:05 ago
1301    0017.0100.0002    DYNAMIC     Vx1        1       18:35:46 ago
1301    0018.0100.0002    DYNAMIC     Vx1        1       18:36:19 ago
1301    0019.0100.0002    DYNAMIC     Vx1        2       1:39:34 ago
1301    0022.2200.0002    DYNAMIC     Vx1        1       0:18:48 ago
1301    0056.5656.5656    STATIC      Vx1
1301    00aa.aaaa.aaaa    STATIC      Router
1301    444c.a873.5c75    DYNAMIC     Vx1        1       0:00:27 ago
1302    0013.0100.0003    DYNAMIC     Vx1        1       1:00:27 ago
1302    0014.0100.0003    DYNAMIC     Vx1        1       1:00:21 ago
1302    0015.0100.0003    DYNAMIC     Po200      1       2:22:14 ago
1302    0016.0100.0003    DYNAMIC     Vx1        1       18:36:05 ago
1302    0017.0100.0003    DYNAMIC     Vx1        1       18:35:46 ago
1302    0018.0100.0003    DYNAMIC     Vx1        1       18:36:19 ago
1302    0019.0100.0003    DYNAMIC     Vx1        1       1:39:34 ago
1302    0022.2200.0003    DYNAMIC     Vx1        1       0:18:48 ago
1302    0056.5656.5656    STATIC      Vx1
1302    00aa.aaaa.aaaa    STATIC      Router
1302    444c.a873.5c75    DYNAMIC     Vx1        1       0:01:53 ago
1303    0013.0100.0004    DYNAMIC     Vx1        1       1:00:27 ago
1303    0014.0100.0004    DYNAMIC     Vx1        1       1:00:21 ago
1303    0015.0100.0004    DYNAMIC     Po200      1       2:22:14 ago
1303    0019.0100.0004    DYNAMIC     Vx1        1       18:36:32 ago
1303    0056.5656.5656    STATIC      Vx1
1303    00aa.aaaa.aaaa    STATIC      Router
1303    444c.a873.5c75    DYNAMIC     Vx1        1       0:01:53 ago
1304    0013.0100.0005    DYNAMIC     Vx1        1       1:00:27 ago
1304    0014.0100.0005    DYNAMIC     Vx1        1       1:00:21 ago
1304    0015.0100.0005    DYNAMIC     Po200      1       2:22:14 ago
1304    0019.0100.0005    DYNAMIC     Vx1        1       0:37:52 ago
1304    0056.5656.5656    STATIC      Vx1
1304    00aa.aaaa.aaaa    STATIC      Router
1304    444c.a873.5c75    DYNAMIC     Vx1        1       0:00:27 ago
4094    0001.0000.0056    DYNAMIC     Vx1        0       18:35:11 ago
4094    0001.0200.0001    DYNAMIC     Vx1        0       0:18:48 ago
4094    00aa.aaaa.aaaa    STATIC      Router
4094    246c.8474.8ddb    DYNAMIC     Vx1        0       18:36:05 ago
4094    2899.3a8f.8f6f    DYNAMIC     Vx1        0       18:36:51 ago
4094    4014.827b.84ab    DYNAMIC     Vx1        0       18:35:46 ago
4094    6c31.0e7b.8b87    DYNAMIC     Vx1        0       18:36:19 ago
4094    6c31.0eb7.505f    DYNAMIC     Vx1        0       18:35:41 ago
4094    7483.ef0b.a4fb    DYNAMIC     Vx1        0       18:34:58 ago
4094    985d.82a2.04f9    DYNAMIC     Vx1        0       18:36:51 ago
4094    c407.780a.777d    DYNAMIC     Vx1        0       18:36:35 ago
4094    c407.780a.9f31    DYNAMIC     Vx1        0       18:36:32 ago
Total Mac Addresses for this criterion: 50

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
0019.0100.0003, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 2: 2-way
      VTEP 100.0.0.22
      VTEP 100.0.0.23
00aa.aaaa.aaaa, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
0015.0100.0002, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0017.0100.0002, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.42
0056.5656.5656, VLAN 1303, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
444c.a873.5c75, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 10: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
0019.0100.0005, VLAN 1304, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 2: 2-way
      VTEP 100.0.0.22
      VTEP 100.0.0.23
0018.0100.0002, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.41
0018.0100.0003, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.41
00aa.aaaa.aaaa, VLAN 1303, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
0022.2200.0002, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.103
0016.0100.0002, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.40
444c.a873.5c75, VLAN 1304, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 10: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
0013.0100.0004, VLAN 1303, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 10: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
0013.0100.0003, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 10: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
0056.5656.5656, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
0016.0100.0003, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.40
0015.0100.0001, VLAN 1203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0015.0100.0004, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0014.0100.0005, VLAN 1304, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.56
0019.0100.0004, VLAN 1303, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 2: 2-way
      VTEP 100.0.0.22
      VTEP 100.0.0.23
0056.5656.5656, VLAN 1302, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
444c.a873.5c75, VLAN 1303, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 10: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
00aa.aaaa.aaaa, VLAN 1304, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
0014.0100.0002, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.56
0017.0100.0003, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.42
00aa.aaaa.aaaa, VLAN 1302, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
0014.0100.0003, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.56
0013.0100.0005, VLAN 1304, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 10: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
0014.0100.0004, VLAN 1303, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.56
0056.5656.5656, VLAN 1304, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
0022.2200.0003, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.103
0013.0100.0002, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 10: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
0019.0100.0002, VLAN 1301, seq 2, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 2: 2-way
      VTEP 100.0.0.22
      VTEP 100.0.0.23
444c.a873.5c75, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 10: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
0015.0100.0003, VLAN 1302, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
0015.0100.0005, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
```

## show vxlan flood vtep domain local

```text
          VXLAN Flood VTEP Table
--------------------------------------------------------------------------------

VLANS                            Ip Address
-----------------------------   ------------------------------------------------
1301-1302                       100.0.0.22      100.0.0.23      100.0.0.40     
                                100.0.0.41      100.0.0.42      100.0.0.56     
                                100.0.0.103     100.0.0.201     100.0.0.202    
                                100.0.0.204    
1303-1304                       100.0.0.22      100.0.0.23      100.0.0.56     
                                100.0.0.201     100.0.0.202     100.0.0.204    
4094                            100.0.0.201     100.0.0.202     100.0.0.204    
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
      Designated forwarder: 100.0.0.203
EVPN instance: VLAN 1301
  Route distinguisher: 100.0.0.203:1301
  Route target import: Route-Target-AS:1301:1301
  Route target export: Route-Target-AS:1301:1301
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
      Designated forwarder: 100.0.0.203
EVPN instance: VLAN 1302
  Route distinguisher: 100.0.0.203:1302
  Route target import: Route-Target-AS:1302:1302
  Route target export: Route-Target-AS:1302:1302
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
      Designated forwarder: 100.0.0.203
EVPN instance: VLAN-aware bundle 1303-1304
  Route distinguisher: 100.0.0.203:1303
  Route target import: Route-Target-AS:1303:1303
  Route target export: Route-Target-AS:1303:1303
  Service interface: VLAN-aware bundle
  Local VXLAN IP address: 100.0.0.203
  VXLAN: enabled
  MPLS: disabled
  Local ethernet segment:
    ESI: 0000:0000:0000:0203:0204
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:30:02:04
      Designated forwarder: 100.0.0.203
```

## show interfaces counters rates | nz

```text
Port      Name        Intvl   In Mbps      %  In Kpps  Out Mbps      % Out Kpps
Et1       A-Spine-200  0:01     157.9   1.9%      170       1.4   0.0%        1
Et5       A-Harn-205   0:01       0.8   0.0%        1      95.3   1.2%      170
Ma1                    0:05       0.0   0.0%        0       0.3   0.0%        0
Po200                  0:01       0.8   0.0%        1      95.3   1.2%      170
```

