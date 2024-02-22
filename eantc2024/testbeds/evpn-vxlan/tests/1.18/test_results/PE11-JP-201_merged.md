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
  Description              Neighbor       V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  ANET.IPV4                20.200.201.200 4 65000           2938      2850    0    0    1d16h Estab   27     27
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.201, local AS number 65201
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  ANET.EVPN                100.0.0.200 4 65000           9240      5657    0    0    1d16h Estab   193    193
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.201, local AS number 65201
BGP routing table entry for auto-discovery 0000:0000:0000:0000:0000, Route Distinguisher: 100.0.0.103:20
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1103:1103 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 Route-Target-AS:1304:1304 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
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
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
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
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
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
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
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
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
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
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.201, local AS number 65201
BGP routing table entry for mac-ip 0013.0100.0001, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0001 10.10.201.201, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0001 10.10.201.201, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0002, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0002, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0002 10.30.1.201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0002 10.30.1.201, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0003, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0003, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0003 10.30.2.201, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0003 10.30.2.201, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0014.0100.0002, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0014.0100.0002 10.30.1.56, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0014.0100.0003, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0014.0100.0003 10.30.2.56, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0015.0100.0002, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0015.0100.0002 10.30.1.203, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0015.0100.0002 10.30.1.203, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0015.0100.0003, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0015.0100.0003 10.30.2.203, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1302 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0015.0100.0003 10.30.2.203, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0016.0100.0001, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan
      VNI: 1040 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0001 10.10.40.40, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1040 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0002, Route Distinguisher: 100.0.0.40:34068
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0002 10.30.1.40, Route Distinguisher: 100.0.0.40:34068
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0003, Route Distinguisher: 100.0.0.40:34069
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0003 10.30.2.40, Route Distinguisher: 100.0.0.40:34069
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0004, Route Distinguisher: 100.0.0.40:34070
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0004 10.30.3.40, Route Distinguisher: 100.0.0.40:34070
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0005, Route Distinguisher: 100.0.0.40:34071
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1304:1304 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0005 10.30.4.40, Route Distinguisher: 100.0.0.40:34071
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1304:1304 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0001, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan
      VNI: 1042 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0001 10.10.42.42, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1042 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0002, Route Distinguisher: 100.0.0.42:34068
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0002 10.30.1.42, Route Distinguisher: 100.0.0.42:34068
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0003, Route Distinguisher: 100.0.0.42:34069
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0003 10.30.2.42, Route Distinguisher: 100.0.0.42:34069
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0001, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0001, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0001 10.10.45.45, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0001 10.10.45.45, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0002, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0002, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0002 10.30.1.45, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0002 10.30.1.45, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0003, Route Distinguisher: 100.0.0.45:34069
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0003, Route Distinguisher: 100.0.0.46:34069
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0003 10.30.2.45, Route Distinguisher: 100.0.0.45:34069
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0003 10.30.2.45, Route Distinguisher: 100.0.0.46:34069
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0019.0100.0001 10.10.22.22, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0019.0100.0002, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0019.0100.0002 10.30.1.22, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0019.0100.0003, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0019.0100.0003 10.30.2.22, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0022.2200.0001 10.10.103.103, Route Distinguisher: 100.0.0.103:1103
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1103:1103 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:05:00:00:01
      VNI: 1103 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.10.56.253, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.30.1.254, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.30.2.254, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.56.254, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.2.254, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan
      VNI: 1040 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan
      VNI: 1042 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.22.202, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.40.202, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1040 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.42.202, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1042 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.45.202, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.45.202, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.201.202, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.201.202, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.30.1.202, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.30.1.202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.30.2.202, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.30.2.202, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 5c5a.c773.4abb, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan
      VNI: 1040 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan
      VNI: 1042 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb 10.10.40.25, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1040 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb 10.10.42.25, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1042 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb 10.10.45.25, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb 10.10.45.25, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 0013.0100.0004, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0013.0100.0004, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0013.0100.0004 10.30.3.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0013.0100.0004 10.30.3.201, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0015.0100.0004, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0015.0100.0004 10.30.3.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0015.0100.0004 10.30.3.203, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0019.0100.0004 10.30.3.22, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 444c.a873.5c75, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 444c.a873.5c75 10.30.3.202, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 444c.a873.5c75 10.30.3.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0013.0100.0005, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0013.0100.0005, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0013.0100.0005 10.30.4.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0013.0100.0005 10.30.4.201, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0015.0100.0005, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 0015.0100.0005 10.30.4.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 0015.0100.0005 10.30.4.203, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 0019.0100.0005 10.30.4.22, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 444c.a873.5c75, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 444c.a873.5c75 10.30.4.202, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 444c.a873.5c75 10.30.4.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
