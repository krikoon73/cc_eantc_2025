# Test results for Harness1-J-205

## show hostname

```text
Hostname: Harness1-J-205
FQDN:     Harness1-J-205.ns.eantc.de
```

## show ip bgp summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.205, local AS number 65205
Neighbor Status Codes: m - Under maintenance
  Neighbor V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.205, local AS number 65205
Neighbor Status Codes: m - Under maintenance
  Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  100.0.0.22  4 65205           2512      5397    0    0 00:51:55 Estab   15     0
  100.0.0.56  4 65205           3821      7494    0    0 21:09:29 Estab   192    192
  100.0.0.201 4 65205           2377      2711    0    0 13:26:50 Estab   471    471
  100.0.0.202 4 65205           2303      2741    0    0 13:26:46 Estab   471    471
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 1303 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1303 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 1304 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:2
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.202:2
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.22:2301
 Paths: 1 available
  Local (Received from a RR-client)
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 1303 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.22:2301
 Paths: 1 available
  Local (Received from a RR-client)
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
BGP routing table entry for mac-ip 001b.0100.0002, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.201, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.203, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.203, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0033, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0033, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0034, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0034, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0034 10.30.1.202, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0034 10.30.1.202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0035, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0035, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0036, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0036, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0036 10.30.1.204, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0036 10.30.1.204, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0037, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0037, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0037 10.30.1.205, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0037 10.30.1.205, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0038, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0038, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0038 10.30.1.206, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0038 10.30.1.206, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0039, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0039, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0039 10.30.1.207, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0039 10.30.1.207, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003a, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003a, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003a 10.30.1.208, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003a 10.30.1.208, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003b, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003b, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003b 10.30.1.209, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003b 10.30.1.209, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003c, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003c, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003c 10.30.1.210, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003c 10.30.1.210, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003d, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003d, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003d 10.30.1.211, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003d 10.30.1.211, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003e, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003e, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003e 10.30.1.212, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003e 10.30.1.212, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003f, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003f, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003f 10.30.1.213, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.003f 10.30.1.213, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0040, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0040, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0040 10.30.1.214, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0040 10.30.1.214, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0041, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0041, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0041 10.30.1.215, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0041 10.30.1.215, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0042, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0042, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0042 10.30.1.216, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0042 10.30.1.216, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0043, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0043, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0043 10.30.1.217, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0043 10.30.1.217, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0044, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0044, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0044 10.30.1.218, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0044 10.30.1.218, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0045, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0045, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0045 10.30.1.219, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0045 10.30.1.219, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0046, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0046, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0046 10.30.1.220, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0046 10.30.1.220, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0047, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0047, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0047 10.30.1.221, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0047 10.30.1.221, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0048, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0048, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0048 10.30.1.222, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0048 10.30.1.222, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0049, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0049, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0049 10.30.1.223, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0049 10.30.1.223, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004a, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004a, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004a 10.30.1.224, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004a 10.30.1.224, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004b, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004b, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004b 10.30.1.225, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004b 10.30.1.225, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004c, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004c, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004c 10.30.1.226, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004c 10.30.1.226, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004d, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004d, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004d 10.30.1.227, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004d 10.30.1.227, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004e, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004e, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004e 10.30.1.228, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004e 10.30.1.228, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004f, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004f, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004f 10.30.1.229, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.004f 10.30.1.229, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0050, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0050, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0050 10.30.1.230, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0050 10.30.1.230, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0051, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0051, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0051 10.30.1.231, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0051 10.30.1.231, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0052, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0052, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0052 10.30.1.232, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0052 10.30.1.232, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0053, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0053, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0053 10.30.1.233, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0053 10.30.1.233, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0054, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0054, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0054 10.30.1.234, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0054 10.30.1.234, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0055, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0055, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0055 10.30.1.235, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0055 10.30.1.235, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0056, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0056, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0056 10.30.1.236, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0056 10.30.1.236, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0057, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0057, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0057 10.30.1.237, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0057 10.30.1.237, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0058, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0058, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0058 10.30.1.238, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0058 10.30.1.238, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0059, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0059, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0059 10.30.1.239, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0059 10.30.1.239, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005a, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005a, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005a 10.30.1.240, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005a 10.30.1.240, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005b, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005b, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005b 10.30.1.241, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005b 10.30.1.241, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005c, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005c, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005c 10.30.1.242, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005c 10.30.1.242, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005d, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005d, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005d 10.30.1.243, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005d 10.30.1.243, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005e, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005e, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005e 10.30.1.244, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005e 10.30.1.244, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005f, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005f, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005f 10.30.1.245, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.005f 10.30.1.245, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0060, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0060, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0060 10.30.1.246, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0060 10.30.1.246, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0061, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0061, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0061 10.30.1.247, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0061 10.30.1.247, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0062, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0062, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0062 10.30.1.248, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0062 10.30.1.248, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0063, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0063, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0063 10.30.1.249, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0063 10.30.1.249, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0064, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0064, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0064 10.30.1.250, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 001b.0100.0064 10.30.1.250, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 0056.5656.5656 10.10.103.254, Route Distinguisher: 100.0.0.56:1103
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1103 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.30.1.254, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.30.2.254, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1302:1302 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.103.254, Route Distinguisher: 100.0.0.56:1103
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1103 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.203.254, Route Distinguisher: 100.0.0.56:1203
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1203:1203 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1203 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00cc.cccc.bbbb, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 00cc.cccc.bbbb, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip a222.0100.0001 10.10.103.103, Route Distinguisher: 100.0.0.103:1103
 Paths: 2 available
  65206 65103 (Received from a RR-client)
    100.0.0.103 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, internal
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:02:00:00:01
      VNI: 1103 L3 VNI: 1001 ESI: 0000:0000:0000:0000:0000
  Local (Received from a RR-client)
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip a244.0101.0001 10.30.1.103, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip a244.0101.0001 10.30.1.103, Route Distinguisher: 100.0.0.103:2301
 Paths: 2 available
  65206 65103 (Received from a RR-client)
    100.0.0.103 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, internal
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:02:00:00:01
      VNI: 2301 L3 VNI: 1001 ESI: 0000:0000:0000:0000:0000
  Local (Received from a RR-client)
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 1303 001b.0100.0003, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0003, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0065, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0065, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0065 10.30.3.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0065 10.30.3.201, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0066, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0066, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0066 10.30.3.202, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0066 10.30.3.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0067, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0067, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0068, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0068, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0068 10.30.3.204, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0068 10.30.3.204, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0069, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0069, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0069 10.30.3.205, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0069 10.30.3.205, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006a, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006a, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006a 10.30.3.206, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006a 10.30.3.206, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006b, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006b, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006b 10.30.3.207, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006b 10.30.3.207, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006c, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006c, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006c 10.30.3.208, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006c 10.30.3.208, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006d, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006d, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006d 10.30.3.209, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006d 10.30.3.209, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006e, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006e, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006e 10.30.3.210, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006e 10.30.3.210, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006f, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006f, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006f 10.30.3.211, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.006f 10.30.3.211, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0070, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0070, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0070 10.30.3.212, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0070 10.30.3.212, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0071, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0071, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0071 10.30.3.213, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0071 10.30.3.213, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0072, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0072, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0072 10.30.3.214, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0072 10.30.3.214, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0073, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0073, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0073 10.30.3.215, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0073 10.30.3.215, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0074, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0074, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0074 10.30.3.216, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0074 10.30.3.216, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0075, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0075, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0075 10.30.3.217, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0075 10.30.3.217, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0076, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0076, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0076 10.30.3.218, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0076 10.30.3.218, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0077, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0077, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0077 10.30.3.219, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0077 10.30.3.219, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0078, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0078, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0078 10.30.3.220, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0078 10.30.3.220, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0079, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0079, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0079 10.30.3.221, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0079 10.30.3.221, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007a, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007a, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007a 10.30.3.222, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007a 10.30.3.222, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007b, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007b, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007b 10.30.3.223, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007b 10.30.3.223, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007c, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007c, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007c 10.30.3.224, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007c 10.30.3.224, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007d, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007d, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007d 10.30.3.225, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007d 10.30.3.225, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007e, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007e, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007e 10.30.3.226, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007e 10.30.3.226, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007f, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007f, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007f 10.30.3.227, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.007f 10.30.3.227, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0080, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0080, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0080 10.30.3.228, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0080 10.30.3.228, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0081, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0081, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0081 10.30.3.229, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0081 10.30.3.229, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0082, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0082, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0082 10.30.3.230, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0082 10.30.3.230, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0083, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0083, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0083 10.30.3.231, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0083 10.30.3.231, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0084, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0084, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0084 10.30.3.232, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0084 10.30.3.232, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0085, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0085, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0085 10.30.3.233, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0085 10.30.3.233, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0086, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0086, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0086 10.30.3.234, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0086 10.30.3.234, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0087, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0087, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0087 10.30.3.235, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0087 10.30.3.235, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0088, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0088, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0088 10.30.3.236, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0088 10.30.3.236, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0089, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0089, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0089 10.30.3.237, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0089 10.30.3.237, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008a, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008a, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008a 10.30.3.238, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008a 10.30.3.238, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008b, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008b, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008b 10.30.3.239, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008b 10.30.3.239, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008c, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008c, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008c 10.30.3.240, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008c 10.30.3.240, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008d, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008d, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008d 10.30.3.241, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008d 10.30.3.241, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008e, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008e, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008e 10.30.3.242, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008e 10.30.3.242, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008f, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008f, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008f 10.30.3.243, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.008f 10.30.3.243, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0090, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0090, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0090 10.30.3.244, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0090 10.30.3.244, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0091, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0091, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0091 10.30.3.245, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0091 10.30.3.245, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0092, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0092, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0092 10.30.3.246, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0092 10.30.3.246, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0093, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0093, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0093 10.30.3.247, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0093 10.30.3.247, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0094, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0094, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0094 10.30.3.248, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0094 10.30.3.248, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0095, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0095, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0095 10.30.3.249, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0095 10.30.3.249, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0096, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0096, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0096 10.30.3.250, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0096 10.30.3.250, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 a266.0102.0001 10.30.3.103, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 a266.0102.0001 10.30.3.103, Route Distinguisher: 100.0.0.103:2303
 Paths: 2 available
  65206 65103 (Received from a RR-client)
    100.0.0.103 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, internal
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:02:00:00:01
      VNI: 2303 L3 VNI: 1001 ESI: 0000:0000:0000:0000:0000
  Local (Received from a RR-client)
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 1304 001b.0100.0004, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0004, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0004 10.30.4.203, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0004 10.30.4.203, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0097, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0097, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0097 10.30.4.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0097 10.30.4.201, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0098, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0098, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0098 10.30.4.202, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0098 10.30.4.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0099, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0099, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009a, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009a, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009a 10.30.4.204, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009a 10.30.4.204, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009b, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009b, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009b 10.30.4.205, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009b 10.30.4.205, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009c, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009c, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009c 10.30.4.206, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009c 10.30.4.206, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009d, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009d, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009d 10.30.4.207, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009d 10.30.4.207, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009e, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009e, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009e 10.30.4.208, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009e 10.30.4.208, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009f, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009f, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009f 10.30.4.209, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.009f 10.30.4.209, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a0, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a0, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a0 10.30.4.210, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a0 10.30.4.210, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a1, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a1, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a1 10.30.4.211, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a1 10.30.4.211, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a2, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a2, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a2 10.30.4.212, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a2 10.30.4.212, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a3, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a3, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a3 10.30.4.213, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a3 10.30.4.213, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a4, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a4, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a4 10.30.4.214, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a4 10.30.4.214, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a5, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a5, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a5 10.30.4.215, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a5 10.30.4.215, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a6, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a6, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a6 10.30.4.216, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a6 10.30.4.216, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a7, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a7, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a7 10.30.4.217, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a7 10.30.4.217, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a8, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a8, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a8 10.30.4.218, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a8 10.30.4.218, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a9, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a9, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a9 10.30.4.219, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00a9 10.30.4.219, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00aa, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00aa, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00aa 10.30.4.220, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00aa 10.30.4.220, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ab, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ab, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ab 10.30.4.221, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ab 10.30.4.221, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ac, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ac, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ac 10.30.4.222, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ac 10.30.4.222, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ad, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ad, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ad 10.30.4.223, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ad 10.30.4.223, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ae, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ae, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ae 10.30.4.224, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ae 10.30.4.224, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00af, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00af, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00af 10.30.4.225, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00af 10.30.4.225, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b0, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b0, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b0 10.30.4.226, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b0 10.30.4.226, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b1, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b1, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b1 10.30.4.227, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b1 10.30.4.227, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b2, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b2, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b2 10.30.4.228, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b2 10.30.4.228, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b3, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b3, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b3 10.30.4.229, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b3 10.30.4.229, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b4, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b4, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b4 10.30.4.230, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b4 10.30.4.230, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b5, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b5, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b5 10.30.4.231, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b5 10.30.4.231, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b6, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b6, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b6 10.30.4.232, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b6 10.30.4.232, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b7, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b7, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b7 10.30.4.233, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b7 10.30.4.233, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b8, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b8, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b8 10.30.4.234, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b8 10.30.4.234, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b9, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b9, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b9 10.30.4.235, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00b9 10.30.4.235, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ba, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ba, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ba 10.30.4.236, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00ba 10.30.4.236, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00bb, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00bb, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00bb 10.30.4.237, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00bb 10.30.4.237, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00bc, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00bc, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00bc 10.30.4.238, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00bc 10.30.4.238, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00bd, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00bd, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00bd 10.30.4.239, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00bd 10.30.4.239, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00be, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00be, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00be 10.30.4.240, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00be 10.30.4.240, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00bf, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00bf, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00bf 10.30.4.241, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00bf 10.30.4.241, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c0, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c0, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c0 10.30.4.242, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c0 10.30.4.242, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c1, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c1, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c1 10.30.4.243, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c1 10.30.4.243, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c2, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c2, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c2 10.30.4.244, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c2 10.30.4.244, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c3, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c3, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c3 10.30.4.245, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c3 10.30.4.245, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c4, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c4, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c4 10.30.4.246, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c4 10.30.4.246, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c5, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c5, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c5 10.30.4.247, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c5 10.30.4.247, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c6, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c6, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c6 10.30.4.248, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c6 10.30.4.248, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c7, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c7, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c7 10.30.4.249, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c7 10.30.4.249, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c8, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c8, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c8 10.30.4.250, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.00c8 10.30.4.250, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 a288.0103.0001 10.30.4.103, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 a288.0103.0001 10.30.4.103, Route Distinguisher: 100.0.0.103:2303
 Paths: 2 available
  65206 65103 (Received from a RR-client)
    100.0.0.103 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, internal
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:02:00:00:01
      VNI: 2304 L3 VNI: 1001 ESI: 0000:0000:0000:0000:0000
  Local (Received from a RR-client)
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
```

## show bgp evpn route-type imet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  Local (Received from a RR-client)
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  Local (Received from a RR-client)
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  Local (Received from a RR-client)
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:2301
 Paths: 1 available
  Local (Received from a RR-client)
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:1103
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1103
      PMSI Tunnel: Ingress Replication, MPLS Label: 1103, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.103, Route Distinguisher: 100.0.0.103:1103
 Paths: 1 available
  65206 65103 (Received from a RR-client)
    100.0.0.103 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, internal
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2299
      PMSI Tunnel: Ingress Replication, MPLS Label: 2299, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 100.0.0.103, Route Distinguisher: 100.0.0.103:2301
 Paths: 1 available
  65206 65103 (Received from a RR-client)
    100.0.0.103 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, internal
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2301
      PMSI Tunnel: Ingress Replication, MPLS Label: 2301, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1303 100.0.0.22, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  Local (Received from a RR-client)
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for imet 1303 100.0.0.56, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1303 100.0.0.103, Route Distinguisher: 100.0.0.103:2303
 Paths: 1 available
  65206 65103 (Received from a RR-client)
    100.0.0.103 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, internal
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2303
      PMSI Tunnel: Ingress Replication, MPLS Label: 2303, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 1303 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1303 100.0.0.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1304 100.0.0.22, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  Local (Received from a RR-client)
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for imet 1304 100.0.0.56, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1304 100.0.0.103, Route Distinguisher: 100.0.0.103:2303
 Paths: 1 available
  65206 65103 (Received from a RR-client)
    100.0.0.103 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, internal
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2304
      PMSI Tunnel: Ingress Replication, MPLS Label: 2304, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 1304 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1304 100.0.0.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.202
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
BGP routing table entry for ethernet-segment 0000:0000:0000:0111:0111 100.0.0.56, Route Distinguisher: 100.0.0.56:0
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:00:00:00:00:00:01
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.201, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:01:11:11:11 DF Election: Preference 100
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:01:11:11:11 DF Election: Preference 150
BGP routing table entry for ethernet-segment 0000:2222:2222:2222:1111 100.0.0.22, Route Distinguisher: 100.0.0.22:0
 Paths: 1 available
  Local (Received from a RR-client)
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ethernet-segment 0000:2222:2222:2222:1111 100.0.0.56, Route Distinguisher: 100.0.0.56:0
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:00:22:22:22:22:22
BGP routing table entry for ethernet-segment 0048:5648:5648:5648:5648 100.0.0.56, Route Distinguisher: 100.0.0.56:0
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:48:56:48:56:48:56
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
BGP routing table entry for ip-prefix 10.10.103.0/24, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.103.103/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local (Received from a RR-client)
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.103/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.201/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.201/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.201/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.202/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.202/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.202/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.203/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.204/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.204/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.204/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.205/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.205/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.205/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.206/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.206/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.206/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.207/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.207/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.207/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.208/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.208/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.208/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.209/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.209/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.209/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.210/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.210/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.210/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.211/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.211/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.211/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.212/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.212/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.212/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.213/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.213/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.213/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.214/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.214/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.214/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.215/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.215/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.215/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.216/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.216/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.216/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.217/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.217/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.217/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.218/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.218/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.218/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.219/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.219/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.219/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.220/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.220/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.220/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.221/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.221/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.221/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.222/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.222/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.222/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.223/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.223/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.223/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.224/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.224/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.224/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.225/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.225/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.225/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.226/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.226/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.226/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.227/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.227/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.227/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.228/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.228/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.228/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.229/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.229/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.229/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.230/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.230/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.230/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.231/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.231/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.231/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.232/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.232/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.232/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.233/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.233/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.233/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.234/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.234/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.234/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.235/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.235/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.235/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.236/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.236/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.236/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.237/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.237/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.237/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.238/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.238/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.238/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.239/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.239/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.239/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.240/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.240/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.240/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.241/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.241/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.241/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.242/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.242/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.242/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.243/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.243/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.243/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.244/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.244/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.244/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.245/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.245/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.245/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.246/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.246/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.246/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.247/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.247/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.247/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.248/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.248/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.248/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.249/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.249/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.249/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.250/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.250/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.250/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.254/32, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local (Received from a RR-client)
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.103/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.201/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.201/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.201/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.202/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.202/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.202/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.203/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.204/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.204/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.204/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.205/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.205/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.205/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.206/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.206/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.206/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.207/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.207/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.207/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.208/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.208/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.208/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.209/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.209/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.209/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.210/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.210/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.210/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.211/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.211/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.211/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.212/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.212/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.212/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.213/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.213/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.213/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.214/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.214/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.214/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.215/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.215/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.215/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.216/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.216/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.216/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.217/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.217/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.217/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.218/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.218/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.218/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.219/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.219/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.219/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.220/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.220/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.220/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.221/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.221/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.221/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.222/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.222/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.222/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.223/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.223/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.223/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.224/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.224/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.224/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.225/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.225/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.225/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.226/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.226/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.226/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.227/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.227/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.227/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.228/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.228/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.228/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.229/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.229/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.229/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.230/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.230/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.230/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.231/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.231/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.231/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.232/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.232/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.232/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.233/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.233/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.233/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.234/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.234/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.234/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.235/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.235/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.235/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.236/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.236/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.236/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.237/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.237/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.237/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.238/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.238/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.238/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.239/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.239/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.239/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.240/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.240/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.240/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.241/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.241/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.241/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.242/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.242/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.242/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.243/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.243/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.243/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.244/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.244/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.244/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.245/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.245/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.245/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.246/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.246/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.246/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.247/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.247/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.247/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.248/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.248/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.248/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.249/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.249/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.249/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.250/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.250/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.250/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.103/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.201/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.201/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.201/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.202/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.202/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.202/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.203/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.204/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.204/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.204/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.205/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.205/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.205/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.206/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.206/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.206/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.207/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.207/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.207/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.208/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.208/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.208/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.209/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.209/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.209/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.210/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.210/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.210/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.211/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.211/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.211/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.212/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.212/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.212/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.213/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.213/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.213/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.214/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.214/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.214/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.215/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.215/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.215/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.216/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.216/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.216/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.217/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.217/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.217/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.218/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.218/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.218/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.219/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.219/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.219/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.220/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.220/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.220/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.221/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.221/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.221/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.222/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.222/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.222/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.223/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.223/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.223/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.224/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.224/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.224/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.225/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.225/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.225/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.226/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.226/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.226/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.227/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.227/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.227/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.228/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.228/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.228/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.229/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.229/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.229/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.230/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.230/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.230/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.231/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.231/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.231/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.232/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.232/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.232/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.233/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.233/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.233/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.234/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.234/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.234/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.235/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.235/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.235/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.236/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.236/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.236/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.237/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.237/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.237/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.238/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.238/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.238/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.239/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.239/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.239/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.240/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.240/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.240/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.241/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.241/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.241/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.242/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.242/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.242/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.243/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.243/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.243/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.244/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.244/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.244/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.245/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.245/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.245/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.246/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.246/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.246/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.247/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.247/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.247/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.248/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.248/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.248/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.249/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.249/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.249/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.250/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.250/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.250/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.204/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.204/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
```

