# Test results for PE15-T3-206

## show hostname

```text
Hostname: P15-T3-206
FQDN:     P15-T3-206.eantc.de
```

## show ip bgp summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.206, local AS number 65206
Neighbor Status Codes: m - Under maintenance
  Neighbor       V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  20.22.206.22   4 65022            147       159    0    0 02:09:01 Estab   1      1
  20.56.200.56   4 65056           2419      2879    0    0 20:07:01 Estab   1      1
  20.103.206.103 4 65103             75        90    0    0 00:35:35 Estab   1      1
  30.4.206.30    4 65304           2775      2984    0    0 20:50:23 Estab   1      1
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.206, local AS number 65206
Neighbor Status Codes: m - Under maintenance
  Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  100.0.0.22  4 65022           5254      2977    0    0 00:42:43 Estab   91     0
  100.0.0.56  4 65056           9488      3427    0    0 19:57:32 Estab   166    166
  100.0.0.103 4 65103             84       113    0    0 00:35:34 Estab   8      8
  100.0.30.4  4 65304           2749      4820    0    0 20:38:36 Estab   0      0
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.206, local AS number 65206
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1301
 Paths: 2 available
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.202:1301
 Paths: 2 available
  65056 65205
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 1303 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1303
 Paths: 2 available
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 1303 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.202:1303
 Paths: 2 available
  65056 65205
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 1304 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1303
 Paths: 2 available
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 1304 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.202:1303
 Paths: 2 available
  65056 65205
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:2
 Paths: 2 available
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1301 Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.202:2
 Paths: 2 available
  65056 65205
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1301 Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.22:2301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2301
BGP routing table entry for auto-discovery 0 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 1303 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2303
BGP routing table entry for auto-discovery 1303 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.22:2301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:1301
 Paths: 2 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:1303
 Paths: 2 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:51301
 Paths: 2 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:51303
 Paths: 2 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0 0030:0903:0405:0607:08cc, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 Route-Origin-AS:56:56
      VNI: 21008
BGP routing table entry for auto-discovery 0 0030:0903:0405:0607:08cc, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302 Route-Origin-AS:56:56
      VNI: 21056
BGP routing table entry for auto-discovery 2303 0030:0903:0405:0607:08cc, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56
      VNI: 368
BGP routing table entry for auto-discovery 2304 0030:0903:0405:0607:08cc, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56
      VNI: 384
BGP routing table entry for auto-discovery 0030:0903:0405:0607:08cc, Route Distinguisher: 100.0.30.9:0
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2033:2033 Route-Target-AS:2301:2301 Route-Target-AS:2302:2302 Route-Target-AS:2303:2303 Route-Origin-AS:56:56 EvpnEsiLabel:31
      VNI: 0
BGP routing table entry for auto-discovery 0 0048:5648:5648:5648:5648, Route Distinguisher: 100.0.3.48:4558
 Paths: 1 available
  65056 64512
    100.0.3.48 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:4558:4558 Route-Origin-AS:56:56
      VNI: 408368
BGP routing table entry for auto-discovery 0048:5648:5648:5648:5648, Route Distinguisher: 100.0.3.48:1
 Paths: 1 available
  65056 64512
    100.0.3.48 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:4558:4558 Route-Origin-AS:56:56 EvpnEsiLabel:25500
      VNI: 0
BGP routing table entry for auto-discovery 0500:00fc:0000:0000:0000, Route Distinguisher: 100.0.30.9:0
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 Route-Target-AS:2302:2302 Route-Origin-AS:56:56 EvpnEsiLabel:3152
      VNI: 0
BGP routing table entry for auto-discovery 0500:00fc:0000:0008:ff00, Route Distinguisher: 100.0.30.9:0
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56 EvpnEsiLabel:3150
      VNI: 0
