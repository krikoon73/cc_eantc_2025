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
  100.0.0.22  4 65205           6288     32750    0    0 01:56:39 Estab   15     15
  100.0.0.201 4 65205            522      1170    0    0 01:56:39 Estab   27     27
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
BGP routing table entry for auto-discovery 1303 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
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
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:2
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.22:2301
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 2301
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.22:2301
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
BGP routing table entry for mac-ip 001b.0100.0002, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
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
BGP routing table entry for mac-ip 00cc.cccc.bbbb, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip a244.0101.0001 10.30.1.103, Route Distinguisher: 100.0.0.103:2301
 Paths: 1 available
  65206 65103 (Received from a RR-client)
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1301 L3 VNI: 1000 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 001b.0100.0003, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1303 a266.0102.0001 10.30.3.103, Route Distinguisher: 100.0.0.103:2303
 Paths: 1 available
  65206 65103 (Received from a RR-client)
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 2303 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 001b.0100.0004, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0004 10.30.4.203, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 a288.0103.0001 10.30.4.103, Route Distinguisher: 100.0.0.103:2303
 Paths: 1 available
  65206 65103 (Received from a RR-client)
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 2304 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
```

## show bgp evpn route-type imet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
      PMSI Tunnel: Ingress Replication, MPLS Label: 1022, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:2301
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 2301
      PMSI Tunnel: Ingress Replication, MPLS Label: 2301, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1303 100.0.0.22, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 1303 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1304 100.0.0.22, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 1304 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.201
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.201, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:11:11:11:11:11 DF Election: Preference 5000
BGP routing table entry for ethernet-segment 0000:2222:2222:2222:1111 100.0.0.22, Route Distinguisher: 100.0.0.22:0
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:22:22:22:22:22 DF Election: Modulus-based
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.205, local AS number 65205
BGP routing table entry for ip-prefix 10.10.103.0/24, Route Distinguisher: 100.0.0.103:1103
 Paths: 1 available
  65206 65103 (Received from a RR-client)
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
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
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.254/32, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local (Received from a RR-client)
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65203 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
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
BGP routing table entry for ip-prefix 100.0.1.204/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65000 65204 (Received from a RR-client)
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
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
 I L2     20.40.201.0/24 [115/10]
           via 20.201.205.201, Ethernet50/1
 I L2     20.200.201.0/24 [115/10]
           via 20.201.205.201, Ethernet50/1
 C        20.201.205.0/24
           directly connected, Ethernet50/1
 I L2     100.0.0.22/32 [115/10]
           via 20.22.205.22, Ethernet49/3
 I L2     100.0.0.201/32 [115/10]
           via 20.201.205.201, Ethernet50/1
 C        100.0.0.205/32
           directly connected, Loopback0

```

## show ip arp

```text
Address         Age (sec)  Hardware Addr   Interface
20.22.205.22      0:00:08  c407.780a.9f31  Ethernet49/3
20.201.205.201    0:00:48  2cdd.e90b.2283  Ethernet50/1
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
 I L2     20.40.201.0/24 [115/10]
           via 20.201.205.201, Ethernet50/1
 I L2     20.200.201.0/24 [115/10]
           via 20.201.205.201, Ethernet50/1
 C        20.201.205.0/24
           directly connected, Ethernet50/1
 I L2     100.0.0.22/32 [115/10]
           via 20.22.205.22, Ethernet49/3
 I L2     100.0.0.201/32 [115/10]
           via 20.201.205.201, Ethernet50/1
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
20.22.205.22      0:00:08  c407.780a.9f31  Ethernet49/3
20.201.205.201    0:00:48  2cdd.e90b.2283  Ethernet50/1

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.21.47     0:02:54  5c5a.c7ff.8a0a  Management1
192.168.21.50     0:01:23  a84f.b1a5.5221  Management1
192.168.21.59     0:04:26  6607.f5d1.ae16  Management1
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
   1    5c5a.c773.4ac0    DYNAMIC     Et17       1       1 day, 10:26:40 ago
 203    001b.0100.0001    DYNAMIC     Et25       1       0:00:28 ago
 203    001b.0100.0002    DYNAMIC     Et25       1       0:30:26 ago
 203    001b.0100.0003    DYNAMIC     Et25       1       0:00:53 ago
 203    00aa.aaaa.aaaa    DYNAMIC     Po200      1       0:50:15 ago
 203    3838.a621.e82f    DYNAMIC     Po200      1       1 day, 10:26:38 ago
 203    985d.82a2.04f9    DYNAMIC     Po200      1       1 day, 2:24:06 ago
 203    a222.0100.0001    DYNAMIC     Po200      1       0:06:02 ago
 203    a244.0101.0001    DYNAMIC     Po200      1       0:06:49 ago
Total Mac Addresses for this criterion: 9

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
985d.82a2.04f9, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
3838.a621.e82f, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
5c5a.c773.4ac0, VLAN 1, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet17
00aa.aaaa.aaaa, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0002, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
a222.0100.0001, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Port-Channel200
001b.0100.0001, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
001b.0100.0003, VLAN 203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet25
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
Et4       ANET-204        0:01      0.6   0.0%        1      0.6   0.0%        1
Et25      Keysight-Gen    0:05      0.6   0.0%        0      0.6   0.0%        0
Et49/3    H3C22-GW WAN    0:05      1.0   0.0%        0      0.9   0.0%        0
Et50/1    ANET201-GW WAN  0:05      0.9   0.0%        0      1.0   0.0%        0
Ma1                       0:05      0.0   0.0%        0      1.4   0.1%        0
Po200                     0:05      0.6   0.0%        0      0.6   0.0%        0
```