## show bgp evpn route-type smet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
```

## show bgp evpn route-type spmsi detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
```

## show bgp evpn arp

```text
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

 C        20.22.205.0/24
           directly connected, Ethernet49/3
 I L2     20.22.206.0/24 [115/20]
           via 20.22.205.22, Ethernet49/3
 C        20.45.205.0/24
           directly connected, Ethernet50/3
 C        20.46.205.0/24
           directly connected, Ethernet50/4
 C        20.56.205.0/24
           directly connected, Ethernet49/1
 I L2     20.200.201.0/24 [115/10]
           via 20.201.205.201, Ethernet50/1
 I L2     20.200.202.0/24 [115/10]
           via 20.202.205.202, Ethernet50/2
 C        20.201.205.0/24
           directly connected, Ethernet50/1
 C        20.202.205.0/24
           directly connected, Ethernet50/2
 I L2     100.0.0.22/32 [115/10]
           via 20.22.205.22, Ethernet49/3
 I L2     100.0.0.56/32 [115/10]
           via 20.56.205.56, Ethernet49/1
 I L2     100.0.0.201/32 [115/10]
           via 20.201.205.201, Ethernet50/1
 I L2     100.0.0.202/32 [115/10]
           via 20.202.205.202, Ethernet50/2
 C        100.0.0.205/32
           directly connected, Loopback0

```