```

## show bgp evpn route-type imet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.201, local AS number 65201
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
      PMSI Tunnel: Ingress Replication, MPLS Label: 1022, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.40, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan
      VNI: 1040
      PMSI Tunnel: Ingress Replication, MPLS Label: 1040, Leaf Information Required: false, Tunnel ID: 100.0.0.40
BGP routing table entry for imet 100.0.0.40, Route Distinguisher: 100.0.0.40:34068
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.40
BGP routing table entry for imet 100.0.0.40, Route Distinguisher: 100.0.0.40:34069
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.40
BGP routing table entry for imet 100.0.0.40, Route Distinguisher: 100.0.0.40:34070
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.40
BGP routing table entry for imet 100.0.0.40, Route Distinguisher: 100.0.0.40:34071
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1304:1304 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.40
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan
      VNI: 1045
      PMSI Tunnel: Ingress Replication, MPLS Label: 1045, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.45:34069
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan
      VNI: 1045
      PMSI Tunnel: Ingress Replication, MPLS Label: 1045, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.46:34069
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.42, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan
      VNI: 1042
      PMSI Tunnel: Ingress Replication, MPLS Label: 1042, Leaf Information Required: false, Tunnel ID: 100.0.0.42
BGP routing table entry for imet 100.0.0.42, Route Distinguisher: 100.0.0.42:34068
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.42
BGP routing table entry for imet 100.0.0.42, Route Distinguisher: 100.0.0.42:34069
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.42
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan DF Election: Modulus-based Multicast Flags: OISM-supported, PEG, SBD
      VNI: 1000
      PMSI Tunnel: Ingress Replication, MPLS Label: 1000, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported
      VNI: 1056
      PMSI Tunnel: Ingress Replication, MPLS Label: 1056, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.103, Route Distinguisher: 100.0.0.103:2
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported, SBD
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 100.0.0.103, Route Distinguisher: 100.0.0.103:3
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported, SBD
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 100.0.0.103, Route Distinguisher: 100.0.0.103:1103
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1103:1103 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported, SBD
      VNI: 1103
      PMSI Tunnel: Ingress Replication, MPLS Label: 1103, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
      PMSI Tunnel: Ingress Replication, MPLS Label: 1201, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
BGP routing table entry for imet 100.0.0.206, Route Distinguisher: 100.0.0.206:1000
 Paths: 1 available
  65000 65206
    100.0.0.206 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan DF Election: Modulus-based Multicast Flags: IGMP proxy, OISM-supported, PEG, SBD
      VNI: 1000
      PMSI Tunnel: Ingress Replication, MPLS Label: 1000, Leaf Information Required: false, Tunnel ID: 100.0.0.206
BGP routing table entry for imet 100.0.0.206, Route Distinguisher: 100.0.0.206:1301
 Paths: 1 available
  65000 65206
    100.0.0.206 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.206
BGP routing table entry for imet 100.0.0.206, Route Distinguisher: 100.0.0.206:1302
 Paths: 1 available
  65000 65206
    100.0.0.206 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.206
BGP routing table entry for imet 1303 100.0.0.22, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 1303 100.0.0.56, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1303 100.0.0.103, Route Distinguisher: 100.0.0.103:4
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported, SBD
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 1303 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
BGP routing table entry for imet 1303 100.0.0.206, Route Distinguisher: 100.0.0.206:1303
 Paths: 1 available
  65000 65206
    100.0.0.206 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.206
BGP routing table entry for imet 1304 100.0.0.22, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65000 65022
    100.0.0.22 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 1304 100.0.0.56, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1304 100.0.0.103, Route Distinguisher: 100.0.0.103:5
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1304:1304 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported, SBD
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 1304 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
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
BGP routing table entry for imet 1304 100.0.0.206, Route Distinguisher: 100.0.0.206:1303
 Paths: 1 available
  65000 65206
    100.0.0.206 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.206
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.201, local AS number 65201
BGP routing table entry for ethernet-segment 0000:0000:0000:0000:0000 100.0.0.103, Route Distinguisher: 100.0.0.103:1
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:00:00:00:00
BGP routing table entry for ethernet-segment 0000:0000:0000:0201:0202 100.0.0.201, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:10:02:02 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0201:0202 100.0.0.202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:10:02:02 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0203:0204 100.0.0.203, Route Distinguisher: 100.0.0.203:1
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:30:02:04 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0203:0204 100.0.0.204, Route Distinguisher: 100.0.0.204:1
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:30:02:04 DF Election: Preference 200
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.201, local AS number 65201
BGP routing table entry for ip-prefix 10.10.40.0/24, Route Distinguisher: 100.0.0.40:1000
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.42.0/24, Route Distinguisher: 100.0.0.42:1000
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.45.0/24, Route Distinguisher: 100.0.0.45:4
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.45.0/24, Route Distinguisher: 100.0.0.46:4
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.56.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.20.56.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.20.206.0/24, Route Distinguisher: 100.0.0.206:1000
 Paths: 1 available
  65000 65206
    100.0.0.206 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:c4:02:71
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.40:1000
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.42:1000
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.45:4
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.46:4
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.103:2
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:05:00:00:01
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.56/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.40:1000
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.42:1000
 Paths: 1 available
  65000 65042
    100.0.0.42 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.45:4
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.46:4
 Paths: 1 available
  65000 65045
    100.0.0.41 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.103:3
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:05:00:00:01
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.56/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.40:1000
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.40:1000
 Paths: 1 available
  65000 65040
    100.0.0.40 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 100.0.1.202/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65000 65056 65202
    100.0.0.56 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 1303 10.30.3.0/24, Route Distinguisher: 100.0.0.103:4
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:05:00:00:01
      VNI: 1000
BGP routing table entry for ip-prefix 1304 10.30.4.0/24, Route Distinguisher: 100.0.0.103:5
 Paths: 1 available
  65000 65103
    100.0.0.103 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:05:00:00:01
      VNI: 1000
```

