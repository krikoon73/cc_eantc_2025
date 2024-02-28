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
  Neighbor     V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  20.22.206.22 4 65022            536       589    0    0 07:55:41 Estab   1      1
  20.56.200.56 4 65056            506       611    0    0 04:09:44 Estab   1      1
  30.4.206.30  4 65304           3541      3821    0    0    1d02h Estab   1      1
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.206, local AS number 65206
Neighbor Status Codes: m - Under maintenance
  Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  100.0.0.22  4 65022           3771      2123    0    0 02:04:25 Estab   97     97
  100.0.0.56  4 65056           6365      3318    0    0 01:49:28 Estab   174    114
  100.0.0.103 4 65103              0         0    0    0 00:02:51 Active
  100.0.30.4  4 65304           3512     28525    0    0    1d02h Estab   0      0
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.206, local AS number 65206
BGP routing table entry for auto-discovery 0 0000:0000:0000:0123:0123, Route Distinguisher: 100.0.0.34:2301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0 0000:0000:0000:0123:0123, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0000:0000:0000:0123:0123, Route Distinguisher: 100.0.37.9:0
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1301
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.30.14:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 0
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.30.14:1305
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 0
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 0
BGP routing table entry for auto-discovery 1303 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:1
 Paths: 2 available
  65022 65314 65000 65201
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
  65056 65205 65314 65000 65201
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.0.201:2
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1301 Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:1111:1111:1111:1111, Route Distinguisher: 100.0.30.14:0
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.22:2301
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 2301
  65056 65205
    100.0.0.22 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2301
BGP routing table entry for auto-discovery 0 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2301
BGP routing table entry for auto-discovery 0 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 1303 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2303
BGP routing table entry for auto-discovery 1303 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.22:2301
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
  65056 65205
    100.0.0.22 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:1301
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:51301
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
BGP routing table entry for auto-discovery 0000:2222:2222:2222:1111, Route Distinguisher: 100.0.0.56:51303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:524270
      VNI: 0
