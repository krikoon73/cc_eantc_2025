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
  CISCO_SPINE_IPV4         20.40.202.40   4 65040           1124      1320    0    0 17:55:06 Estab   8      8
  ANET.IPV4                20.200.202.200 4 65000           1955      1924    0    0 00:53:01 Estab   11     11
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.202, local AS number 65202
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  CISCO_EVPN_REMOTE        100.0.0.40  4 65040           1272      1462    0    0 17:55:02 Estab   35     35
  ANET.EVPN                100.0.0.200 4 65000           7669      4537    0    0 00:53:00 Estab   62     62
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
  65040 65201
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan
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
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.201:2
 Paths: 1 available
  65040 65201
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:2
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:51301:51301 Route-Target-AS:65040:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
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
BGP routing table entry for mac-ip 00cc.cccc.bbbb, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65000 65203
    100.0.0.203 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 3333.3333.3333, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201 65040 65045
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 3333.3333.3333, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65040 65045
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 3333.3333.3333 10.30.1.50, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201 65040 65045
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 3333.3333.3333 10.30.1.50, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65040 65045
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 6c31.0e7b.8b87, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201 65040 65045
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.45:512 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 6c31.0e7b.8b87, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65040 65045
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.45:512 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 6c31.0eb7.505f, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201 65040 65045
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.46:512 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 6c31.0eb7.505f, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65040 65045
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.46:512 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65040 65201 65000 65204
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.203 remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65040 65201 65000 65204
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:51301:51301 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.203 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 00cc.cccc.bbbb remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65040 65201 65000 65203
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 00cc.cccc.bbbb remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
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
BGP routing table entry for imet 100.0.0.201 remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65040 65201
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan
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
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:11:11:11:11:11 DF Election: Preference 50
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:11:11:11:11:11 DF Election: Preference 150
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.201 remote, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  65040 65201
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:11:11:11:11:11 DF Election: Preference 50
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
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:00:00:fe:15
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
BGP routing table entry for ip-prefix 10.10.44.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201 65040 65045
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.10.44.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65040 65045
    - from - (0.0.0.0)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
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
 Paths: 2 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  65040 65201
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65040 65201 65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
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
  65040 65201 65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65201
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 3 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  65040 65201
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN
  65040 65045
    - from - (0.0.0.0)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
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
BGP routing table entry for ip-prefix 10.30.1.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65040 65201 65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65040 65201 65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN 1:1:EVPN
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
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65040 65201 65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN 1:1:EVPN
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
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65040 65201 65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN 1:1:EVPN
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
BGP routing table entry for ip-prefix 100.0.1.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65040 65201 65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
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
  65040 65201 65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.204/32, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65000 65204
    100.0.0.204 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
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
BGP routing table entry for ip-prefix 10.10.44.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65201 65040 65045
    - from - (0.0.0.0)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN 2:2:EVPN
BGP routing table entry for ip-prefix 10.10.201.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.201.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  65000 65201
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201 65000 65203
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.203/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201 65000 65203
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.203/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
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
BGP routing table entry for ip-prefix 10.30.1.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 4 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65201
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.203/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201 65000 65204
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.203/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.2.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201 65000 65203
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.2.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201 65000 65204
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201 65000 65203
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.203/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201 65000 65203
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.203/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.204/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201 65000 65204
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.204/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
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
1301  1301   VXLAN 10.30.1.50         3333.3333.3333  100.0.0.45         Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.50         3333.3333.3333  100.0.0.46         Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.50         3333.3333.3333  100.0.0.201        Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.203        001b.0100.0002  100.0.0.204        -   
1301  1301   VXLAN 10.30.1.203        001b.0100.0002  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.203        001b.0100.0002  100.0.0.201        -   
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

 B E      20.40.201.0/24 [20/0]
           via 20.200.202.200, Ethernet1
           via 20.40.202.40, Ethernet48
 C        20.40.202.0/24
           directly connected, Ethernet48
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
           via 20.40.202.40, Ethernet48
 B E      100.0.0.40/32 [20/0]
           via 20.40.202.40, Ethernet48
 B E      100.0.0.41/32 [20/0]
           via 20.40.202.40, Ethernet48
 B E      100.0.0.45/32 [20/0]
           via 20.40.202.40, Ethernet48
 B E      100.0.0.46/32 [20/0]
           via 20.40.202.40, Ethernet48
 B E      100.0.0.200/32 [20/0]
           via 20.200.202.200, Ethernet1
 B E      100.0.0.201/32 [20/0]
           via 20.200.202.200, Ethernet1
           via 20.40.202.40, Ethernet48
 C        100.0.0.202/32
           directly connected, Loopback0
 B E      100.0.0.203/32 [20/0]
           via 20.200.202.200, Ethernet1
 B E      100.0.0.204/32 [20/0]
           via 20.200.202.200, Ethernet1