## show ip arp

```text
Address         Age (sec)  Hardware Addr   Interface
20.56.205.56      0:00:06  407c.7dc4.ab98  Ethernet49/1
20.22.205.22      0:00:18  c407.780a.9f31  Ethernet49/3
20.201.205.201    0:00:07  2cdd.e90b.2283  Ethernet50/1
20.202.205.202    0:00:03  2cdd.e90b.25b7  Ethernet50/2
20.45.205.45      3:36:20  6c31.0e7b.8b87  Ethernet50/3
20.46.205.46      2:14:51  6c31.0eb7.505f  Ethernet50/4
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

 C        20.22.205.0/24
           directly connected, Ethernet49/3
 I L2     20.22.206.0/24 [115/20]
           via 20.22.205.22, Ethernet49/3
 C        20.45.205.0/24
           directly connected, Ethernet50/3
 C        20.46.205.0/24
           directly connected, Ethernet50/4
 C        20.56.205.0/24
           directly connected, Ethernet49/1
 I L2     20.200.201.0/24 [115/10]
           via 20.201.205.201, Ethernet50/1
 I L2     20.200.202.0/24 [115/10]
           via 20.202.205.202, Ethernet50/2
 C        20.201.205.0/24
           directly connected, Ethernet50/1
 C        20.202.205.0/24
           directly connected, Ethernet50/2
 I L2     100.0.0.22/32 [115/10]
           via 20.22.205.22, Ethernet49/3
 I L2     100.0.0.56/32 [115/10]
           via 20.56.205.56, Ethernet49/1
 I L2     100.0.0.201/32 [115/10]
           via 20.201.205.201, Ethernet50/1
 I L2     100.0.0.202/32 [115/10]
           via 20.202.205.202, Ethernet50/2
 C        100.0.0.205/32
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

```