## show bgp evpn route-type smet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.201, local AS number 65201
BGP routing table entry for smet (S, G): (*, *) originating IP: 100.0.0.206, Route Distinguisher: 100.0.0.206:1000
 Paths: 1 available
  65000 65206
    100.0.0.206 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan
      Multicast Flags: exclude
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
0     10     VXLAN 10.10.22.22        0019.0100.0001  100.0.0.23         -   
0     10     VXLAN 10.10.22.22        0019.0100.0001  100.0.0.23         -   
0     1022   VXLAN 10.10.22.22        0019.0100.0001  100.0.0.23         -   
1201  1201   VXLAN 10.10.201.201      0013.0100.0001  Local              -   
1201  1201   VXLAN 10.10.201.201      0013.0100.0001  100.0.0.202        -   
1201  1201   VXLAN 10.10.201.202      444c.a873.5c75  Local              -   
1201  1201   VXLAN 10.10.201.202      444c.a873.5c75  100.0.0.202        -   
1301  1301   VXLAN 10.30.1.45         0018.0100.0002  100.0.0.41         -   
1301  1301   VXLAN 10.30.1.45         0018.0100.0002  100.0.0.41         -   
1301  1301   VXLAN 10.30.1.254        0056.5656.5656  100.0.0.56         Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.254        00aa.aaaa.aaaa  100.0.0.56         Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.42         0017.0100.0002  100.0.0.42         -   
1301  1301   VXLAN 10.30.1.56         0014.0100.0002  100.0.0.56         -   
1301  1301   VXLAN 10.30.1.201        0013.0100.0002  Local              -   
1301  1301   VXLAN 10.30.1.201        0013.0100.0002  100.0.0.202        -   
1301  1301   VXLAN 10.30.1.22         0019.0100.0002  100.0.0.22         -   
1301  1301   VXLAN 10.30.1.203        0015.0100.0002  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.203        0015.0100.0002  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.103        0022.2200.0002  100.0.0.103        -   
1301  1301   VXLAN 10.30.1.40         0016.0100.0002  100.0.0.40         -   
1301  1301   VXLAN 10.30.1.202        444c.a873.5c75  Local              -   
1301  1301   VXLAN 10.30.1.202        444c.a873.5c75  100.0.0.202        -   
1302  1302   VXLAN 10.30.2.42         0017.0100.0003  100.0.0.42         -   
1302  1302   VXLAN 10.30.2.201        0013.0100.0003  Local              -   
1302  1302   VXLAN 10.30.2.201        0013.0100.0003  100.0.0.202        -   
1302  1302   VXLAN 10.30.2.254        00aa.aaaa.aaaa  100.0.0.56         Stic
                                                                         ky  
1302  1302   VXLAN 10.30.2.56         0014.0100.0003  100.0.0.56         -   
1302  1302   VXLAN 10.30.2.202        444c.a873.5c75  Local              -   
1302  1302   VXLAN 10.30.2.202        444c.a873.5c75  100.0.0.202        -   
1302  1302   VXLAN 10.30.2.103        0022.2200.0003  100.0.0.103        -   
1302  1302   VXLAN 10.30.2.254        0056.5656.5656  100.0.0.56         Stic
                                                                         ky  