```

## show ip arp

```text
Address         Age (sec)  Hardware Addr   Interface
20.200.202.200    0:00:12  444c.a873.5c75  Ethernet1
20.40.202.40      0:00:05  246c.8474.8ddb  Ethernet48
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
           via 20.200.202.200, Ethernet1
           via 20.40.202.40, Ethernet48
 C        20.40.202.0/24
           directly connected, Ethernet48
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
           via 20.40.202.40, Ethernet48
 B E      100.0.0.40/32 [20/0]
           via 20.40.202.40, Ethernet48
 B E      100.0.0.41/32 [20/0]
           via 20.40.202.40, Ethernet48
 B E      100.0.0.45/32 [20/0]
           via 20.40.202.40, Ethernet48
 B E      100.0.0.46/32 [20/0]
           via 20.40.202.40, Ethernet48
 B E      100.0.0.200/32 [20/0]
           via 20.200.202.200, Ethernet1
 B E      100.0.0.201/32 [20/0]
           via 20.200.202.200, Ethernet1
           via 20.40.202.40, Ethernet48
 C        100.0.0.202/32
           directly connected, Loopback0
 B E      100.0.0.203/32 [20/0]
           via 20.200.202.200, Ethernet1
 B E      100.0.0.204/32 [20/0]
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

 B E      10.10.44.0/24 [20/0]
           via VTEP 100.0.0.45 VNI 1000 router-mac 6c:31:0e:7b:8b:87
 C        10.10.201.0/24
           directly connected, Vlan1201
 B E      10.10.203.203/32 [20/0]
           via VTEP 100.0.0.204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 100.0.0.203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 B E      10.10.203.0/24 [20/0]
           via VTEP 100.0.0.204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 100.0.0.203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 B E      10.30.1.203/32 [20/0]
           via VTEP 100.0.0.204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 100.0.0.203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 C        10.30.1.0/24
           directly connected, Vlan1301
 B E      10.30.2.0/24 [20/0]
           via VTEP 100.0.0.204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 100.0.0.203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 B E      10.30.3.0/24 [20/0]
           via VTEP 100.0.0.204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 100.0.0.203 VNI 1000 router-mac 38:38:a6:21:e8:2f
 B E      10.30.4.0/24 [20/0]
           via VTEP 100.0.0.204 VNI 1000 router-mac 98:5d:82:a2:04:f9
           via VTEP 100.0.0.203 VNI 1000 router-mac 38:38:a6:21:e8:2f
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
20.200.202.200    0:00:12  444c.a873.5c75  Ethernet1
20.40.202.40      0:00:06  246c.8474.8ddb  Ethernet48

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.20.2      0:04:25  bcea.fa02.6ce2  Management1
192.168.20.19     0:00:46  c407.7858.8001  Management1
192.168.20.20     0:01:59  e484.29d0.4001  Management1
192.168.20.21     0:04:31  7081.85c1.b801  Management1
192.168.20.22     0:02:11  c407.780a.9f04  Management1
192.168.20.23     0:00:52  c407.780a.7750  Management1
192.168.20.24     0:00:52  6c87.2089.ede5  Management1
192.168.20.26     0:03:30  04a9.59d5.df66  Management1
192.168.20.27     0:04:19  04a9.59d5.dfe6  Management1
192.168.20.28     0:02:35  98a9.2d59.bae6  Management1
192.168.20.29     0:03:00  90f7.b223.d466  Management1
192.168.20.52     0:00:52  f83e.95dc.1289  Management1
192.168.21.47     0:04:31  5c5a.c7ff.8a0a  Management1
192.168.21.50     0:01:53  a84f.b1a5.5221  Management1
192.168.21.59     0:01:10  6607.f5d1.ae16  Management1

VRF: tenant-a
Address         Age (sec)  Hardware Addr   Interface
10.30.1.203             -  001b.0100.0002  Vlan1301, Vxlan1
```

## show vxlan address-table

```text
          Vxlan Mac Address Table
----------------------------------------------------------------------

VLAN  Mac Address     Type      Prt  VTEP             Moves   Last Move
----  -----------     ----      ---  ----             -----   ---------
1301  001b.0100.0002  EVPN      Vx1  100.0.0.203      1       0:01:51 ago
                                     100.0.0.204    
1301  00cc.cccc.bbbb  EVPN      Vx1  100.0.0.203      1       0:27:18 ago
                                     100.0.0.204    
1301  3333.3333.3333  EVPN      Vx1  100.0.0.45       1       0:27:18 ago
                                     100.0.0.46     
1301  6c31.0e7b.8b87  EVPN      Vx1  100.0.0.45       1       0:27:18 ago
                                     100.0.0.46     
1301  6c31.0eb7.505f  EVPN      Vx1  100.0.0.45       1       0:27:18 ago
                                     100.0.0.46     