## show ip arp vrf all

```text

VRF: default
Address         Age (sec)  Hardware Addr   Interface
20.56.205.56      0:00:06  407c.7dc4.ab98  Ethernet49/1
20.22.205.22      0:00:19  c407.780a.9f31  Ethernet49/3
20.201.205.201    0:00:08  2cdd.e90b.2283  Ethernet50/1
20.202.205.202    0:00:03  2cdd.e90b.25b7  Ethernet50/2
20.45.205.45      3:36:21  6c31.0e7b.8b87  Ethernet50/3
20.46.205.46      2:14:52  6c31.0eb7.505f  Ethernet50/4

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.21.47     0:00:17  5c5a.c7ff.8a0a  Management1
192.168.21.50     0:03:57  a84f.b1a5.5221  Management1
192.168.21.59     0:02:13  6607.f5d1.ae16  Management1
```

## show vxlan address-table

```text
          Vxlan Mac Address Table
----------------------------------------------------------------------

VLAN  Mac Address     Type      Prt  VTEP             Moves   Last Move
----  -----------     ----      ---  ----             -----   ---------
Total Remote Mac Addresses for this criterion: 0
```

## show vxlan vni

```text
```

## show mac address-table

```text
          Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports      Moves   Last Move
----    -----------       ----        -----      -----   ---------
   1    5c5a.c773.4ac0    DYNAMIC     Et17       1       1 day, 0:50:55 ago
  40    246c.8474.8de0    DYNAMIC     Et15       1       1 day, 0:50:53 ago
 203    001b.0100.0001    DYNAMIC     Et25       1       1:45:42 ago
 203    001b.0100.0002    DYNAMIC     Et25       1       1:44:40 ago
 203    001b.0100.0003    DYNAMIC     Et25       1       1:44:40 ago
 203    001b.0100.0004    DYNAMIC     Et25       1       1:44:40 ago
 203    0056.5656.5656    DYNAMIC     Po200      1       15:57:43 ago
 203    3838.a621.e82f    DYNAMIC     Po200      1       1 day, 0:50:53 ago
 203    985d.82a2.04f9    DYNAMIC     Po200      1       16:48:21 ago
 203    a222.0100.0001    DYNAMIC     Po200      1       0:04:34 ago
 203    a244.0101.0001    DYNAMIC     Po200      1       0:03:14 ago
 203    a266.0102.0001    DYNAMIC     Po200      1       0:03:14 ago
 203    a288.0103.0001    DYNAMIC     Po200      1       0:03:14 ago
Total Mac Addresses for this criterion: 13

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
0056.5656.5656, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
985d.82a2.04f9, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
3838.a621.e82f, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
5c5a.c773.4ac0, VLAN 1, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet17
001b.0100.0004, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
001b.0100.0002, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
a222.0100.0001, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
a288.0103.0001, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0001, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
a266.0102.0001, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0003, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
246c.8474.8de0, VLAN 40, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet15
a244.0101.0001, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
```

## show vxlan flood vtep domain local

```text
          VXLAN Flood VTEP Table
--------------------------------------------------------------------------------

VLANS                            Ip Address
-----------------------------   ------------------------------------------------
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
Router identifier 100.0.0.205, local AS number 65205
```

## show bgp evpn instance

```text
```

## show interfaces counters rates | nz

```text
Port      Name           Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Et3       ANET-203        0:01      0.6   0.0%        1      0.6   0.0%        1
Et4       ANET-204        0:01      1.7   0.0%        3      1.7   0.0%        3
Et25      Keysight-Gen    0:05      2.4   0.0%        4      2.5   0.0%        4
Et49/1    Nokia-GW WAN    0:05      3.8   0.0%        4      3.7   0.0%        4
Et50/1    ANET201-GW WAN  0:05      1.9   0.0%        2      3.8   0.0%        4
Et50/2    ANET202-GW WAN  0:05      1.9   0.0%        2      0.0   0.0%        0
Ma1                       0:05      0.0   0.0%        0      0.3   0.0%        0
Po200                     0:05      2.3   0.0%        3      2.2   0.0%        3
```