1302  1302   VXLAN 10.30.2.45         0018.0100.0003  100.0.0.41         -   
1302  1302   VXLAN 10.30.2.45         0018.0100.0003  100.0.0.41         -   
1302  1302   VXLAN 10.30.2.203        0015.0100.0003  100.0.0.204        -   
1302  1302   VXLAN 10.30.2.203        0015.0100.0003  100.0.0.203        -   
1302  1302   VXLAN 10.30.2.22         0019.0100.0003  100.0.0.23         -   
1302  1302   VXLAN 10.30.2.22         0019.0100.0003  100.0.0.22         -   
1302  1302   VXLAN 10.30.2.40         0016.0100.0003  100.0.0.40         -   
1303  1303   VXLAN 10.30.3.254        0056.5656.5656  100.0.0.56         Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.201        0013.0100.0004  Local              -   
1303  1303   VXLAN 10.30.3.201        0013.0100.0004  100.0.0.202        -   
1303  1303   VXLAN 10.30.3.254        00aa.aaaa.aaaa  100.0.0.56         Stic
                                                                         ky  
1303  1303   VXLAN 10.30.3.203        0015.0100.0004  100.0.0.204        -   
1303  1303   VXLAN 10.30.3.203        0015.0100.0004  100.0.0.203        -   
1303  1303   VXLAN 10.30.3.22         0019.0100.0004  100.0.0.22         -   
1303  1303   VXLAN 10.30.3.103        0022.2200.0004  100.0.0.103        -   
1303  1303   VXLAN 10.30.3.202        444c.a873.5c75  Local              -   
1303  1303   VXLAN 10.30.3.202        444c.a873.5c75  100.0.0.202        -   
1303  1303   VXLAN 10.30.3.40         0016.0100.0004  100.0.0.40         -   
1304  1304   VXLAN 10.30.4.201        0013.0100.0005  Local              -   
1304  1304   VXLAN 10.30.4.201        0013.0100.0005  100.0.0.202        -   
1304  1304   VXLAN 10.30.4.203        0015.0100.0005  100.0.0.203        -   
1304  1304   VXLAN 10.30.4.203        0015.0100.0005  100.0.0.204        -   
1304  1304   VXLAN 10.30.4.254        0056.5656.5656  100.0.0.56         Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.202        444c.a873.5c75  Local              -   
1304  1304   VXLAN 10.30.4.202        444c.a873.5c75  100.0.0.202        -   
1304  1304   VXLAN 10.30.4.254        00aa.aaaa.aaaa  100.0.0.56         Stic
                                                                         ky  
1304  1304   VXLAN 10.30.4.22         0019.0100.0005  100.0.0.22         -   
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

 B E      20.22.200.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.40.200.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.42.200.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.44.200.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.45.200.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.46.200.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.56.200.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.103.200.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 C        20.200.201.0/24
           directly connected, Ethernet1
 B E      20.200.202.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.200.203.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.200.204.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.200.206.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.22/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.40/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.41/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.42/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.44/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.45/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.46/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.56/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.103/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.200/32 [20/0]
           via 20.200.201.200, Ethernet1
 C        100.0.0.201/32
           directly connected, Loopback0
 B E      100.0.0.202/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.203/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.204/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.206/32 [20/0]
           via 20.200.201.200, Ethernet1