BGP routing table entry for auto-discovery 0 0030:0903:0405:0607:08cc, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0 0030:0903:0405:0607:08cc, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 2303 0030:0903:0405:0607:08cc, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 2304 0030:0903:0405:0607:08cc, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0030:0903:0405:0607:08cc, Route Distinguisher: 100.0.30.9:0
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0 0048:5648:5648:5648:5648, Route Distinguisher: 100.0.3.48:4558
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0048:5648:5648:5648:5648, Route Distinguisher: 100.0.3.48:1
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0500:00fc:0000:0000:0000, Route Distinguisher: 100.0.30.9:0
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0500:00fc:0000:0000:0000, Route Distinguisher: 100.0.37.9:0
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0500:00fc:0000:0008:ff00, Route Distinguisher: 100.0.30.9:0
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0500:00fc:0000:0009:0000, Route Distinguisher: 100.0.30.9:0
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for auto-discovery 0500:00ff:2200:0005:1500, Route Distinguisher: 100.0.30.14:0
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0500:00ff:2200:0005:1700, Route Distinguisher: 100.0.30.14:0
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0500:00ff:2200:0005:1800, Route Distinguisher: 100.0.30.14:0
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.206, local AS number 65206
BGP routing table entry for mac-ip 0056.5656.5656 10.10.103.254, Route Distinguisher: 100.0.0.56:1103
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1103 ESI: 0000:0000:0000:0000:0000
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1103 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.30.1.254, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 0056.5656.5656 10.30.1.254, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 0056.5656.5656 10.30.2.254, Route Distinguisher: 100.0.0.56:1302
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:1302:1302 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.14:1301
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2301 ESI: 0000:2222:2222:2222:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0500:00ff:2200:0005:1500
BGP routing table entry for mac-ip 00aa.aaaa.aaaa, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.103.254, Route Distinguisher: 100.0.0.56:1103
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1103 ESI: 0000:0000:0000:0000:0000
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:1103:1103 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1103 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.203.254, Route Distinguisher: 100.0.0.56:1203
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1203 ESI: 0000:0000:0000:0000:0000
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:1203:1203 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1203 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.30.14:1301
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 2301 ESI: 0000:2222:2222:2222:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0500:00ff:2200:0005:1500
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 20.30.1.254, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 20.30.1.254, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 20.30.2.254, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 00cc.cccc.bbbb, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 00cc.cccc.bbbb, Route Distinguisher: 100.0.0.201:1301
 Paths: 2 available
  65022 65000 65203
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 2301 L3 VNI: 1001 ESI: 0000:2222:2222:2222:1111
      D-PATH: 1:1:EVPN
  65056 65205 65000 65203
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:1111:1111:1111:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 60c7.8d2d.4416, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 60c7.8d2d.4416 20.30.1.201, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip e4f2.7cef.a505, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip e4f2.7cef.a505, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip e4f2.7cef.a505 20.30.1.200, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip e4f2.7cef.a505 20.30.2.200, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip f87a.4118.8af6, Route Distinguisher: 100.0.3.48:4558
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip f87a.416d.d0ec, Route Distinguisher: 100.0.3.48:4558
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip f8c1.1604.3007, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip f8c1.1604.3007, Route Distinguisher: 100.0.30.14:1301
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2301 ESI: 0000:2222:2222:2222:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip f8c1.1604.3007 10.30.1.14, Route Distinguisher: 100.0.0.56:51301
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2301 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip f8c1.1604.3007 10.30.1.14, Route Distinguisher: 100.0.30.14:1301
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2301 ESI: 0000:2222:2222:2222:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 001b.0100.0003, Route Distinguisher: 100.0.30.14:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:14
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:14
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:14
      VNI: 2303 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 001b.0100.0003 10.30.3.203, Route Distinguisher: 100.0.30.14:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:14
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:14
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 0056.5656.5656, Route Distinguisher: 100.0.30.14:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2303 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254, Route Distinguisher: 100.0.30.14:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.14:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.14:1305
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0500:00ff:2200:0005:1700
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0500:00ff:2200:0005:1700
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2303 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.30.14:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.30.14:1305
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0500:00ff:2200:0005:1700
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0500:00ff:2200:0005:1700
BGP routing table entry for mac-ip 1303 a266.0102.0001, Route Distinguisher: 100.0.30.14:1305
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 a266.0102.0001 10.30.3.103, Route Distinguisher: 100.0.0.56:51303
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 a266.0102.0001 10.30.3.103, Route Distinguisher: 100.0.30.14:1305
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 f8c1.1604.3007, Route Distinguisher: 100.0.30.14:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 f8c1.1604.3007, Route Distinguisher: 100.0.30.14:1305
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 f8c1.1604.3007 10.30.3.14, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2303 ESI: 0000:2222:2222:2222:1111
BGP routing table entry for mac-ip 1303 f8c1.1604.3007 10.30.3.14, Route Distinguisher: 100.0.30.14:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1303 f8c1.1604.3007 10.30.3.14, Route Distinguisher: 100.0.30.14:1305
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 0056.5656.5656, Route Distinguisher: 100.0.30.14:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254, Route Distinguisher: 100.0.0.56:51304
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254, Route Distinguisher: 100.0.30.14:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.14:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.14:1305
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0500:00ff:2200:0005:1800
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0500:00ff:2200:0005:1800
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.0.56:51304
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.30.14:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.30.14:1305
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0500:00ff:2200:0005:1800
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0500:00ff:2200:0005:1800
BGP routing table entry for mac-ip 1304 a288.0103.0001, Route Distinguisher: 100.0.30.14:1305
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1304 a288.0103.0001 10.30.4.103, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 a288.0103.0001 10.30.4.103, Route Distinguisher: 100.0.30.14:1305
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1304 f8c1.1604.3007, Route Distinguisher: 100.0.0.56:51304
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 f8c1.1604.3007, Route Distinguisher: 100.0.30.14:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1304 f8c1.1604.3007, Route Distinguisher: 100.0.30.14:1305
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 f8c1.1604.3007 10.30.4.14, Route Distinguisher: 100.0.0.56:51304
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 2304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 f8c1.1604.3007 10.30.4.14, Route Distinguisher: 100.0.30.14:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:65205:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:1111:1111:1111:1111
BGP routing table entry for mac-ip 1304 f8c1.1604.3007 10.30.4.14, Route Distinguisher: 100.0.30.14:1305
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2303 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 2303 00aa.aaaa.aaaa 20.30.3.254, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 2303 e4f2.7cef.a505, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 2303 e4f2.7cef.a505 20.30.3.200, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 2304 00aa.aaaa.aaaa, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 2304 00aa.aaaa.aaaa 20.30.4.254, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 2304 e4f2.7cef.a505, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for mac-ip 2304 e4f2.7cef.a505 20.30.4.200, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
```

## show bgp evpn route-type imet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.206, local AS number 65206
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
      PMSI Tunnel: Ingress Replication, MPLS Label: 1022, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1301
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.22
  65056 65205
    100.0.0.22 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1302
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.22
  65056 65205
    100.0.0.22 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:1302:1302 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:2301
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 2301
      PMSI Tunnel: Ingress Replication, MPLS Label: 2301, Leaf Information Required: false, Tunnel ID: 100.0.0.22
  65056 65205
    100.0.0.22 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:1301:1301 Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2301
      PMSI Tunnel: Ingress Replication, MPLS Label: 2301, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.34, Route Distinguisher: 100.0.0.34:2301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
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
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65056 65205 65314 65000 65201
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1302:1302 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.3.48, Route Distinguisher: 100.0.3.48:4558
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for imet 100.0.30.9, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for imet 100.0.30.9, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for imet 100.0.30.14, Route Distinguisher: 100.0.30.14:1301
 Paths: 1 available
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.30.14
BGP routing table entry for imet 100.0.37.9, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for imet 1303 100.0.0.22, Route Distinguisher: 100.0.0.22:1303
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.22
  65056 65205
    100.0.0.22 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 1303 100.0.0.56, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2303
      PMSI Tunnel: Ingress Replication, MPLS Label: 2303, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1303 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1303 100.0.30.14, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.30.14
BGP routing table entry for imet 1303 100.0.30.14, Route Distinguisher: 100.0.30.14:1305
 Paths: 1 available
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.30.14
BGP routing table entry for imet 1304 100.0.0.22, Route Distinguisher: 100.0.0.22:1304
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.22
  65056 65205
    100.0.0.22 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 1304 100.0.0.56, Route Distinguisher: 100.0.0.56:51304
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 2304
      PMSI Tunnel: Ingress Replication, MPLS Label: 2304, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1304 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1304 100.0.30.14, Route Distinguisher: 100.0.30.14:1303
 Paths: 1 available
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.30.14
BGP routing table entry for imet 1304 100.0.30.14, Route Distinguisher: 100.0.30.14:1305
 Paths: 1 available
  65056 65205
    100.0.30.14 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1303:1303 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.30.14
BGP routing table entry for imet 2303 100.0.30.9, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for imet 2304 100.0.30.9, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.206, local AS number 65206
BGP routing table entry for ethernet-segment 0000:0000:0000:0111:0111 100.0.0.56, Route Distinguisher: 100.0.0.56:0
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:00:00:00:00:00:01
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:00:00:00:00:00:01
BGP routing table entry for ethernet-segment 0000:0000:0000:0123:0123 100.0.37.9, Route Distinguisher: 100.0.37.9:0
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.0.201, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:11:11:11:11:11 DF Election: Preference 100
BGP routing table entry for ethernet-segment 0000:1111:1111:1111:1111 100.0.30.14, Route Distinguisher: 100.0.30.14:0
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:11:11:11:11:11
BGP routing table entry for ethernet-segment 0000:2222:2222:2222:1111 100.0.0.22, Route Distinguisher: 100.0.0.22:0
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:22:22:22:22:22 DF Election: Modulus-based
  65056 65205
    100.0.0.22 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:22:22:22:22:22 DF Election: Modulus-based
BGP routing table entry for ethernet-segment 0000:2222:2222:2222:1111 100.0.0.56, Route Distinguisher: 100.0.0.56:0
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:00:22:22:22:22:22
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:00:22:22:22:22:22
BGP routing table entry for ethernet-segment 0048:5648:5648:5648:5648 100.0.0.56, Route Distinguisher: 100.0.0.56:0
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP head, ECMP, best, ECMP contributor
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:48:56:48:56:48:56
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, ECMP, ECMP contributor
      Extended Community: Route-Origin-AS:56:56 EvpnEsImportRt:48:56:48:56:48:56
BGP routing table entry for ethernet-segment 0048:5648:5648:5648:5648 100.0.3.48, Route Distinguisher: 100.0.3.48:0
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.206, local AS number 65206
BGP routing table entry for ip-prefix 10.10.103.0/24, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.10.103.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:EVPN
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
  65056 65205
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056 65000 65204
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 2 available
  65022 65000 65204
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
      D-PATH: 1:1:EVPN
  65056 65205 65000 65204
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.203/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056 65000 65203
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 10.10.203.203/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 2 available
  65022 65000 65203
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
      D-PATH: 1:1:EVPN
  65056 65205 65000 65203
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 2 available
  65022 65000 65203
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
      D-PATH: 1:1:EVPN
  65056 65205 65000 65203
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.1.14/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.1.14/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056 65000 65204
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 2 available
  65022 65000 65204
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
      D-PATH: 1:1:EVPN
  65056 65205 65000 65204
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.22:1000
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
  65056 65205
    100.0.0.22 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 2 available
  65022 65000 65204
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
      D-PATH: 1:1:EVPN
  65056 65205 65000 65204
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.3.14/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.3.14/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.3.203/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.3.203/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.3.254/32, Route Distinguisher: 100.0.0.22:1000
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
  65056 65205
    100.0.0.22 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.22:1000
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
  65056 65205
    100.0.0.22 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 2 available
  65022 65000 65204
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
      D-PATH: 1:1:EVPN
  65056 65205 65000 65204
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 10.30.4.14/32, Route Distinguisher: 100.0.0.56:652
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.4.14/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.4.254/32, Route Distinguisher: 100.0.0.22:1000
 Paths: 2 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
  65056 65205
    100.0.0.22 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan DefaultGateway EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1000
BGP routing table entry for ip-prefix 20.10.33.0/24, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 20.10.33.200/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 20.10.33.254/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 20.30.1.0/24, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 20.30.1.200/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 20.30.1.254/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 20.30.2.0/24, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 20.30.2.200/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 20.30.2.254/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 20.30.3.0/24, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 20.30.3.200/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 20.30.3.254/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 20.30.4.0/24, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 20.30.4.200/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref -, weight 0, tag 0, invalid, local
BGP routing table entry for ip-prefix 20.30.4.254/32, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  Local
    PolicyReject from 100.0.0.56 (100.0.0.56)
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
 Paths: 2 available
  65022 65000 65203
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
      D-PATH: 1:1:EVPN
  65056 65205 65000 65203
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.204/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056 65000 65204
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1001
      D-PATH: 2:2:EVPN 1:1:EVPN
BGP routing table entry for ip-prefix 100.0.1.204/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 2 available
  65022 65000 65204
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1001
      D-PATH: 1:1:EVPN
  65056 65205 65000 65204
    100.0.0.201 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:65205:1000 Route-Origin-AS:56:56 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
      D-PATH: 1:1:EVPN
```

