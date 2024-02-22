# Test results for Spine1-J-200

## show hostname

```text
Hostname: SPINE1-J-200
FQDN:     SPINE1-J-200.ns.eantc.de
```

## show ip bgp summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.200, local AS number 65000
Neighbor Status Codes: m - Under maintenance
  Neighbor       V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  20.22.200.22   4 65022           2973      2938    0    0    1d16h Estab   1      1
  20.40.200.40   4 65040           2440      2938    0    0    1d16h Estab   1      1
  20.42.200.42   4 65042           2440      2938    0    0    1d16h Estab   1      1
  20.44.200.40   4 65044           2440      2943    0    0    1d16h Estab   1      1
  20.45.200.45   4 65045           2441      2943    0    0    1d16h Estab   3      3
  20.46.200.46   4 65045           2441      2946    0    0    1d16h Estab   3      3
  20.56.200.56   4 65056           4873      5802    0    0    1d16h Estab   1      1
  20.103.200.103 4 65103             35        51    0    0 00:16:00 Estab   1      1
  20.200.201.201 4 65201           2850      2938    0    0    1d16h Estab   2      2
  20.200.202.202 4 65202           2857      2939    0    0    1d16h Estab   2      2
  20.200.203.203 4 65203           1373      1415    0    0 19:22:30 Estab   2      2
  20.200.204.204 4 65204           1364      1418    0    0 19:23:01 Estab   2      2
  20.200.206.206 4 65206           1300      1336    0    0 18:26:07 Estab   2      2
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.200, local AS number 65000
Neighbor Status Codes: m - Under maintenance
  Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  100.0.0.22  4 65022           3617     12419    0    0    1d16h Estab   13     13
  100.0.0.40  4 65040           2488     12676    0    0    1d16h Estab   24     24
  100.0.0.42  4 65042           2470     12694    0    0    1d16h Estab   16     16
  100.0.0.44  4 65044           2438     12746    0    0    1d16h Estab   0      0
  100.0.0.45  4 65045           2470     12707    0    0    1d16h Estab   16     16
  100.0.0.46  4 65045           2469     12694    0    0    1d16h Estab   16     16
  100.0.0.56  4 65056           5776     17016    0    0    1d16h Estab   32     32
  100.0.0.103 4 65103             46       257    0    0 00:16:00 Estab   12     12
  100.0.0.201 4 65201           5657      9240    0    0    1d16h Estab   32     32
  100.0.0.202 4 65202           7480      7941    0    0    1d16h Estab   26     26
  100.0.0.203 4 65203           1523      8711    0    0 19:22:26 Estab   16     16
  100.0.0.204 4 65204           1492      8744    0    0 19:23:00 Estab   18     18
  100.0.0.206 4 65206           1319      8437    0    0 18:26:06 Estab   7      7
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
BGP routing table entry for auto-discovery 0000:0000:0000:0000:0000, Route Distinguisher: 100.0.0.103:20
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (196.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1103:1103 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 Route-Target-AS:1304:1304 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
BGP routing table entry for mac-ip 0013.0100.0001, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0001 10.10.201.201, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0001 10.10.201.201, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0002, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0002, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0002 10.30.1.201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0002 10.30.1.201, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0003, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0003, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0003 10.30.2.201, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0013.0100.0003 10.30.2.201, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0014.0100.0002, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0014.0100.0002 10.30.1.56, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0014.0100.0003, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0014.0100.0003 10.30.2.56, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0015.0100.0002, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0015.0100.0002 10.30.1.203, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0015.0100.0002 10.30.1.203, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0015.0100.0003, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0015.0100.0003 10.30.2.203, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1302 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0015.0100.0003 10.30.2.203, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0016.0100.0001, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan
      VNI: 1040 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0001 10.10.40.40, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1040 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0002, Route Distinguisher: 100.0.0.40:34068
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0002 10.30.1.40, Route Distinguisher: 100.0.0.40:34068
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0003, Route Distinguisher: 100.0.0.40:34069
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0003 10.30.2.40, Route Distinguisher: 100.0.0.40:34069
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0004, Route Distinguisher: 100.0.0.40:34070
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0004 10.30.3.40, Route Distinguisher: 100.0.0.40:34070
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0005, Route Distinguisher: 100.0.0.40:34071
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1304:1304 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0016.0100.0005 10.30.4.40, Route Distinguisher: 100.0.0.40:34071
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1304:1304 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0001, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65042
    100.0.0.42 from 100.0.0.42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan
      VNI: 1042 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0001 10.10.42.42, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65042
    100.0.0.42 from 100.0.0.42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1042 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0002, Route Distinguisher: 100.0.0.42:34068
 Paths: 1 available
  65042
    100.0.0.42 from 100.0.0.42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0002 10.30.1.42, Route Distinguisher: 100.0.0.42:34068
 Paths: 1 available
  65042
    100.0.0.42 from 100.0.0.42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0003, Route Distinguisher: 100.0.0.42:34069
 Paths: 1 available
  65042
    100.0.0.42 from 100.0.0.42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0017.0100.0003 10.30.2.42, Route Distinguisher: 100.0.0.42:34069
 Paths: 1 available
  65042
    100.0.0.42 from 100.0.0.42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0001, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0001, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0001 10.10.45.45, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0001 10.10.45.45, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0002, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0002, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0002 10.30.1.45, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0002 10.30.1.45, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0003, Route Distinguisher: 100.0.0.45:34069
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0003, Route Distinguisher: 100.0.0.46:34069
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0003 10.30.2.45, Route Distinguisher: 100.0.0.45:34069
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0018.0100.0003 10.30.2.45, Route Distinguisher: 100.0.0.46:34069
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0019.0100.0001 10.10.22.22, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0019.0100.0002, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0019.0100.0002 10.30.1.22, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0019.0100.0003, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0019.0100.0003 10.30.2.22, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0022.2200.0001 10.10.103.103, Route Distinguisher: 100.0.0.103:1103
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (196.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1103:1103 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:05:00:00:01
      VNI: 1103 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.10.56.253, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.30.1.254, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.5656.5656 10.30.2.254, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.56.254, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.2.254, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 02a4.023e.28dc 192.168.1.2, Route Distinguisher: 100.0.3.41:1111
 Paths: 1 available
  65056 64512
    100.0.3.41 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:100:100 Route-Target-AS:64512:1111 Route-Origin-IP:100.0.3.41:1111
      VNI: 384032 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan
      VNI: 1040 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65042
    100.0.0.42 from 100.0.0.42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan
      VNI: 1042 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.22.202, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.40.202, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1040 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.42.202, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65042
    100.0.0.42 from 100.0.0.42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1042 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.45.202, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.45.202, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.201.202, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.201.202, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.30.1.202, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.30.1.202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.30.2.202, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 444c.a873.5c75 10.30.2.202, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 5c5a.c773.4abb, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan
      VNI: 1040 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65042
    100.0.0.42 from 100.0.0.42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan
      VNI: 1042 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb 10.10.40.25, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1040 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb 10.10.42.25, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65042
    100.0.0.42 from 100.0.0.42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1042 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb 10.10.45.25, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 5c5a.c773.4abb 10.10.45.25, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 Route-Origin-IP:100.0.0.41:0 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 0013.0100.0004, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0013.0100.0004, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0013.0100.0004 10.30.3.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0013.0100.0004 10.30.3.201, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0015.0100.0004, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0015.0100.0004 10.30.3.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0015.0100.0004 10.30.3.203, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0019.0100.0004 10.30.3.22, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 444c.a873.5c75, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 444c.a873.5c75 10.30.3.202, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 444c.a873.5c75 10.30.3.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0013.0100.0005, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0013.0100.0005, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0013.0100.0005 10.30.4.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0013.0100.0005 10.30.4.201, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0015.0100.0005, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 0015.0100.0005 10.30.4.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 0015.0100.0005 10.30.4.203, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 0019.0100.0005 10.30.4.22, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 444c.a873.5c75, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 444c.a873.5c75 10.30.4.202, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 444c.a873.5c75 10.30.4.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnNdFlags:pflag
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
```

## show bgp evpn route-type imet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
      PMSI Tunnel: Ingress Replication, MPLS Label: 1022, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 100.0.0.40, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan
      VNI: 1040
      PMSI Tunnel: Ingress Replication, MPLS Label: 1040, Leaf Information Required: false, Tunnel ID: 100.0.0.40
BGP routing table entry for imet 100.0.0.40, Route Distinguisher: 100.0.0.40:34068
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.40
BGP routing table entry for imet 100.0.0.40, Route Distinguisher: 100.0.0.40:34069
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.40
BGP routing table entry for imet 100.0.0.40, Route Distinguisher: 100.0.0.40:34070
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.40
BGP routing table entry for imet 100.0.0.40, Route Distinguisher: 100.0.0.40:34071
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1304:1304 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.40
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan
      VNI: 1045
      PMSI Tunnel: Ingress Replication, MPLS Label: 1045, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.45:34069
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan
      VNI: 1045
      PMSI Tunnel: Ingress Replication, MPLS Label: 1045, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.41, Route Distinguisher: 100.0.0.46:34069
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.41
BGP routing table entry for imet 100.0.0.42, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65042
    100.0.0.42 from 100.0.0.42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan
      VNI: 1042
      PMSI Tunnel: Ingress Replication, MPLS Label: 1042, Leaf Information Required: false, Tunnel ID: 100.0.0.42
BGP routing table entry for imet 100.0.0.42, Route Distinguisher: 100.0.0.42:34068
 Paths: 1 available
  65042
    100.0.0.42 from 100.0.0.42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.42
BGP routing table entry for imet 100.0.0.42, Route Distinguisher: 100.0.0.42:34069
 Paths: 1 available
  65042
    100.0.0.42 from 100.0.0.42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.42
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan DF Election: Modulus-based Multicast Flags: OISM-supported, PEG, SBD
      VNI: 1000
      PMSI Tunnel: Ingress Replication, MPLS Label: 1000, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported
      VNI: 1056
      PMSI Tunnel: Ingress Replication, MPLS Label: 1056, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.103, Route Distinguisher: 100.0.0.103:2
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (196.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported, SBD
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 100.0.0.103, Route Distinguisher: 100.0.0.103:3
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (196.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported, SBD
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 100.0.0.103, Route Distinguisher: 100.0.0.103:1103
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (196.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1103:1103 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported, SBD
      VNI: 1103
      PMSI Tunnel: Ingress Replication, MPLS Label: 1103, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
      PMSI Tunnel: Ingress Replication, MPLS Label: 1201, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.201, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 100.0.0.202, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
      PMSI Tunnel: Ingress Replication, MPLS Label: 1201, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 100.0.0.202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 100.0.0.202, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 100.0.0.203, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
      PMSI Tunnel: Ingress Replication, MPLS Label: 1203, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 100.0.0.203, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 100.0.0.203, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 100.0.0.204, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 100.0.0.204, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 100.0.0.206, Route Distinguisher: 100.0.0.206:1000
 Paths: 1 available
  65206
    100.0.0.206 from 100.0.0.206 (100.0.0.206)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan DF Election: Modulus-based Multicast Flags: IGMP proxy, OISM-supported, PEG, SBD
      VNI: 1000
      PMSI Tunnel: Ingress Replication, MPLS Label: 1000, Leaf Information Required: false, Tunnel ID: 100.0.0.206
BGP routing table entry for imet 100.0.0.206, Route Distinguisher: 100.0.0.206:1301
 Paths: 1 available
  65206
    100.0.0.206 from 100.0.0.206 (100.0.0.206)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 100.0.0.206
BGP routing table entry for imet 100.0.0.206, Route Distinguisher: 100.0.0.206:1302
 Paths: 1 available
  65206
    100.0.0.206 from 100.0.0.206 (100.0.0.206)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 100.0.0.206
BGP routing table entry for imet 1303 100.0.0.22, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 1303 100.0.0.56, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1303 100.0.0.103, Route Distinguisher: 100.0.0.103:4
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (196.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported, SBD
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 1303 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1303 100.0.0.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1303 100.0.0.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 1303 100.0.0.204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 1303 100.0.0.206, Route Distinguisher: 100.0.0.206:1303
 Paths: 1 available
  65206
    100.0.0.206 from 100.0.0.206 (100.0.0.206)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.206
BGP routing table entry for imet 1304 100.0.0.22, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65022
    100.0.0.22 from 100.0.0.22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.22
BGP routing table entry for imet 1304 100.0.0.56, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1304 100.0.0.103, Route Distinguisher: 100.0.0.103:5
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (196.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1304:1304 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported, SBD
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.103
BGP routing table entry for imet 1304 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.201
BGP routing table entry for imet 1304 100.0.0.202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.202
BGP routing table entry for imet 1304 100.0.0.203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.203
BGP routing table entry for imet 1304 100.0.0.204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 1304 100.0.0.206, Route Distinguisher: 100.0.0.206:1303
 Paths: 1 available
  65206
    100.0.0.206 from 100.0.0.206 (100.0.0.206)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.206
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
BGP routing table entry for ethernet-segment 0000:0000:0000:0000:0000 100.0.0.103, Route Distinguisher: 100.0.0.103:1
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (196.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:00:00:00:00
BGP routing table entry for ethernet-segment 0000:0000:0000:0201:0202 100.0.0.201, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:10:02:02 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0201:0202 100.0.0.202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  65202
    100.0.0.202 from 100.0.0.202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:10:02:02 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0203:0204 100.0.0.203, Route Distinguisher: 100.0.0.203:1
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:30:02:04 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0203:0204 100.0.0.204, Route Distinguisher: 100.0.0.204:1
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:30:02:04 DF Election: Preference 200
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
BGP routing table entry for ip-prefix 1.2.3.0/24, Route Distinguisher: 100.0.3.60:0
 Paths: 1 available
  65056 64512 64999
    100.0.3.60 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:100:100
      VNI: 0 Gateway IP Address: 192.168.1.2
BGP routing table entry for ip-prefix 10.10.40.0/24, Route Distinguisher: 100.0.0.40:1000
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.42.0/24, Route Distinguisher: 100.0.0.42:1000
 Paths: 1 available
  65042
    100.0.0.42 from 100.0.0.42 (100.0.0.42)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.45.0/24, Route Distinguisher: 100.0.0.45:4
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.45 (100.0.0.45)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.45.0/24, Route Distinguisher: 100.0.0.46:4
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.46 (100.0.0.46)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.56.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.20.56.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.20.206.0/24, Route Distinguisher: 100.0.0.206:1000
 Paths: 1 available
  65206
    100.0.0.206 from 100.0.0.206 (100.0.0.206)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:c4:02:71
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.40:1000
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.42:1000
 Paths: 1 available
  65042
    100.0.0.42 from 100.0.0.42 (100.0.0.42)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.45:4
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.45 (100.0.0.45)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.46:4
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.46 (100.0.0.46)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.103:2
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (196.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:05:00:00:01
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.56/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.40:1000
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.42:1000
 Paths: 1 available
  65042
    100.0.0.42 from 100.0.0.42 (100.0.0.42)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.45:4
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.45 (100.0.0.45)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:7b:8b:87
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.46:4
 Paths: 1 available
  65045
    100.0.0.41 from 100.0.0.46 (100.0.0.46)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:6c:31:0e:b7:50:5f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.103:3
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (196.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:05:00:00:01
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.56/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.40:1000
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.40:1000
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 100.0.1.202/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056 65202
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 100.9.9.0/24, Route Distinguisher: 100.0.3.60:0
 Paths: 1 available
  65056 64512
    100.0.3.60 from 100.0.0.56 (100.0.0.56)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:100:100
      VNI: 384032
BGP routing table entry for ip-prefix 1303 10.30.3.0/24, Route Distinguisher: 100.0.0.103:4
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (196.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:05:00:00:01
      VNI: 1000
BGP routing table entry for ip-prefix 1304 10.30.4.0/24, Route Distinguisher: 100.0.0.103:5
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (196.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:05:00:00:01
      VNI: 1000
```

## show bgp evpn route-type smet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
BGP routing table entry for smet (S, G): (*, *) originating IP: 100.0.0.206, Route Distinguisher: 100.0.0.206:1000
 Paths: 1 available
  65206
    100.0.0.206 from 100.0.0.206 (100.0.0.206)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan
      Multicast Flags: exclude
```

## show bgp evpn route-type spmsi detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
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

 C        20.22.200.0/24
           directly connected, Ethernet26
 C        20.40.200.0/24
           directly connected, Ethernet15
 C        20.42.200.0/24
           directly connected, Ethernet16
 C        20.44.200.0/24
           directly connected, Ethernet17
 C        20.45.200.0/24
           directly connected, Ethernet13
 C        20.46.200.0/24
           directly connected, Ethernet14
 C        20.56.200.0/24
           directly connected, Ethernet11
 C        20.103.200.0/24
           directly connected, Ethernet12
 C        20.200.201.0/24
           directly connected, Ethernet1
 C        20.200.202.0/24
           directly connected, Ethernet2
 C        20.200.203.0/24
           directly connected, Ethernet3
 C        20.200.204.0/24
           directly connected, Ethernet4
 C        20.200.206.0/24
           directly connected, Ethernet5
 B E      100.0.0.22/32 [20/0]
           via 20.22.200.22, Ethernet26
 B E      100.0.0.40/32 [20/0]
           via 20.40.200.40, Ethernet15
 B E      100.0.0.41/32 [20/0]
           via 20.45.200.45, Ethernet13
           via 20.46.200.46, Ethernet14
 B E      100.0.0.42/32 [20/0]
           via 20.42.200.42, Ethernet16
 B E      100.0.0.44/32 [20/0]
           via 20.44.200.40, Ethernet17
 B E      100.0.0.45/32 [20/0]
           via 20.45.200.45, Ethernet13
           via 20.46.200.46, Ethernet14
 B E      100.0.0.46/32 [20/0]
           via 20.45.200.45, Ethernet13
           via 20.46.200.46, Ethernet14
 B E      100.0.0.56/32 [20/0]
           via 20.56.200.56, Ethernet11
 B E      100.0.0.103/32 [20/0]
           via 20.103.200.103, Ethernet12
 C        100.0.0.200/32
           directly connected, Loopback0
 B E      100.0.0.201/32 [20/0]
           via 20.200.201.201, Ethernet1
 B E      100.0.0.202/32 [20/0]
           via 20.200.202.202, Ethernet2
 B E      100.0.0.203/32 [20/0]
           via 20.200.203.203, Ethernet3
 B E      100.0.0.204/32 [20/0]
           via 20.200.204.204, Ethernet4
 B E      100.0.0.206/32 [20/0]
           via 20.200.206.206, Ethernet5

```

## show ip arp

```text
Address         Age (sec)  Hardware Addr   Interface
20.200.201.201    0:00:15  2899.3a8f.8f6f  Ethernet1
20.200.202.202    0:00:15  7483.ef0b.a4fb  Ethernet2
20.200.203.203    0:00:12  3838.a621.e82f  Ethernet3
20.200.204.204    0:00:15  985d.82a2.04f9  Ethernet4
20.200.206.206    0:00:15  985d.82c4.0271  Ethernet5
20.56.200.56      0:00:06  407c.7dc4.ab9d  Ethernet11
20.103.200.103    0:00:03  0011.0100.0001  Ethernet12
20.45.200.45      0:00:10  6c31.0e7b.8b87  Ethernet13
20.46.200.46      0:00:09  6c31.0eb7.505f  Ethernet14
20.40.200.40      0:00:06  246c.8474.8ddb  Ethernet15
20.42.200.42      0:00:09  4014.827b.84ab  Ethernet16
20.44.200.40      0:00:08  5c5a.c773.4abb  Ethernet17
20.22.200.22      0:00:10  c407.780a.9f31  Ethernet26
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

 C        20.22.200.0/24
           directly connected, Ethernet26
 C        20.40.200.0/24
           directly connected, Ethernet15
 C        20.42.200.0/24
           directly connected, Ethernet16
 C        20.44.200.0/24
           directly connected, Ethernet17
 C        20.45.200.0/24
           directly connected, Ethernet13
 C        20.46.200.0/24
           directly connected, Ethernet14
 C        20.56.200.0/24
           directly connected, Ethernet11
 C        20.103.200.0/24
           directly connected, Ethernet12
 C        20.200.201.0/24
           directly connected, Ethernet1
 C        20.200.202.0/24
           directly connected, Ethernet2
 C        20.200.203.0/24
           directly connected, Ethernet3
 C        20.200.204.0/24
           directly connected, Ethernet4
 C        20.200.206.0/24
           directly connected, Ethernet5
 B E      100.0.0.22/32 [20/0]
           via 20.22.200.22, Ethernet26
 B E      100.0.0.40/32 [20/0]
           via 20.40.200.40, Ethernet15
 B E      100.0.0.41/32 [20/0]
           via 20.45.200.45, Ethernet13
           via 20.46.200.46, Ethernet14
 B E      100.0.0.42/32 [20/0]
           via 20.42.200.42, Ethernet16
 B E      100.0.0.44/32 [20/0]
           via 20.44.200.40, Ethernet17
 B E      100.0.0.45/32 [20/0]
           via 20.45.200.45, Ethernet13
           via 20.46.200.46, Ethernet14
 B E      100.0.0.46/32 [20/0]
           via 20.45.200.45, Ethernet13
           via 20.46.200.46, Ethernet14
 B E      100.0.0.56/32 [20/0]
           via 20.56.200.56, Ethernet11
 B E      100.0.0.103/32 [20/0]
           via 20.103.200.103, Ethernet12
 C        100.0.0.200/32
           directly connected, Loopback0
 B E      100.0.0.201/32 [20/0]
           via 20.200.201.201, Ethernet1
 B E      100.0.0.202/32 [20/0]
           via 20.200.202.202, Ethernet2
 B E      100.0.0.203/32 [20/0]
           via 20.200.203.203, Ethernet3
 B E      100.0.0.204/32 [20/0]
           via 20.200.204.204, Ethernet4
 B E      100.0.0.206/32 [20/0]
           via 20.200.206.206, Ethernet5


VRF: 1022
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
           via 10.10.22.254, Vlan1022

 C        10.10.22.0/24
           directly connected, Vlan1022


VRF: 1040
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
           via 10.10.40.254, Vlan1040

 C        10.10.40.0/24
           directly connected, Vlan1040

! IP routing not enabled

VRF: 1042
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
           via 10.10.42.254, Vlan1042

 C        10.10.42.0/24
           directly connected, Vlan1042

! IP routing not enabled

VRF: 1044
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

Gateway of last resort is not reachable


! IP routing not enabled

VRF: 1045
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
           via 10.10.45.254, Vlan1045

 C        10.10.45.0/24
           directly connected, Vlan1045

! IP routing not enabled

VRF: 1056
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
           via 10.10.56.254, Vlan1056

 C        10.10.56.0/24
           directly connected, Vlan1056

! IP routing not enabled

VRF: 1201
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
           via 10.10.201.254, Vlan1201

 C        10.10.201.0/24
           directly connected, Vlan1201

! IP routing not enabled

VRF: 1203
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
           via 10.10.203.254, Vlan1203

 C        10.10.203.0/24
           directly connected, Vlan1203

! IP routing not enabled

VRF: 1301
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
           via 10.30.1.254, Vlan1301

 C        10.30.1.0/24
           directly connected, Vlan1301

! IP routing not enabled

VRF: 1301-201
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


! IP routing not enabled

VRF: 1301-203
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


! IP routing not enabled

VRF: 1302
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
           via 10.30.2.254, Vlan1302

 C        10.30.2.0/24
           directly connected, Vlan1302

! IP routing not enabled

VRF: 1302-201
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


! IP routing not enabled

VRF: 1302-203
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


! IP routing not enabled

VRF: 1303
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
           via 10.30.3.254, Vlan1303

 C        10.30.3.0/24
           directly connected, Vlan1303

! IP routing not enabled

VRF: 1303-201
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


! IP routing not enabled

VRF: 1303-203
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


! IP routing not enabled

VRF: 1304
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
           via 10.30.4.254, Vlan1304

 C        10.30.4.0/24
           directly connected, Vlan1304

! IP routing not enabled

VRF: 1304-201
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


! IP routing not enabled

VRF: 1304-203
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


! IP routing not enabled

VRF: 201
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

Gateway of last resort is not reachable


! IP routing not enabled

VRF: 203
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


! IP routing not enabled

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


VRF: red
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


! IP routing not enabled
```

## show ip arp vrf all

```text

VRF: 1022
Address         Age (sec)  Hardware Addr   Interface
10.10.22.254      0:12:02  00aa.aaaa.aaaa  Vlan1022, not learned

VRF: 1040
Address         Age (sec)  Hardware Addr   Interface
10.10.40.254      2:12:04  00aa.aaaa.aaaa  Vlan1040, Ethernet48

VRF: 1042
Address         Age (sec)  Hardware Addr   Interface
10.10.42.254      2:47:51  00aa.aaaa.aaaa  Vlan1042, not learned

VRF: 1044
Address         Age (sec)  Hardware Addr   Interface

VRF: 1045
Address         Age (sec)  Hardware Addr   Interface
10.10.45.254      2:34:05  00aa.aaaa.aaaa  Vlan1045, Ethernet48

VRF: 1056
Address         Age (sec)  Hardware Addr   Interface
10.10.56.254      3:31:10  00aa.aaaa.aaaa  Vlan1056, not learned

VRF: 1201
Address         Age (sec)  Hardware Addr   Interface
10.10.201.254     1:05:32  00aa.aaaa.aaaa  Vlan1201, Ethernet48

VRF: 1203
Address         Age (sec)  Hardware Addr   Interface
10.10.203.254     0:22:59  00aa.aaaa.aaaa  Vlan1203, not learned

VRF: 1301
Address         Age (sec)  Hardware Addr   Interface
10.30.1.254       3:13:29  00aa.aaaa.aaaa  Vlan1301, Ethernet48

VRF: 1301-201
Address         Age (sec)  Hardware Addr   Interface

VRF: 1301-203
Address         Age (sec)  Hardware Addr   Interface

VRF: 1302
Address         Age (sec)  Hardware Addr   Interface
10.30.2.254       3:51:53  00aa.aaaa.aaaa  Vlan1302, Ethernet48

VRF: 1302-201
Address         Age (sec)  Hardware Addr   Interface

VRF: 1302-203
Address         Age (sec)  Hardware Addr   Interface

VRF: 1303
Address         Age (sec)  Hardware Addr   Interface
10.30.3.254       3:23:05  00aa.aaaa.aaaa  Vlan1303, Ethernet48

VRF: 1303-201
Address         Age (sec)  Hardware Addr   Interface

VRF: 1303-203
Address         Age (sec)  Hardware Addr   Interface

VRF: 1304
Address         Age (sec)  Hardware Addr   Interface
10.30.4.254       1:42:15  00aa.aaaa.aaaa  Vlan1304, Ethernet48

VRF: 1304-201
Address         Age (sec)  Hardware Addr   Interface

VRF: 1304-203
Address         Age (sec)  Hardware Addr   Interface

VRF: 201
Address         Age (sec)  Hardware Addr   Interface

VRF: 203
Address         Age (sec)  Hardware Addr   Interface

VRF: default
Address         Age (sec)  Hardware Addr   Interface
20.200.201.201    0:00:15  2899.3a8f.8f6f  Ethernet1
20.200.202.202    0:00:15  7483.ef0b.a4fb  Ethernet2
20.200.203.203    0:00:13  3838.a621.e82f  Ethernet3
20.200.204.204    0:00:15  985d.82a2.04f9  Ethernet4
20.200.206.206    0:00:15  985d.82c4.0271  Ethernet5
20.56.200.56      0:00:06  407c.7dc4.ab9d  Ethernet11
20.103.200.103    0:00:03  0011.0100.0001  Ethernet12
20.45.200.45      0:00:11  6c31.0e7b.8b87  Ethernet13
20.46.200.46      0:00:09  6c31.0eb7.505f  Ethernet14
20.40.200.40      0:00:06  246c.8474.8ddb  Ethernet15
20.42.200.42      0:00:09  4014.827b.84ab  Ethernet16
20.44.200.40      0:00:09  5c5a.c773.4abb  Ethernet17
20.22.200.22      0:00:10  c407.780a.9f31  Ethernet26

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.20.2      0:02:43  bcea.fa02.6ce2  Management1
192.168.20.18     0:02:55  e484.29cd.e801  Management1
192.168.20.19     0:01:30  c407.7858.8001  Management1
192.168.20.20     0:00:10  e484.29d0.4001  Management1
192.168.20.21     0:04:57  7081.85c1.b801  Management1
192.168.20.22     0:00:29  c407.780a.9f04  Management1
192.168.20.23     0:01:11  c407.780a.7750  Management1
192.168.20.24     0:00:04  6c87.2089.ede5  Management1
192.168.20.25     0:03:50  6c87.2089.ece5  Management1
192.168.20.28     0:02:37  98a9.2d59.bae6  Management1
192.168.20.52     0:01:42  f83e.95dc.1289  Management1
192.168.21.50     0:04:08  a84f.b1a5.5221  Management1
192.168.21.59     0:04:45  6607.f5d1.ae16  Management1

VRF: red
Address         Age (sec)  Hardware Addr   Interface
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
1022    444c.a873.5c75    STATIC      Router
1040    00aa.aaaa.aaaa    DYNAMIC     Et48       1       0:00:49 ago
1040    246c.8474.8de0    DYNAMIC     Et48       1       21:14:47 ago
1040    444c.a873.5c75    STATIC      Router
1042    4014.827b.84b0    DYNAMIC     Et48       1       21:07:23 ago
1042    444c.a873.5c75    STATIC      Router
1045    0026.f002.0000    DYNAMIC     Et48       1       21:27:15 ago
1045    00aa.aaaa.aaaa    DYNAMIC     Et48       1       0:04:04 ago
1045    444c.a873.5c75    STATIC      Router
1056    0056.5656.5656    DYNAMIC     Et48       1       16:14:39 ago
1056    444c.a873.5c75    STATIC      Router
1201    00aa.aaaa.aaaa    DYNAMIC     Et48       1       1:17:27 ago
1201    444c.a873.5c75    STATIC      Router
1203    444c.a873.5c75    STATIC      Router
1301    0013.0100.0002    DYNAMIC     Et48       1       0:26:47 ago
1301    0014.0100.0002    DYNAMIC     Et48       1       0:11:28 ago
1301    0016.0100.0002    DYNAMIC     Et48       1       0:15:44 ago
1301    0017.0100.0002    DYNAMIC     Et48       1       0:11:28 ago
1301    0018.0100.0002    DYNAMIC     Et48       1       0:11:28 ago
1301    00aa.aaaa.aaaa    DYNAMIC     Et48       1       18:53:54 ago
1301    444c.a873.5c75    STATIC      Router
1302    0013.0100.0003    DYNAMIC     Et48       1       0:26:47 ago
1302    0014.0100.0003    DYNAMIC     Et48       1       0:11:28 ago
1302    0016.0100.0003    DYNAMIC     Et48       1       0:15:44 ago
1302    0017.0100.0003    DYNAMIC     Et48       1       0:11:28 ago
1302    0018.0100.0003    DYNAMIC     Et48       1       0:11:28 ago
1302    00aa.aaaa.aaaa    DYNAMIC     Et48       1       0:02:25 ago
1302    444c.a873.5c75    STATIC      Router
1303    0013.0100.0004    DYNAMIC     Et48       1       0:11:28 ago
1303    00aa.aaaa.aaaa    DYNAMIC     Et48       1       0:32:27 ago
1303    444c.a873.5c75    STATIC      Router
1304    0013.0100.0005    DYNAMIC     Et48       1       0:11:28 ago
1304    00aa.aaaa.aaaa    DYNAMIC     Et48       1       1:31:43 ago
1304    444c.a873.5c75    STATIC      Router
Total Mac Addresses for this criterion: 34

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
00aa.aaaa.aaaa, VLAN 1045, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
00aa.aaaa.aaaa, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0017.0100.0002, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
00aa.aaaa.aaaa, VLAN 1201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0018.0100.0002, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0018.0100.0003, VLAN 1302, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
00aa.aaaa.aaaa, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0016.0100.0002, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0013.0100.0004, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0013.0100.0003, VLAN 1302, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0016.0100.0003, VLAN 1302, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
4014.827b.84b0, VLAN 1042, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
00aa.aaaa.aaaa, VLAN 1040, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
00aa.aaaa.aaaa, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0014.0100.0002, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0017.0100.0003, VLAN 1302, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
00aa.aaaa.aaaa, VLAN 1302, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0014.0100.0003, VLAN 1302, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0013.0100.0005, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0056.5656.5656, VLAN 1056, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0013.0100.0002, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
246c.8474.8de0, VLAN 1040, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0026.f002.0000, VLAN 1045, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
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
Router identifier 100.0.0.200, local AS number 65000
```

## show bgp evpn instance

```text
```

## show interfaces counters rates | nz

```text
Port      Name         Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Et1       A-PE11-201    0:01      0.5   0.0%        0     79.1   0.9%       85
Et2       A-PE12-202    0:01     79.3   0.9%       85      0.7   0.0%        0
Et3       A-PE13-203    0:01     79.1   0.9%       85     78.6   0.9%       84
Et4       A-PE14-204    0:01      1.2   0.0%        1      1.6   0.0%        1
Et11      Nokia-56      0:05      1.4   0.0%        1      3.3   0.0%        3
Et12      Keysight-103  0:05      2.9   0.0%        2      0.0   0.0%        0
Et13      Cisco-45-N9K  0:05      0.5   0.0%        0      0.5   0.0%        0
Et14      Cisco-46-N9K  0:05      0.9   0.0%        1      0.9   0.0%        1
Et15      Cisco-40-N9K  0:05      1.9   0.0%        2     12.1   0.1%       13
Et16      Cisco-42-N9K  0:05      0.9   0.0%        1      0.9   0.0%        1
Et26      H3C-22        0:05    166.9   2.0%      179    157.7   1.8%      169
Et48      Spine-host    0:05     82.4   1.1%      143      0.0   0.0%        0
Ma1                     0:05      0.0   0.0%        0      0.1   0.0%        0
```