```

## show ip arp

```text
Address         Age (sec)  Hardware Addr   Interface
20.200.201.200    0:00:15  444c.a873.5c75  Ethernet1
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

 B E      20.22.200.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.40.200.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.42.200.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.44.200.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.45.200.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.46.200.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.56.200.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.103.200.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 C        20.200.201.0/24
           directly connected, Ethernet1
 B E      20.200.202.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.200.203.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.200.204.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      20.200.206.0/24 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.22/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.40/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.41/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.42/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.44/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.45/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.46/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.56/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.103/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.200/32 [20/0]
           via 20.200.201.200, Ethernet1
 C        100.0.0.201/32
           directly connected, Loopback0
 B E      100.0.0.202/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.203/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.204/32 [20/0]
           via 20.200.201.200, Ethernet1
 B E      100.0.0.206/32 [20/0]
           via 20.200.201.200, Ethernet1


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

 B E      10.10.40.25/32 [20/0]
           via VTEP 100.0.0.40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      10.10.40.40/32 [20/0]
           via VTEP 100.0.0.40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      10.10.40.202/32 [20/0]
           via VTEP 100.0.0.40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      10.10.40.0/24 [20/0]
           via VTEP 100.0.0.40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      10.10.42.25/32 [20/0]
           via VTEP 100.0.0.42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      10.10.42.42/32 [20/0]
           via VTEP 100.0.0.42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      10.10.42.202/32 [20/0]
           via VTEP 100.0.0.42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      10.10.42.0/24 [20/0]
           via VTEP 100.0.0.42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      10.10.45.25/32 [20/0]
           via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:7b:8b:87
           via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:b7:50:5f
 B E      10.10.45.45/32 [20/0]
           via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:7b:8b:87
           via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:b7:50:5f
 B E      10.10.45.202/32 [20/0]
           via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:7b:8b:87
           via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:b7:50:5f
 B E      10.10.45.0/24 [20/0]
           via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:7b:8b:87
           via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:b7:50:5f
 B E      10.10.56.0/24 [20/0]
           via VTEP 100.0.0.56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      10.10.103.103/32 [20/0]
           via VTEP 100.0.0.103 VNI 1000 router-mac 00:01:05:00:00:01
 C        10.10.201.0/24
           directly connected, Vlan1201
 B E      10.20.56.0/24 [20/0]
           via VTEP 100.0.0.56 VNI 1000 router-mac 00:01:00:00:00:56
 B E      10.20.206.0/24 [20/0]
           via VTEP 100.0.0.206 VNI 1000 router-mac 98:5d:82:c4:02:71
 B E      10.30.1.40/32 [20/0]
           via VTEP 100.0.0.40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      10.30.1.42/32 [20/0]
           via VTEP 100.0.0.42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      10.30.1.45/32 [20/0]
           via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:7b:8b:87
           via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:b7:50:5f
 B E      10.30.1.56/32 [20/0]
           via VTEP 100.0.0.56 VNI 1000 router-mac 00:01:00:00:00:56
 C        10.30.1.0/24
           directly connected, Vlan1301
 B E      10.30.2.40/32 [20/0]
           via VTEP 100.0.0.40 VNI 1000 router-mac 24:6c:84:74:8d:db
 B E      10.30.2.42/32 [20/0]
           via VTEP 100.0.0.42 VNI 1000 router-mac 40:14:82:7b:84:ab
 B E      10.30.2.45/32 [20/0]
           via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:7b:8b:87
           via VTEP 100.0.0.41 VNI 1000 router-mac 6c:31:0e:b7:50:5f
 B E      10.30.2.56/32 [20/0]
           via VTEP 100.0.0.56 VNI 1000 router-mac 00:01:00:00:00:56
 C        10.30.2.0/24
           directly connected, Vlan1302
 B E      10.30.3.40/32 [20/0]
           via VTEP 100.0.0.40 VNI 1000 router-mac 24:6c:84:74:8d:db
 C        10.30.3.0/24
           directly connected, Vlan1303
 B E      10.30.4.40/32 [20/0]
           via VTEP 100.0.0.40 VNI 1000 router-mac 24:6c:84:74:8d:db
 C        10.30.4.0/24
           directly connected, Vlan1304
 C        100.0.1.201/32
           directly connected, Loopback100
 B E      100.0.1.202/32 [20/0]
           via VTEP 100.0.0.56 VNI 1000 router-mac 00:01:00:00:00:56

```

## show ip arp vrf all

```text

VRF: default
Address         Age (sec)  Hardware Addr   Interface
20.200.201.200    0:00:15  444c.a873.5c75  Ethernet1

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.20.2      0:01:08  bcea.fa02.6ce2  Management1
192.168.20.18     0:01:38  e484.29cd.e801  Management1
192.168.20.19     0:02:51  c407.7858.8001  Management1
192.168.20.20     0:04:53  e484.29d0.4001  Management1
192.168.20.21     0:02:39  7081.85c1.b801  Management1
192.168.20.22     0:04:23  c407.780a.9f04  Management1
192.168.20.23     0:03:04  c407.780a.7750  Management1
192.168.20.24     0:04:53  6c87.2089.ede5  Management1
192.168.20.25     0:01:14  6c87.2089.ece5  Management1
192.168.20.26     0:04:53  04a9.59d5.df66  Management1
192.168.20.29     0:01:26  90f7.b223.d466  Management1
192.168.20.52     0:02:33  f83e.95dc.1289  Management1
192.168.21.50     0:02:57  a84f.b1a5.5221  Management1
192.168.21.59     0:02:39  6607.f5d1.ae16  Management1

