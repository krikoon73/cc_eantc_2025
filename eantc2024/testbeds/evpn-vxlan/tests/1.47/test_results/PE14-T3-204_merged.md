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
  ANET.IPV4                20.200.204.200 4 65000           3725      3616    0    0    1d23h Estab   16     16
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.204, local AS number 65204
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  ANET.EVPN                100.0.0.200 4 65000          12477      5994    0    0    1d23h Estab   60     60
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
BGP routing table entry for mac-ip 001b.0100.0002, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 001c.0100.0002, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201 65040 65045
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 001c.0100.0002, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65202 65040 65045
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 001c.0100.0002 10.30.1.44, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65201 65040 65045
    100.0.0.201 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
BGP routing table entry for mac-ip 001c.0100.0002 10.30.1.44, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65202 65040 65045
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
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
  65000 65202 65040 65045
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:25:b7
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
  65000 65202 65040 65045
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:25:b7
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
  65000 65202 65040 65045
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.45:512 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:25:b7
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
  65000 65202 65040 65045
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.46:512 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 2:2:EVPN
```

## show bgp evpn route-type imet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.204, local AS number 65204
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
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:11:11:11:11:11 DF Election: Preference 50
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:11:11:11:11:11 DF Election: Preference 150
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.204, local AS number 65204
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
  65000 65202 65040 65045
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
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
 Paths: 1 available
  65000 65202
    100.0.0.202 from 100.0.0.200 (100.0.0.200)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
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
1203  1203   VXLAN 10.10.203.203      6666.6666.0001  100.0.0.103        -   
1203  1203   VXLAN 10.10.203.204      444c.a873.5c75  100.0.0.203        -   
1203  1203   VXLAN 10.10.203.203      001b.0100.0001  100.0.0.203        -   
1203  1203   VXLAN 10.10.203.203      001b.0100.0001  Local              -   
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
1301  1301   VXLAN 10.30.1.50         3333.3333.3333  100.0.0.201        Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.50         3333.3333.3333  100.0.0.202        Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.137        a244.0100.0027  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.226        001b.0100.004c  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.115        a244.0100.0011  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.114      a222.0100.000c  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.206        001b.0100.0038  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.195        a244.0100.0061  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.179      a222.0100.004d  100.0.0.201        -   
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
1301  1301   VXLAN 10.30.1.223        001b.0100.0049  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.249        001b.0100.0063  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.44         001c.0100.0002  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.44         001c.0100.0002  100.0.0.202        -   
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
1301  1301   VXLAN 10.30.1.50         3333.3333.3333  100.0.0.202        Stic
                                                                         ky  
1301  1301   VXLAN 10.30.1.213        001b.0100.003f  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.243        001b.0100.005d  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.205        001b.0100.0037  100.0.0.203        -   
1301  1301   VXLAN 10.10.103.150      a222.0100.0030  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.168        a244.0100.0046  100.0.0.201        -   
1301  1301   VXLAN 10.10.103.112      a222.0100.000a  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.159        a244.0100.003d  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.44         001c.0100.0002  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.44         001c.0100.0002  100.0.0.202        -   
1301  1301   VXLAN 10.10.103.191      a222.0100.0059  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.161        a244.0100.003f  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.154        a244.0100.0038  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.160        a244.0100.003e  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.129        a244.0100.001f  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.219        001b.0100.0045  100.0.0.203        -   
1301  1301   VXLAN 10.30.1.199        a244.0100.0065  100.0.0.201        -   
1301  1301   VXLAN 10.30.1.142        a244.0100.002c  100.0.0.201        -   
1302  1302   VXLAN 10.30.2.202        444c.a873.5c75  100.0.0.203        -   
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

 B E      20.40.201.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      20.40.202.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      20.103.200.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      20.200.201.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      20.200.202.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      20.200.203.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 C        20.200.204.0/24
           directly connected, Ethernet1
 B E      20.201.205.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.40/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.41/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.45/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.46/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.200/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.201/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.202/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.203/32 [20/0]
           via 20.200.204.200, Ethernet1
 C        100.0.0.204/32
           directly connected, Loopback0

```

## show ip arp

```text
Address         Age (sec)  Hardware Addr   Interface
20.200.204.200    0:00:16  444c.a873.5c75  Ethernet1
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
 B E      20.40.202.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      20.103.200.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      20.200.201.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      20.200.202.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      20.200.203.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 C        20.200.204.0/24
           directly connected, Ethernet1
 B E      20.201.205.0/24 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.40/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.41/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.45/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.46/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.200/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.201/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.202/32 [20/0]
           via 20.200.204.200, Ethernet1
 B E      100.0.0.203/32 [20/0]
           via 20.200.204.200, Ethernet1
 C        100.0.0.204/32
           directly connected, Loopback0


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
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
 B E      10.10.201.0/24 [20/0]
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
 C        10.10.203.0/24
           directly connected, Vlan1203
 B E      10.30.1.44/32 [20/0]
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
 B E      10.30.1.50/32 [20/0]
           via VTEP 100.0.0.201 VNI 1000 router-mac 2c:dd:e9:0b:22:83
           via VTEP 100.0.0.202 VNI 1000 router-mac 2c:dd:e9:0b:25:b7
 C        10.30.1.0/24
           directly connected, Vlan1301
 C        10.30.2.0/24
           directly connected, Vlan1302
 C        10.30.3.0/24
           directly connected, Vlan1303
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
20.200.204.200    0:00:16  444c.a873.5c75  Ethernet1

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.21.47     0:01:34  5c5a.c7ff.8a0a  Management1
192.168.21.50     0:04:19  a84f.b1a5.5221  Management1

VRF: tenant-a
Address         Age (sec)  Hardware Addr   Interface
10.10.203.203           -  001b.0100.0001  Vlan1203, Port-Channel200
10.30.1.44              -  001c.0100.0002  Vlan1301, Vxlan1
10.30.4.203       1:29:10  001b.0100.0004  Vlan1304, not learned
```