Total Remote Mac Addresses for this criterion: 5
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
1301    001b.0100.0002    DYNAMIC     Vx1        1       0:01:52 ago
1301    00aa.aaaa.aaaa    STATIC      Router
1301    00cc.cccc.bbbb    STATIC      Vx1
1301    2cdd.e90b.25b7    STATIC      Router
1301    3333.3333.3333    STATIC      Vx1
1301    6c31.0e7b.8b87    STATIC      Vx1
1301    6c31.0eb7.505f    STATIC      Vx1
1302    00aa.aaaa.aaaa    STATIC      Router
1302    2cdd.e90b.25b7    STATIC      Router
1303    00aa.aaaa.aaaa    STATIC      Router
1303    2cdd.e90b.25b7    STATIC      Router
1304    00aa.aaaa.aaaa    STATIC      Router
1304    2cdd.e90b.25b7    STATIC      Router
4092    00aa.aaaa.aaaa    STATIC      Router
4092    2cdd.e90b.25b7    STATIC      Router
Total Mac Addresses for this criterion: 19

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
6c31.0eb7.505f, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 97: 2-way
      VTEP 100.0.0.45
      VTEP 100.0.0.46
00cc.cccc.bbbb, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 96: 2-way
      VTEP 100.0.0.203
      VTEP 100.0.0.204
6c31.0e7b.8b87, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 97: 2-way
      VTEP 100.0.0.45
      VTEP 100.0.0.46
3333.3333.3333, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 97: 2-way
      VTEP 100.0.0.45
      VTEP 100.0.0.46
001b.0100.0002, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 96: 2-way
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
1301-1304                       100.0.0.201     100.0.0.203     100.0.0.204    
```

## show vxlan flood vtep domain remote

```text
          VXLAN Flood VTEP Table
--------------------------------------------------------------------------------

VLANS                            Ip Address
-----------------------------   ------------------------------------------------
1301                            100.0.0.45      100.0.0.46     
```

## show bgp evpn domain remote detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.202, local AS number 65202
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65040 65201
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan
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
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.201:2
 Paths: 1 available
  65040 65201
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111 remote, Route Distinguisher: 100.0.0.202:2
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:51301:51301 Route-Target-AS:65040:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
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
BGP routing table entry for mac-ip 001b.0100.0002 remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65040 65201 65000 65204
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.203 remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65040 65201 65000 65204
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:51301:51301 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.203 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 00cc.cccc.bbbb remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65040 65201 65000 65203
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 00cc.cccc.bbbb remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
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
BGP routing table entry for imet 100.0.0.201 remote, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65040 65201
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.202 remote, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:51301:51301 TunnelEncap:tunnelTypeVxlan
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
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.201 remote, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  65040 65201
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:11:11:11:11:11 DF Election: Preference 50
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
    100.0.0.46 from 100.0.0.40 (100.0.0.40)
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
BGP routing table entry for ip-prefix 10.10.44.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65201 65040 65045
    - from - (0.0.0.0)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN 2:2:EVPN
BGP routing table entry for ip-prefix 10.10.201.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.201.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  65000 65201
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201 65000 65203
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.203/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201 65000 65203
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.203/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
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
BGP routing table entry for ip-prefix 10.30.1.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 4 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65201
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.203/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201 65000 65204
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.203/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.2.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201 65000 65203
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.2.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201 65000 65204
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.0/24 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201 65000 65203
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.0/24 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 2 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.203/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201 65000 65203
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.203/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.204/32 remote, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65040 65201 65000 65204
    100.0.0.201 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.204/32 remote, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65040:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
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
      ES-Import RT: 00:11:11:11:11:11
      DF election algorithm: preference
      Designated forwarder: 100.0.0.202
      Non-Designated forwarder: 100.0.0.201
EVPN instance: VLAN 1301
  Route distinguisher: 100.0.0.202:1301
  Route distinguisher remote: 100.0.0.202:1301
  Route target import: Route-Target-AS:1301:1301
  Route target export: Route-Target-AS:1301:1301
  Route target import remote: Route-Target-AS:51301:51301
  Route target export remote: Route-Target-AS:51301:51301
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.202
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:0000:0000:0203:0204
    Active TEPs: 100.0.0.203, 100.0.0.204
    ESI: 0300:0000:00fe:1500:0309
    Active TEPs: 100.0.0.45, 100.0.0.46
  Local ethernet segment:
    ESI: 0000:1111:1111:1111:1111
      Interface: Vxlan1
      Mode: all-active
      State: up
      ES-Import RT: 00:11:11:11:11:11
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
      ES-Import RT: 00:11:11:11:11:11
      DF election algorithm: preference
      Designated forwarder: 100.0.0.202
      Non-Designated forwarder: 100.0.0.201
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
  Remote ethernet segment:
    ESI: 0000:0000:0000:0203:0204
    Active TEPs: 100.0.0.203, 100.0.0.204
  Local ethernet segment:
    ESI: 0000:1111:1111:1111:1111
      Interface: Vxlan1
      Mode: all-active
      State: up
      ES-Import RT: 00:11:11:11:11:11
      DF election algorithm: preference
      Designated forwarder: 100.0.0.202
      Non-Designated forwarder: 100.0.0.201
```

## show interfaces counters rates | nz

```text
Port      Name           Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Ma1                       0:05      0.0   0.0%        0      0.2   0.0%        0
```