VRF: tenant-a
Address         Age (sec)  Hardware Addr   Interface
10.10.201.201     0:01:39  0013.0100.0001  Vlan1201, Port-Channel100
10.10.201.202     0:00:16  444c.a873.5c75  Vlan1201, Port-Channel100
10.30.1.22              -  0019.0100.0002  Vlan1301, Vxlan1
10.30.1.40              -  0016.0100.0002  Vlan1301, Vxlan1
10.30.1.42              -  0017.0100.0002  Vlan1301, Vxlan1
10.30.1.45              -  0018.0100.0002  Vlan1301, Vxlan1
10.30.1.56              -  0014.0100.0002  Vlan1301, Vxlan1
10.30.1.201       0:07:19  0013.0100.0002  Vlan1301, Port-Channel100
10.30.1.202       0:03:51  444c.a873.5c75  Vlan1301, Port-Channel100
10.30.1.203             -  0015.0100.0002  Vlan1301, Vxlan1
10.30.2.22              -  0019.0100.0003  Vlan1302, Vxlan1
10.30.2.40              -  0016.0100.0003  Vlan1302, Vxlan1
10.30.2.42              -  0017.0100.0003  Vlan1302, Vxlan1
10.30.2.45              -  0018.0100.0003  Vlan1302, Vxlan1
10.30.2.56              -  0014.0100.0003  Vlan1302, Vxlan1
10.30.2.201       0:10:07  0013.0100.0003  Vlan1302, Port-Channel100
10.30.2.202       0:02:25  444c.a873.5c75  Vlan1302, Port-Channel100
10.30.2.203             -  0015.0100.0003  Vlan1302, Vxlan1
10.30.3.22              -  0019.0100.0004  Vlan1303, Vxlan1
10.30.3.40        0:16:08  0016.0100.0004  Vlan1303, not learned
10.30.3.201       0:11:43  0013.0100.0004  Vlan1303, Port-Channel100
10.30.3.202       0:02:25  444c.a873.5c75  Vlan1303, Port-Channel100
10.30.3.203             -  0015.0100.0004  Vlan1303, Vxlan1
10.30.4.22              -  0019.0100.0005  Vlan1304, Vxlan1
10.30.4.201       0:11:43  0013.0100.0005  Vlan1304, Port-Channel100
10.30.4.202       0:01:39  444c.a873.5c75  Vlan1304, Port-Channel100
10.30.4.203             -  0015.0100.0005  Vlan1304, Vxlan1
```

## show vxlan address-table

```text
          Vxlan Mac Address Table
----------------------------------------------------------------------

VLAN  Mac Address     Type      Prt  VTEP             Moves   Last Move
----  -----------     ----      ---  ----             -----   ---------
1301  0014.0100.0002  EVPN      Vx1  100.0.0.56       1       0:26:47 ago
1301  0015.0100.0002  EVPN      Vx1  100.0.0.203      1       0:49:51 ago
                                     100.0.0.204    
1301  0016.0100.0002  EVPN      Vx1  100.0.0.40       1       2:37:55 ago
1301  0017.0100.0002  EVPN      Vx1  100.0.0.42       1       2:37:54 ago
1301  0018.0100.0002  EVPN      Vx1  100.0.0.41       1       2:37:55 ago
1301  0019.0100.0002  EVPN      Vx1  100.0.0.22       1       1:41:06 ago
1301  0056.5656.5656  EVPN      Vx1  100.0.0.56       1       1 day, 16:33:37 ago
1302  0014.0100.0003  EVPN      Vx1  100.0.0.56       1       0:26:47 ago
1302  0015.0100.0003  EVPN      Vx1  100.0.0.203      1       0:49:51 ago
                                     100.0.0.204    
1302  0016.0100.0003  EVPN      Vx1  100.0.0.40       1       2:37:55 ago
1302  0017.0100.0003  EVPN      Vx1  100.0.0.42       1       2:37:54 ago
1302  0018.0100.0003  EVPN      Vx1  100.0.0.41       1       2:37:55 ago
1302  0019.0100.0003  EVPN      Vx1  100.0.0.22       1       1:41:06 ago
1302  0056.5656.5656  EVPN      Vx1  100.0.0.56       1       1 day, 16:33:37 ago
1303  0015.0100.0004  EVPN      Vx1  100.0.0.203      1       0:49:51 ago
                                     100.0.0.204    