## show vxlan address-table

```text
          Vxlan Mac Address Table
----------------------------------------------------------------------

VLAN  Mac Address     Type      Prt  VTEP             Moves   Last Move
----  -----------     ----      ---  ----             -----   ---------
1301  001c.0100.0002  EVPN      Vx1  100.0.0.201      1       1:06:25 ago
                                     100.0.0.202    
1301  6c31.0e7b.8b87  EVPN      Vx1  100.0.0.201      1       1:39:25 ago
                                     100.0.0.202    
1301  6c31.0eb7.505f  EVPN      Vx1  100.0.0.201      1       1:39:25 ago
                                     100.0.0.202    
4093  c407.780a.9f31  EVPN      Vx1  100.0.30.14              1 day, 2:03:49 ago
4094  0001.0400.0001  EVPN      Vx1  100.0.0.103              1:26:16 ago
4094  2cdd.e90b.2283  EVPN      Vx1  100.0.0.201              1 day, 15:46:26 ago
4094  2cdd.e90b.25b7  EVPN      Vx1  100.0.0.202              2:05:30 ago
4094  3838.a621.e82f  EVPN      Vx1  100.0.0.203              1 day, 23:44:29 ago
Total Remote Mac Addresses for this criterion: 8
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
1203    001b.0100.0001    DYNAMIC     Po200      1       0:59:12 ago
1203    00aa.aaaa.aaaa    STATIC      Router
1301    001b.0100.0002    DYNAMIC     Po200      1       1:09:11 ago
1301    001c.0100.0002    DYNAMIC     Vx1        1       1:06:26 ago
1301    00aa.aaaa.aaaa    STATIC      Router
1301    00cc.cccc.bbbb    STATIC      Po200
1301    6c31.0e7b.8b87    STATIC      Vx1
1301    6c31.0eb7.505f    STATIC      Vx1
1302    00aa.aaaa.aaaa    STATIC      Router
1303    00aa.aaaa.aaaa    STATIC      Router
1304    00aa.aaaa.aaaa    STATIC      Router
4093    00aa.aaaa.aaaa    STATIC      Router
4093    c407.780a.9f31    DYNAMIC     Vx1        0       1 day, 2:03:49 ago
4094    0001.0400.0001    DYNAMIC     Vx1        0       1:26:17 ago
4094    00aa.aaaa.aaaa    STATIC      Router
4094    2cdd.e90b.2283    DYNAMIC     Vx1        0       1 day, 15:46:26 ago
4094    2cdd.e90b.25b7    DYNAMIC     Vx1        0       2:05:30 ago
4094    3838.a621.e82f    DYNAMIC     Vx1        0       1 day, 23:44:29 ago
Total Mac Addresses for this criterion: 18

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
6c31.0eb7.505f, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 34: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
00cc.cccc.bbbb, VLAN 1301, seq 1, pref 48, evpnIntfStaticMac, source: BGP
   Port-Channel200
6c31.0e7b.8b87, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 34: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
3333.3333.3333, VLAN 1301, seq 1, pref 48, evpnConfiguredRemoteMac, source: BGP
   Load Balance entry 34: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
001b.0100.0001, VLAN 1203, seq 1, pref 16, evpnIntfDynamicMac, source: BGP
   Port-Channel200
001c.0100.0002, VLAN 1301, seq 1, pref 16, evpnDynamicRemoteMac, source: BGP
   Load Balance entry 34: 2-way
      VTEP 100.0.0.201
      VTEP 100.0.0.202
001b.0100.0002, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
```

## show vxlan flood vtep domain local

```text
          VXLAN Flood VTEP Table
--------------------------------------------------------------------------------

VLANS                            Ip Address
-----------------------------   ------------------------------------------------
1203,4094                       100.0.0.203    
1301-1304                       100.0.0.201     100.0.0.202     100.0.0.203    
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
  Route distinguisher: 100.0.0.204:1302
  Route target import: Route-Target-AS:1302:1302
  Route target export: Route-Target-AS:1302:1302
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.204
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
  Route distinguisher: 100.0.0.204:1303
  Route target import: Route-Target-AS:1303:1303
  Route target export: Route-Target-AS:1303:1303
  Service interface: VLAN-aware bundle
  Local VXLAN IP address: 100.0.0.204
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
Et1       A-Spine-200  0:01      1.9   0.0%        2      0.9   0.0%        1
Et5       A-Harn-205   0:01      0.6   0.0%        0      1.1   0.0%        2
Ma1                    0:05      0.0   0.0%        0      0.2   0.0%        0
Po200                  0:01      0.6   0.0%        0      1.1   0.0%        2
```