## show bgp evpn route-type smet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.206, local AS number 65206
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
 C        100.0.0.206/32
           directly connected, Loopback0
 B E      100.0.30.4/32 [20/0]
           via 30.4.206.30, Ethernet49/4

```

## show ip arp

```text
Address         Age (sec)  Hardware Addr   Interface
20.103.206.103    0:06:28  0011.0100.0001  Ethernet49/1
20.56.200.56      0:00:15  407c.7dc4.ab9d  Ethernet49/2
20.22.206.22      0:00:22  c407.780a.9f31  Ethernet49/3
30.4.206.4        1:23:14  9c8a.cb49.040e  Ethernet49/4
30.4.206.30       0:00:09  9c8a.cb49.040e  Ethernet49/4
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
20.103.206.103    0:06:28  0011.0100.0001  Ethernet49/1
20.56.200.56      0:00:16  407c.7dc4.ab9d  Ethernet49/2
20.22.206.22      0:00:22  c407.780a.9f31  Ethernet49/3
30.4.206.4        1:23:14  9c8a.cb49.040e  Ethernet49/4
30.4.206.30       0:00:09  9c8a.cb49.040e  Ethernet49/4

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.21.47     0:03:06  5c5a.c7ff.8a0a  Management1
192.168.21.50     0:00:40  a84f.b1a5.5221  Management1
192.168.21.59     0:02:36  6607.f5d1.ae16  Management1
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
Et49/1    KEYSIGHT 103  5:00      0.1   0.0%        0      0.1   0.0%        0
Et49/2    NOK 56        5:00      0.1   0.0%        0      0.0   0.0%        0
Et49/3    H3C 22        5:00      0.0   0.0%        0      0.0   0.0%        0
Et49/4    JNPR 304      5:00      0.0   0.0%        0      0.0   0.0%        0
```