1303  0019.0100.0004  EVPN      Vx1  100.0.0.22       1       1:41:06 ago
1303  0056.5656.5656  EVPN      Vx1  100.0.0.56       1       1 day, 16:33:37 ago
1304  0015.0100.0005  EVPN      Vx1  100.0.0.203      1       0:22:50 ago
                                     100.0.0.204    
1304  0019.0100.0005  EVPN      Vx1  100.0.0.22       1       1:41:06 ago
1304  0056.5656.5656  EVPN      Vx1  100.0.0.56       1       1 day, 16:33:37 ago
Total Remote Mac Addresses for this criterion: 20
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
VNI        VLAN       VRF       Source       
---------- ---------- --------- ------------ 
1000       4094                 evpn         

```

## show mac address-table

```text
          Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports      Moves   Last Move
----    -----------       ----        -----      -----   ---------
1201    0013.0100.0001    DYNAMIC     Po100      1       0:01:42 ago
1201    00aa.aaaa.aaaa    STATIC      Router
1201    2899.3a8f.8f6f    STATIC      Router
1201    444c.a873.5c75    DYNAMIC     Po100      1       0:00:16 ago
1301    0013.0100.0002    DYNAMIC     Po100      1       0:28:08 ago
1301    0014.0100.0002    DYNAMIC     Vx1        1       0:26:47 ago
1301    0015.0100.0002    DYNAMIC     Vx1        1       0:49:51 ago
1301    0016.0100.0002    DYNAMIC     Vx1        1       2:37:55 ago
1301    0017.0100.0002    DYNAMIC     Vx1        1       2:37:55 ago
1301    0018.0100.0002    DYNAMIC     Vx1        1       2:37:55 ago
1301    0019.0100.0002    DYNAMIC     Vx1        1       1:41:07 ago
1301    0056.5656.5656    STATIC      Vx1
1301    00aa.aaaa.aaaa    STATIC      Router
1301    2899.3a8f.8f6f    STATIC      Router
1301    444c.a873.5c75    DYNAMIC     Po100      1       0:03:50 ago
1302    0013.0100.0003    DYNAMIC     Po100      1       0:27:25 ago
1302    0014.0100.0003    DYNAMIC     Vx1        1       0:26:47 ago
1302    0015.0100.0003    DYNAMIC     Vx1        1       0:49:51 ago
1302    0016.0100.0003    DYNAMIC     Vx1        1       2:37:55 ago
1302    0017.0100.0003    DYNAMIC     Vx1        1       2:37:55 ago
1302    0018.0100.0003    DYNAMIC     Vx1        1       2:37:55 ago
1302    0019.0100.0003    DYNAMIC     Vx1        1       1:41:07 ago
1302    0056.5656.5656    STATIC      Vx1
1302    00aa.aaaa.aaaa    STATIC      Router
1302    2899.3a8f.8f6f    STATIC      Router
1302    444c.a873.5c75    DYNAMIC     Po100      1       0:02:24 ago
1303    0013.0100.0004    DYNAMIC     Po100      1       0:11:43 ago
1303    0015.0100.0004    DYNAMIC     Vx1        1       0:49:51 ago
1303    0019.0100.0004    DYNAMIC     Vx1        1       1:41:07 ago
1303    0056.5656.5656    STATIC      Vx1
1303    00aa.aaaa.aaaa    STATIC      Router
1303    2899.3a8f.8f6f    STATIC      Router
1303    444c.a873.5c75    DYNAMIC     Po100      1       0:02:24 ago
1304    0013.0100.0005    DYNAMIC     Po100      1       0:11:43 ago
1304    0015.0100.0005    DYNAMIC     Vx1        1       0:22:50 ago
1304    0019.0100.0005    DYNAMIC     Vx1        1       1:41:07 ago
1304    0056.5656.5656    STATIC      Vx1
1304    00aa.aaaa.aaaa    STATIC      Router
1304    2899.3a8f.8f6f    STATIC      Router
1304    444c.a873.5c75    DYNAMIC     Po100      1       0:01:42 ago
4094    00aa.aaaa.aaaa    STATIC      Router
4094    2899.3a8f.8f6f    STATIC      Router
Total Mac Addresses for this criterion: 42

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
0019.0100.0003, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.22
00aa.aaaa.aaaa, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
0015.0100.0002, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 17: 2-way
      VTEP 100.0.0.203
      VTEP 100.0.0.204