BGP routing table entry for auto-discovery 0500:00fc:0000:0009:0000, Route Distinguisher: 100.0.30.9:0
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56 EvpnEsiLabel:3151
      VNI: 0
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.206, local AS number 65206
BGP routing table entry for mac-ip 000c.29a8.0a35, Route Distinguisher: 100.0.3.48:4558
 Paths: 1 available
  65056 64512
    100.0.3.48 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:4558:4558 Route-Origin-AS:56:56 Route-Origin-IP:100.0.3.48:4558
      VNI: 408368 ESI: 0048:5648:5648:5648:5648
BGP routing table entry for mac-ip 001b.0100.0002, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 001b.0100.0002, Route Distinguisher: 100.0.0.201:1301
 Paths: 2 available
  65056 65205 65000 65204
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 001b.0100.0002, Route Distinguisher: 100.0.0.202:1301
 Paths: 2 available
  65056 65205 65000 65204
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 001b.0100.0002, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 Route-Origin-AS:56:56
      VNI: 21008 ESI: 0030:0903:0405:0607:08cc
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.201, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.201, Route Distinguisher: 100.0.0.202:1301
 Paths: 2 available
  65056 65205 65000 65204
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.203, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.203, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 001b.0100.0002 10.30.1.203, Route Distinguisher: 100.0.0.202:1301
 Paths: 2 available
  65056 65205 65000 65204
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 001b.0100.0002 20.30.1.33, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 Route-Origin-AS:56:56
      VNI: 21008 ESI: 0030:0903:0405:0607:08cc
BGP routing table entry for mac-ip 001b.0100.0003, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302 Route-Origin-AS:56:56
      VNI: 21056 ESI: 0030:0903:0405:0607:08cc
BGP routing table entry for mac-ip 001b.0100.0003 20.30.2.33, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302 Route-Origin-AS:56:56
      VNI: 21056 ESI: 0030:0903:0405:0607:08cc
BGP routing table entry for mac-ip 0056.5656.5656 10.10.103.254, Route Distinguisher: 100.0.0.56:1103
 Paths: 2 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1103 ESI: 0000:0000:0000:0000:0000
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 0056.5656.5656 10.30.1.254, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 0056.5656.5656 10.30.1.254, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 0056.5656.5656 10.30.2.254, Route Distinguisher: 100.0.0.56:1302
 Paths: 2 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 Route-Origin-AS:56:56 EvpnMacMobility:sticky
      VNI: 21008 ESI: 0500:00fc:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302 Route-Origin-AS:56:56 EvpnMacMobility:sticky
      VNI: 21056 ESI: 0500:00fc:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.103.254, Route Distinguisher: 100.0.0.56:1103
 Paths: 2 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1103 ESI: 0000:0000:0000:0000:0000
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.203.254, Route Distinguisher: 100.0.0.56:1203
 Paths: 2 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1203 ESI: 0000:0000:0000:0000:0000
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 20.30.1.254, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 Route-Origin-AS:56:56
      VNI: 21008 ESI: 0500:00fc:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 20.30.2.254, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302 Route-Origin-AS:56:56
      VNI: 21056 ESI: 0500:00fc:0000:0000:0000