0017.0100.0002, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.42
0056.5656.5656, VLAN 1303, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
444c.a873.5c75, VLAN 1302, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0019.0100.0005, VLAN 1304, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.22
0018.0100.0002, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.41
0018.0100.0003, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.41
00aa.aaaa.aaaa, VLAN 1303, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
0016.0100.0002, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.40
444c.a873.5c75, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0013.0100.0004, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0013.0100.0001, VLAN 1201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0013.0100.0003, VLAN 1302, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0056.5656.5656, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
0016.0100.0003, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.40
0015.0100.0004, VLAN 1303, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 17: 2-way
      VTEP 100.0.0.203
      VTEP 100.0.0.204
0019.0100.0004, VLAN 1303, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.22
0056.5656.5656, VLAN 1302, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
444c.a873.5c75, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
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
0013.0100.0005, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
444c.a873.5c75, VLAN 1201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0056.5656.5656, VLAN 1304, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   VTEP 100.0.0.56
0013.0100.0002, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0019.0100.0002, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   VTEP 100.0.0.22
444c.a873.5c75, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel100
0015.0100.0003, VLAN 1302, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 17: 2-way
      VTEP 100.0.0.203
      VTEP 100.0.0.204
0015.0100.0005, VLAN 1304, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 17: 2-way
      VTEP 100.0.0.203
      VTEP 100.0.0.204
```

## show vxlan flood vtep domain local

```text
          VXLAN Flood VTEP Table
--------------------------------------------------------------------------------

VLANS                            Ip Address
-----------------------------   ------------------------------------------------
1201                            100.0.0.202    
1301-1302                       100.0.0.22      100.0.0.40      100.0.0.41     
                                100.0.0.42      100.0.0.56      100.0.0.103    
                                100.0.0.202     100.0.0.203     100.0.0.204    
                                100.0.0.206    
1303                            100.0.0.22      100.0.0.56      100.0.0.103    
                                100.0.0.202     100.0.0.203     100.0.0.204    
                                100.0.0.206    
1304                            100.0.0.22      100.0.0.56      100.0.0.202    
                                100.0.0.203     100.0.0.204     100.0.0.206    
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
  Local VXLAN IP address: 100.0.0.201
  VXLAN: enabled
  MPLS: disabled
  Local ethernet segment:
    ESI: 0000:0000:0000:0201:0202
      Interface: Port-Channel100
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:10:02:02
      DF election algorithm: preference
      Designated forwarder: 100.0.0.201
      Non-Designated forwarder: 100.0.0.202
EVPN instance: VLAN 1301
  Route distinguisher: 100.0.0.201:1301
  Route target import: Route-Target-AS:1301:1301
  Route target export: Route-Target-AS:1301:1301
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.201
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:0000:0000:0203:0204
    Active TEPs: 100.0.0.203, 100.0.0.204
  Local ethernet segment:
    ESI: 0000:0000:0000:0201:0202
      Interface: Port-Channel100
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:10:02:02
      DF election algorithm: preference
      Designated forwarder: 100.0.0.201
      Non-Designated forwarder: 100.0.0.202
EVPN instance: VLAN 1302
  Route distinguisher: 100.0.0.201:1302
  Route target import: Route-Target-AS:1302:1302
  Route target export: Route-Target-AS:1302:1302
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.201
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:0000:0000:0203:0204
    Active TEPs: 100.0.0.203, 100.0.0.204
  Local ethernet segment:
    ESI: 0000:0000:0000:0201:0202
      Interface: Port-Channel100
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:10:02:02
      DF election algorithm: preference
      Designated forwarder: 100.0.0.201
      Non-Designated forwarder: 100.0.0.202
EVPN instance: VLAN-aware bundle 1303-1304
  Route distinguisher: 100.0.0.201:1303
  Route target import: Route-Target-AS:1303:1303
  Route target export: Route-Target-AS:1303:1303
  Service interface: VLAN-aware bundle
  Local VXLAN IP address: 100.0.0.201
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:0000:0000:0203:0204
    Active TEPs: 100.0.0.203, 100.0.0.204
  Local ethernet segment:
    ESI: 0000:0000:0000:0201:0202
      Interface: Port-Channel100
      Mode: all-active
      State: up
      ES-Import RT: 00:00:20:10:02:02
      DF election algorithm: preference
      Designated forwarder: 100.0.0.201
      Non-Designated forwarder: 100.0.0.202
```

## show interfaces counters rates | nz

```text
Port      Name        Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Et1       A-Spine-200  0:01     79.1   0.9%       85      0.5   0.0%        0
Et5       A-Harn-205   0:01      0.3   0.0%        0     47.7   0.6%       85
Ma1                    0:05      0.0   0.0%        0      0.2   0.0%        0
Po100                  0:01      0.3   0.0%        0     47.7   0.6%       85
```