BGP routing table entry for mac-ip 00cc.cccc.bbbb, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 00cc.cccc.bbbb, Route Distinguisher: 100.0.0.201:1301
 Paths: 2 available
  65056 65205 65000 65203
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 00cc.cccc.bbbb, Route Distinguisher: 100.0.0.202:1301
 Paths: 2 available
  65056 65205 65000 65203
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip a244.0101.0001 10.30.1.103, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip a244.0101.0001 10.30.1.103, Route Distinguisher: 100.0.0.103:2301
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (192.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:02:00:00:01
      VNI: 2301 L3 VNI: 1001 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip b0a6.5130.362b, Route Distinguisher: 100.0.3.45:4568
 Paths: 1 available
  65056 64512
    100.0.3.45 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:4558:4558 Route-Origin-AS:56:56 Route-Origin-IP:100.0.3.45:4558
      VNI: 449920 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip e4f2.7cef.a505, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 Route-Origin-AS:56:56 EvpnMacMobility:sticky
      VNI: 21008 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip e4f2.7cef.a505, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302 Route-Origin-AS:56:56 EvpnMacMobility:sticky
      VNI: 21056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip e4f2.7cef.a505 20.30.1.200, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 Route-Origin-AS:56:56 EvpnMacMobility:sticky
      VNI: 21008 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip e4f2.7cef.a505 20.30.2.200, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302 Route-Origin-AS:56:56 EvpnMacMobility:sticky
      VNI: 21056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip f87a.4118.8af6, Route Distinguisher: 100.0.3.48:4558
 Paths: 1 available
  65056 64512
    100.0.3.48 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:4558:4558 Route-Origin-AS:56:56 Route-Origin-IP:100.0.3.48:4558
      VNI: 408368 ESI: 0048:5648:5648:5648:5648
BGP routing table entry for mac-ip f87a.416d.d0ec, Route Distinguisher: 100.0.3.48:4558
 Paths: 1 available
  65056 64512
    100.0.3.48 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:4558:4558 Route-Origin-AS:56:56 Route-Origin-IP:100.0.3.48:4558
      VNI: 408368 ESI: 0048:5648:5648:5648:5648
BGP routing table entry for mac-ip 1303 001b.0100.0003, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2303 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 001b.0100.0003, Route Distinguisher: 100.0.0.201:1303
 Paths: 2 available
  65056 65205 65000 65203
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 1303 001b.0100.0003, Route Distinguisher: 100.0.0.202:1303
 Paths: 2 available
  65056 65205 65000 65203
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2303 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203, Route Distinguisher: 100.0.0.202:1303
 Paths: 2 available
  65056 65205 65000 65203
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1303 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2303 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2303 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 1303 a266.0102.0001 10.30.3.103, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 1303 a266.0102.0001 10.30.3.103, Route Distinguisher: 100.0.0.103:2303
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (192.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:02:00:00:01
      VNI: 2303 L3 VNI: 1001 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 001b.0100.0004, Route Distinguisher: 100.0.0.56:51304
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 001b.0100.0004, Route Distinguisher: 100.0.0.201:1303
 Paths: 2 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
  65056 65205 65000 65204
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0004, Route Distinguisher: 100.0.0.202:1303
 Paths: 2 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
  65056 65205 65000 65204
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 1304 001b.0100.0004 10.30.4.203, Route Distinguisher: 100.0.0.56:51304
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 001b.0100.0004 10.30.4.203, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 1304 001b.0100.0004 10.30.4.203, Route Distinguisher: 100.0.0.202:1303
 Paths: 2 available
  65056 65205 65000 65204
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1304 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254, Route Distinguisher: 100.0.0.56:51304
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.0.56:51304
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 a288.0103.0001 10.30.4.103, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 1304 a288.0103.0001 10.30.4.103, Route Distinguisher: 100.0.0.103:2303
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (192.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:02:00:00:01
      VNI: 2304 L3 VNI: 1001 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2303 001b.0100.0004, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56
      VNI: 368 ESI: 0030:0903:0405:0607:08cc
BGP routing table entry for mac-ip 2303 001b.0100.0004 20.30.3.33, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56
      VNI: 368 ESI: 0030:0903:0405:0607:08cc
BGP routing table entry for mac-ip 2303 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56 EvpnMacMobility:sticky
      VNI: 368 ESI: 0500:00fc:0000:0008:ff00
BGP routing table entry for mac-ip 2303 00aa.aaaa.aaaa 20.30.3.254, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56
      VNI: 368 ESI: 0500:00fc:0000:0008:ff00
BGP routing table entry for mac-ip 2303 e4f2.7cef.a505, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56 EvpnMacMobility:sticky
      VNI: 368 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2303 e4f2.7cef.a505 20.30.3.200, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56 EvpnMacMobility:sticky
      VNI: 368 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2304 001b.0100.0005, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56
      VNI: 384 ESI: 0030:0903:0405:0607:08cc
BGP routing table entry for mac-ip 2304 001b.0100.0005 20.30.4.33, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56
      VNI: 384 ESI: 0030:0903:0405:0607:08cc
BGP routing table entry for mac-ip 2304 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56 EvpnMacMobility:sticky
      VNI: 384 ESI: 0500:00fc:0000:0009:0000
BGP routing table entry for mac-ip 2304 00aa.aaaa.aaaa 20.30.4.254, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56
      VNI: 384 ESI: 0500:00fc:0000:0009:0000
BGP routing table entry for mac-ip 2304 e4f2.7cef.a505, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56 EvpnMacMobility:sticky
      VNI: 384 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2304 e4f2.7cef.a505 20.30.4.200, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56 EvpnMacMobility:sticky
      VNI: 384 ESI: 0000:0000:0000:0000:0000
```

## show bgp evpn route-type imet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.206, local AS number 65206
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:2301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:1103
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1103
      PMSI Tunnel: Ingress Replication, MPLS Label: 1103, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2301
      PMSI Tunnel: Ingress Replication, MPLS Label: 2301, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.103, Route Distinguisher: 100.0.0.103:1103
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (192.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1103:1103 TunnelEncap:tunnelTypeVxlan
      VNI: 2299
      PMSI Tunnel: Ingress Replication, MPLS Label: 2299, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 100.0.0.103, Route Distinguisher: 100.0.0.103:2301
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (192.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 2301
      PMSI Tunnel: Ingress Replication, MPLS Label: 2301, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65056 65205
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 100.0.3.45, Route Distinguisher: 100.0.3.45:4568
 Paths: 1 available
  65056 64512
    100.0.3.45 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:4558:4558 Route-Origin-AS:56:56 L2 Attributes: none Multicast Flags: IGMP proxy
      VNI: 384065
      PMSI Tunnel: Ingress Replication, MPLS Label: 384065, Leaf Information Required: false, Tunnel ID: 100.0.3.45
BGP routing table entry for imet 100.0.3.48, Route Distinguisher: 100.0.3.48:4558
 Paths: 1 available
  65056 64512
    100.0.3.48 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:4558:4558 Route-Origin-AS:56:56 L2 Attributes: none Multicast Flags: IGMP proxy
      VNI: 384049
      PMSI Tunnel: Ingress Replication, MPLS Label: 384049, Leaf Information Required: false, Tunnel ID: 100.0.3.48
BGP routing table entry for imet 100.0.30.9, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 Route-Origin-AS:56:56
      VNI: 15738097
      PMSI Tunnel: Ingress Replication, MPLS Label: 15738097, Leaf Information Required: false, Tunnel ID: 100.0.30.9
BGP routing table entry for imet 100.0.30.9, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302 Route-Origin-AS:56:56
      VNI: 15738113
      PMSI Tunnel: Ingress Replication, MPLS Label: 15738113, Leaf Information Required: false, Tunnel ID: 100.0.30.9
BGP routing table entry for imet 1303 100.0.0.22, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for imet 1303 100.0.0.56, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2303
      PMSI Tunnel: Ingress Replication, MPLS Label: 2303, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1303 100.0.0.103, Route Distinguisher: 100.0.0.103:2303
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (192.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 2303
      PMSI Tunnel: Ingress Replication, MPLS Label: 2303, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 1303 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1303 100.0.0.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65056 65205
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1304 100.0.0.22, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for imet 1304 100.0.0.56, Route Distinguisher: 100.0.0.56:51304
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2304
      PMSI Tunnel: Ingress Replication, MPLS Label: 2304, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1304 100.0.0.103, Route Distinguisher: 100.0.0.103:2303
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (192.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 2304
      PMSI Tunnel: Ingress Replication, MPLS Label: 2304, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 1304 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1304 100.0.0.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65056 65205
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 2303 100.0.30.9, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56
      VNI: 15737889
      PMSI Tunnel: Ingress Replication, MPLS Label: 15737889, Leaf Information Required: false, Tunnel ID: 100.0.30.9
BGP routing table entry for imet 2304 100.0.30.9, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 Route-Origin-AS:56:56
      VNI: 15737905
      PMSI Tunnel: Ingress Replication, MPLS Label: 15737905, Leaf Information Required: false, Tunnel ID: 100.0.30.9
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.206, local AS number 65206
BGP routing table entry for ethernet-segment 0000:0000:0000:0111:0111 100.0.0.56, Route Distinguisher: 100.0.0.56:0
 Paths: 2 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:00:00:00:00:00:01
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.201, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ethernet-segment 0000:2222:2222:2222:1111 100.0.0.22, Route Distinguisher: 100.0.0.22:0
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ethernet-segment 0000:2222:2222:2222:1111 100.0.0.56, Route Distinguisher: 100.0.0.56:0
 Paths: 2 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:00:22:22:22:22:22
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ethernet-segment 0048:5648:5648:5648:5648 100.0.0.56, Route Distinguisher: 100.0.0.56:0
 Paths: 2 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:48:56:48:56:48:56
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ethernet-segment 0048:5648:5648:5648:5648 100.0.3.48, Route Distinguisher: 100.0.3.48:0
 Paths: 1 available
  65056 64512
    100.0.3.48 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:48:56:48:56:48:56 DF Election: Modulus-based
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.206, local AS number 65206
BGP routing table entry for ip-prefix 10.10.103.0/24, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.10.103.0/24, Route Distinguisher: 100.0.0.22:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.10.103.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.10.103.0/24, Route Distinguisher: 100.0.0.103:1103
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (192.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:02:00:00:01
      VNI: 1001
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.22:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65056 65205
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.22:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056 65000 65204
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65056 65205 65000 65204
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65056 65205 65000 65203
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.203/32, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.10.203.203/32, Route Distinguisher: 100.0.0.22:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.10.203.203/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056 65000 65204
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65056 65205 65000 65204
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65056 65205 65000 65204
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.22:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65056 65205
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.103/32, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.1.103/32, Route Distinguisher: 100.0.0.22:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.1.103/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.1.201/32, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.1.201/32, Route Distinguisher: 100.0.0.22:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.1.201/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.1.201/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65056 65205 65000 65204
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.201/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65056 65205 65000 65204
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.203/32, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.1.203/32, Route Distinguisher: 100.0.0.22:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.1.203/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.1.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65056 65205 65000 65204
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65056 65205 65000 65204
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.22:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65056 65205
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.22:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65056 65205
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.103/32, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.3.103/32, Route Distinguisher: 100.0.0.22:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.3.103/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.3.203/32, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.3.203/32, Route Distinguisher: 100.0.0.22:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.3.203/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.3.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65056 65205 65000 65203
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65056 65205 65000 65203
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.22:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65056 65205
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.103/32, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.4.103/32, Route Distinguisher: 100.0.0.22:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.4.103/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.4.203/32, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.4.203/32, Route Distinguisher: 100.0.0.22:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 10.30.4.203/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.4.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65056 65205 65000 65204
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65056 65205 65000 65204
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 20.10.33.0/24, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.10.33.33/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.10.33.200/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.10.33.254/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.30.1.0/24, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.30.1.33/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.30.1.200/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.30.1.254/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.30.2.0/24, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.30.2.33/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.30.2.200/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.30.2.254/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.30.3.0/24, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.30.3.33/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.30.3.200/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.30.3.254/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.30.4.0/24, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.30.4.33/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.30.4.200/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 20.30.4.254/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Origin-AS:56:56
      VNI: 448
BGP routing table entry for ip-prefix 100.0.1.203/32, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 100.0.1.203/32, Route Distinguisher: 100.0.0.22:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 100.0.1.203/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056 65000 65203
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65056 65205 65000 65203
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.203/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65056 65205 65000 65203
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.204/32, Route Distinguisher: 100.0.0.22:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 100.0.1.204/32, Route Distinguisher: 100.0.0.22:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 100.0.1.204/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056 65000 65204
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.204/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65056 65205 65000 65204
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.204/32, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65056 65205 65000 65204
    100.0.0.202 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
      D-PATH: 1:1:EVPN
```

## show bgp evpn route-type smet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.206, local AS number 65206
BGP routing table entry for smet (S, G): (*, 239.0.0.60) originating IP: 100.0.3.48, Route Distinguisher: 100.0.3.48:4558
 Paths: 1 available
  65056 64512
    100.0.3.48 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:4558:4558 Route-Origin-AS:56:56
      Multicast Flags: exclude
```

## show bgp evpn route-type spmsi detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.206, local AS number 65206
```

## show bgp evpn arp

```text
VLAN  Label  Encap IP                 MAC             Tunnel Endpoint    Seq#
----- ------ ----- ------------------ --------------- ------------------ ----
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

 C        20.22.206.0/24
           directly connected, Ethernet49/3
 C        20.56.200.0/24
           directly connected, Ethernet49/2
 C        20.103.206.0/24
           directly connected, Ethernet49/1
 C        30.4.206.0/24
           directly connected, Ethernet49/4
 B E      100.0.0.22/32 [20/0]
           via 20.22.206.22, Ethernet49/3
 B E      100.0.0.56/32 [20/0]
           via 20.56.200.56, Ethernet49/2
 B E      100.0.0.103/32 [20/0]
           via 20.103.206.103, Ethernet49/1
 C        100.0.0.206/32
           directly connected, Loopback0
 B E      100.0.30.4/32 [20/0]
           via 30.4.206.30, Ethernet49/4

```

## show ip arp

```text
Address         Age (sec)  Hardware Addr   Interface
20.103.206.103    0:00:07  0011.0100.0001  Ethernet49/1
20.56.200.56      0:00:04  407c.7dc4.ab9d  Ethernet49/2
20.22.206.22      0:00:21  c407.780a.9f31  Ethernet49/3
30.4.206.4        3:17:31  9c8a.cb49.040e  Ethernet49/4
30.4.206.30       0:00:04  9c8a.cb49.040e  Ethernet49/4
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

 C        20.22.206.0/24
           directly connected, Ethernet49/3
 C        20.56.200.0/24
           directly connected, Ethernet49/2
 C        20.103.206.0/24
           directly connected, Ethernet49/1
 C        30.4.206.0/24
           directly connected, Ethernet49/4
 B E      100.0.0.22/32 [20/0]
           via 20.22.206.22, Ethernet49/3
 B E      100.0.0.56/32 [20/0]
           via 20.56.200.56, Ethernet49/2
 B E      100.0.0.103/32 [20/0]
           via 20.103.206.103, Ethernet49/1
 C        100.0.0.206/32
           directly connected, Loopback0
 B E      100.0.30.4/32 [20/0]
           via 30.4.206.30, Ethernet49/4


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

! IP routing not enabled
```

## show ip arp vrf all

```text

VRF: default
Address         Age (sec)  Hardware Addr   Interface
20.103.206.103    0:00:07  0011.0100.0001  Ethernet49/1
20.56.200.56      0:00:04  407c.7dc4.ab9d  Ethernet49/2
20.22.206.22      0:00:21  c407.780a.9f31  Ethernet49/3
30.4.206.4        3:17:32  9c8a.cb49.040e  Ethernet49/4
30.4.206.30       0:00:05  9c8a.cb49.040e  Ethernet49/4

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.21.47     0:04:13  5c5a.c7ff.8a0a  Management1
192.168.21.50     0:01:17  a84f.b1a5.5221  Management1
192.168.21.59     0:02:42  6607.f5d1.ae16  Management1
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
Total Mac Addresses for this criterion: 0

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
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
Router identifier 100.0.0.206, local AS number 65206
```

## show bgp evpn instance

```text
```

## show interfaces counters rates | nz

```text
Port      Name         Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Et49/1    KEYSIGHT 103  5:00      3.8   0.0%        3      2.8   0.0%        2
Et49/2    NOK 56        5:00      2.8   0.0%        2      3.8   0.0%        3
Et49/3    H3C 22        5:00      0.0   0.0%        0      0.0   0.0%        0
Et49/4    JNPR 304      5:00      0.0   0.0%        0      0.0   0.0%        0
```

