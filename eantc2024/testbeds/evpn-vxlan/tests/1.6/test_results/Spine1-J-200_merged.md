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
  20.40.200.40   4 65040           3942      4913    0    0    2d17h Estab   1      1
  20.42.200.42   4 65042           3942      4914    0    0    2d17h Estab   1      1
  20.44.200.40   4 65044           3942      4927    0    0    2d17h Estab   1      1
  20.45.200.45   4 65045           3943      4926    0    0    2d17h Estab   3      3
  20.46.200.46   4 65045           3943      4919    0    0    2d17h Estab   3      3
  20.56.200.56   4 65056           7877      9525    0    0    2d17h Estab   1      1
  20.103.200.103 4 65103             39        54    0    0 00:17:34 Estab   1      1
  20.200.201.201 4 65201           4620      4916    0    0    2d17h Estab   2      2
  20.200.203.203 4 65203           1244      1267    0    0 17:36:18 Estab   2      2
  20.200.204.204 4 65204           1242      1266    0    0 17:36:14 Estab   2      2
  20.200.206.206 4 65206           1443      1473    0    0 20:25:39 Estab   2      2
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.200, local AS number 65000
Neighbor Status Codes: m - Under maintenance
  Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  100.0.0.40  4 65040           3992     19101    0    0    2d17h Estab   16     16
  100.0.0.42  4 65042           3975     19101    0    0    2d17h Estab   12     12
  100.0.0.44  4 65044           3940     19174    0    0    2d17h Estab   0      0
  100.0.0.45  4 65045           3975     19119    0    0    2d17h Estab   12     12
  100.0.0.46  4 65045           3974     19108    0    0    2d17h Estab   12     12
  100.0.0.56  4 65056            386       413    0    0 00:19:43 Estab   123    123
  100.0.0.103 4 65103             43       141    0    0 00:17:34 Estab   5      5
  100.0.0.201 4 65201           7984     14939    0    0    2d17h Estab   11     11
  100.0.0.203 4 65203           1520      2281    0    0 17:36:17 Estab   25     25
  100.0.0.204 4 65204           1517      2309    0    0 17:36:13 Estab   21     21
  100.0.0.206 4 65206           1515      2835    0    0 20:25:38 Estab   8      8
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
BGP routing table entry for auto-discovery 0000:0000:0000:0000:0000, Route Distinguisher: 100.0.0.103:20
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (193.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
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
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
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
BGP routing table entry for auto-discovery 0 0001:0203:0405:0607:0801, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301
      VNI: 304
BGP routing table entry for auto-discovery 0 0001:0203:0405:0607:0801, Route Distinguisher: 100.0.37.9:2302
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302
      VNI: 336
BGP routing table entry for auto-discovery 0 0001:0203:0405:0607:0801, Route Distinguisher: 100.0.37.9:2303
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 592
BGP routing table entry for auto-discovery 0001:0203:0405:0607:0801, Route Distinguisher: 100.0.37.9:0
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2032:2032 Route-Target-AS:2301:2301 Route-Target-AS:2302:2302 Route-Target-AS:2303:2303 EvpnEsiLabel:31
      VNI: 0
BGP routing table entry for auto-discovery 0 0001:0203:0405:0607:0802, Route Distinguisher: 100.0.0.4:2301
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2301:2301 Route-Origin-IP:100.0.0.34:0
      VNI: 770592
BGP routing table entry for auto-discovery 0 0001:0203:0405:0607:0802, Route Distinguisher: 100.0.0.4:2302
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2302:2302 Route-Origin-IP:100.0.0.34:0
      VNI: 770672
BGP routing table entry for auto-discovery 2303 0001:0203:0405:0607:0802, Route Distinguisher: 100.0.0.4:2303
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2303:2303 Route-Origin-IP:100.0.0.34:0
      VNI: 770720
BGP routing table entry for auto-discovery 2304 0001:0203:0405:0607:0802, Route Distinguisher: 100.0.0.4:2303
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2303:2303 Route-Origin-IP:100.0.0.34:0
      VNI: 770816
BGP routing table entry for auto-discovery 0001:0203:0405:0607:0802, Route Distinguisher: 100.0.0.34:0
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2004:2004 Route-Target-AS:2301:2301 Route-Target-AS:2302:2302 Route-Target-AS:2303:2303 EvpnEsiLabel:48165
      VNI: 0
BGP routing table entry for auto-discovery 0 0001:0203:0405:0607:08cc, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301
      VNI: 3856
BGP routing table entry for auto-discovery 0 0001:0203:0405:0607:08cc, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302
      VNI: 3904
BGP routing table entry for auto-discovery 2303 0001:0203:0405:0607:08cc, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 3952
BGP routing table entry for auto-discovery 2304 0001:0203:0405:0607:08cc, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 3968
BGP routing table entry for auto-discovery 0001:0203:0405:0607:08cc, Route Distinguisher: 100.0.30.9:0
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2033:2033 Route-Target-AS:2301:2301 Route-Target-AS:2302:2302 Route-Target-AS:2303:2303 EvpnEsiLabel:530
      VNI: 0
BGP routing table entry for auto-discovery 0500:00fc:0000:0008:fd00, Route Distinguisher: 100.0.37.9:0
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 EvpnEsiLabel:160
      VNI: 0
BGP routing table entry for auto-discovery 0500:00fc:0000:0008:fe00, Route Distinguisher: 100.0.37.9:0
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302 EvpnEsiLabel:162
      VNI: 0
BGP routing table entry for auto-discovery 0500:00fc:0000:0008:ff00, Route Distinguisher: 100.0.37.9:0
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 EvpnEsiLabel:164
      VNI: 0
BGP routing table entry for auto-discovery 0500:00fc:0000:0009:0000, Route Distinguisher: 100.0.37.9:0
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 EvpnEsiLabel:166
      VNI: 0
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
BGP routing table entry for mac-ip 0013.0100.0002, Route Distinguisher: 100.0.0.4:2301
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2301:2301 Route-Origin-IP:100.0.0.34:0
      VNI: 770592 ESI: 0001:0203:0405:0607:0802
BGP routing table entry for mac-ip 0013.0100.0002 20.30.1.4, Route Distinguisher: 100.0.0.4:2301
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2301:2301 Route-Origin-IP:100.0.0.34:0
      VNI: 770592 ESI: 0001:0203:0405:0607:0802
BGP routing table entry for mac-ip 0013.0100.0003, Route Distinguisher: 100.0.0.4:2302
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2302:2302 Route-Origin-IP:100.0.0.34:0
      VNI: 770672 ESI: 0001:0203:0405:0607:0802
BGP routing table entry for mac-ip 0013.0100.0003 20.30.2.4, Route Distinguisher: 100.0.0.4:2302
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2302:2302 Route-Origin-IP:100.0.0.34:0
      VNI: 770672 ESI: 0001:0203:0405:0607:0802
BGP routing table entry for mac-ip 0014.0100.0001, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0015.0100.0001, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0015.0100.0001 10.10.203.203, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f EvpnNdFlags:pflag
      VNI: 1203 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0015.0100.0001 10.10.203.203, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1203 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
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
BGP routing table entry for mac-ip 00aa.aaaa.aaaa, Route Distinguisher: 100.0.0.4:2301
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2301:2301 Route-Origin-IP:100.0.0.34:0 EvpnMacMobility:sticky
      VNI: 770592 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa, Route Distinguisher: 100.0.0.4:2302
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2302:2302 Route-Origin-IP:100.0.0.34:0 EvpnMacMobility:sticky
      VNI: 770672 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.56.254, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
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
BGP routing table entry for mac-ip 444c.a873.5c75, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203 ESI: 0000:0000:0000:0203:0204
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
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.203.204, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1203 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 444c.a873.5c75 10.10.203.204, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1203 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
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
BGP routing table entry for mac-ip 1303 0056.5656.5656 10.30.3.254, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 0056.5656.5656 10.30.4.254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2301 0015.0100.0002, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301
      VNI: 304 ESI: 0001:0203:0405:0607:0801
BGP routing table entry for mac-ip 2301 0015.0100.0002 20.30.1.32, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301
      VNI: 304 ESI: 0001:0203:0405:0607:0801
BGP routing table entry for mac-ip 2301 001b.0100.0002, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301
      VNI: 3856 ESI: 0001:0203:0405:0607:08cc
BGP routing table entry for mac-ip 2301 001b.0100.0002 20.30.1.33, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301
      VNI: 3856 ESI: 0001:0203:0405:0607:08cc
BGP routing table entry for mac-ip 2301 00aa.aaaa.aaaa, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 EvpnMacMobility:sticky
      VNI: 304 ESI: 0500:00fc:0000:0008:fd00
BGP routing table entry for mac-ip 2301 00aa.aaaa.aaaa 20.30.1.254, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301
      VNI: 304 ESI: 0500:00fc:0000:0008:fd00
BGP routing table entry for mac-ip 2301 60c7.8d2d.4416, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 EvpnMacMobility:sticky
      VNI: 304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2301 60c7.8d2d.4416 20.30.1.201, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301
      VNI: 304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2301 e4f2.7cef.a505, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 EvpnMacMobility:sticky
      VNI: 3856 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2301 e4f2.7cef.a505 20.30.1.200, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 EvpnMacMobility:sticky
      VNI: 3856 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2302 0015.0100.0003, Route Distinguisher: 100.0.37.9:2302
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302
      VNI: 336 ESI: 0001:0203:0405:0607:0801
BGP routing table entry for mac-ip 2302 0015.0100.0003 20.30.2.32, Route Distinguisher: 100.0.37.9:2302
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302
      VNI: 336 ESI: 0001:0203:0405:0607:0801
BGP routing table entry for mac-ip 2302 001b.0100.0003, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302
      VNI: 3904 ESI: 0001:0203:0405:0607:08cc
BGP routing table entry for mac-ip 2302 001b.0100.0003 20.30.2.33, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302
      VNI: 3904 ESI: 0001:0203:0405:0607:08cc
BGP routing table entry for mac-ip 2302 00aa.aaaa.aaaa, Route Distinguisher: 100.0.37.9:2302
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302 EvpnMacMobility:sticky
      VNI: 336 ESI: 0500:00fc:0000:0008:fe00
BGP routing table entry for mac-ip 2302 00aa.aaaa.aaaa 20.30.2.254, Route Distinguisher: 100.0.37.9:2302
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302
      VNI: 336 ESI: 0500:00fc:0000:0008:fe00
BGP routing table entry for mac-ip 2302 60c7.8d2d.4416, Route Distinguisher: 100.0.37.9:2302
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302 EvpnMacMobility:sticky
      VNI: 336 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2302 60c7.8d2d.4416 20.30.2.201, Route Distinguisher: 100.0.37.9:2302
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302
      VNI: 336 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2302 e4f2.7cef.a505, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302 EvpnMacMobility:sticky
      VNI: 3904 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2302 e4f2.7cef.a505 20.30.2.200, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302 EvpnMacMobility:sticky
      VNI: 3904 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2303 0013.0100.0004, Route Distinguisher: 100.0.0.4:2303
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2303:2303 Route-Origin-IP:100.0.0.34:0
      VNI: 770720 ESI: 0001:0203:0405:0607:0802
BGP routing table entry for mac-ip 2303 0013.0100.0004 20.30.3.4, Route Distinguisher: 100.0.0.4:2303
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2303:2303 Route-Origin-IP:100.0.0.34:0
      VNI: 770720 ESI: 0001:0203:0405:0607:0802
BGP routing table entry for mac-ip 2303 0015.0100.0004, Route Distinguisher: 100.0.37.9:2303
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 592 ESI: 0001:0203:0405:0607:0801
BGP routing table entry for mac-ip 2303 0015.0100.0004 20.30.3.32, Route Distinguisher: 100.0.37.9:2303
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 592 ESI: 0001:0203:0405:0607:0801
BGP routing table entry for mac-ip 2303 001b.0100.0004, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 3952 ESI: 0001:0203:0405:0607:08cc
BGP routing table entry for mac-ip 2303 001b.0100.0004 20.30.3.33, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 3952 ESI: 0001:0203:0405:0607:08cc
BGP routing table entry for mac-ip 2303 00aa.aaaa.aaaa, Route Distinguisher: 100.0.0.4:2303
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2303:2303 Route-Origin-IP:100.0.0.34:0 EvpnMacMobility:sticky
      VNI: 770720 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2303 00aa.aaaa.aaaa, Route Distinguisher: 100.0.37.9:2303
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 EvpnMacMobility:sticky
      VNI: 2608 ESI: 0500:00fc:0000:0008:ff00
BGP routing table entry for mac-ip 2303 00aa.aaaa.aaaa 20.30.3.254, Route Distinguisher: 100.0.37.9:2303
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 2608 ESI: 0500:00fc:0000:0008:ff00
BGP routing table entry for mac-ip 2303 60c7.8d2d.4416, Route Distinguisher: 100.0.37.9:2303
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 EvpnMacMobility:sticky
      VNI: 368 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2303 60c7.8d2d.4416 20.30.3.201, Route Distinguisher: 100.0.37.9:2303
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 368 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2303 e4f2.7cef.a505, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 EvpnMacMobility:sticky
      VNI: 3952 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2303 e4f2.7cef.a505 20.30.3.200, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 EvpnMacMobility:sticky
      VNI: 3952 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2304 0013.0100.0005, Route Distinguisher: 100.0.0.4:2303
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2303:2303 Route-Origin-IP:100.0.0.34:0
      VNI: 770816 ESI: 0001:0203:0405:0607:0802
BGP routing table entry for mac-ip 2304 0013.0100.0005 20.30.4.4, Route Distinguisher: 100.0.0.4:2303
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2303:2303 Route-Origin-IP:100.0.0.34:0
      VNI: 770816 ESI: 0001:0203:0405:0607:0802
BGP routing table entry for mac-ip 2304 0015.0100.0005, Route Distinguisher: 100.0.37.9:2303
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 592 ESI: 0001:0203:0405:0607:0801
BGP routing table entry for mac-ip 2304 0015.0100.0005 20.30.4.32, Route Distinguisher: 100.0.37.9:2303
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 592 ESI: 0001:0203:0405:0607:0801
BGP routing table entry for mac-ip 2304 001b.0100.0005, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 3968 ESI: 0001:0203:0405:0607:08cc
BGP routing table entry for mac-ip 2304 001b.0100.0005 20.30.4.33, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 3968 ESI: 0001:0203:0405:0607:08cc
BGP routing table entry for mac-ip 2304 00aa.aaaa.aaaa, Route Distinguisher: 100.0.0.4:2303
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2303:2303 Route-Origin-IP:100.0.0.34:0 EvpnMacMobility:sticky
      VNI: 770816 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2304 00aa.aaaa.aaaa, Route Distinguisher: 100.0.37.9:2303
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 EvpnMacMobility:sticky
      VNI: 2640 ESI: 0500:00fc:0000:0009:0000
BGP routing table entry for mac-ip 2304 00aa.aaaa.aaaa 20.30.4.254, Route Distinguisher: 100.0.37.9:2303
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 2640 ESI: 0500:00fc:0000:0009:0000
BGP routing table entry for mac-ip 2304 60c7.8d2d.4416, Route Distinguisher: 100.0.37.9:2303
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 EvpnMacMobility:sticky
      VNI: 368 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2304 60c7.8d2d.4416 20.30.4.201, Route Distinguisher: 100.0.37.9:2303
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 368 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2304 e4f2.7cef.a505, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 EvpnMacMobility:sticky
      VNI: 3968 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2304 e4f2.7cef.a505 20.30.4.200, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303 EvpnMacMobility:sticky
      VNI: 3968 ESI: 0000:0000:0000:0000:0000
```

## show bgp evpn route-type imet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
BGP routing table entry for imet 100.0.0.34, Route Distinguisher: 100.0.0.4:2301
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2301:2301 Route-Origin-IP:100.0.0.34:0
      VNI: 770609
      PMSI Tunnel: Ingress Replication, MPLS Label: 770609, Leaf Information Required: false, Tunnel ID: 100.0.0.34
BGP routing table entry for imet 100.0.0.34, Route Distinguisher: 100.0.0.4:2302
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2302:2302 Route-Origin-IP:100.0.0.34:0
      VNI: 770689
      PMSI Tunnel: Ingress Replication, MPLS Label: 770689, Leaf Information Required: false, Tunnel ID: 100.0.0.34
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
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan DF Election: Modulus-based Multicast Flags: IGMP proxy, OISM-supported, PEG, SBD
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
BGP routing table entry for imet 100.0.0.103, Route Distinguisher: 100.0.0.103:1
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (193.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan
      VNI: 1000
      PMSI Tunnel: Ingress Replication, MPLS Label: 1000, Leaf Information Required: false, Tunnel ID: 100.0.0.103
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
BGP routing table entry for imet 100.0.0.203, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan Multicast Flags: IGMP proxy, OISM-supported, SBD
      VNI: 1000
      PMSI Tunnel: Ingress Replication, MPLS Label: 1000, Leaf Information Required: false, Tunnel ID: 100.0.0.203
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
BGP routing table entry for imet 100.0.0.204, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan Multicast Flags: IGMP proxy, OISM-supported, SBD
      VNI: 1000
      PMSI Tunnel: Ingress Replication, MPLS Label: 1000, Leaf Information Required: false, Tunnel ID: 100.0.0.204
BGP routing table entry for imet 100.0.0.204, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
      PMSI Tunnel: Ingress Replication, MPLS Label: 1203, Leaf Information Required: false, Tunnel ID: 100.0.0.204
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
BGP routing table entry for imet 1303 100.0.0.56, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1303 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 100.0.0.201
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
BGP routing table entry for imet 1304 100.0.0.56, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan Multicast Flags: OISM-supported
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 1304 100.0.0.201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 100.0.0.201
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
BGP routing table entry for imet 2301 100.0.30.9, Route Distinguisher: 100.0.30.9:2301
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301
      VNI: 15737984
      PMSI Tunnel: Ingress Replication, MPLS Label: 15737984, Leaf Information Required: false, Tunnel ID: 100.0.30.9
BGP routing table entry for imet 2301 100.0.37.9, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301
      VNI: 2896
      PMSI Tunnel: Ingress Replication, MPLS Label: 2896, Leaf Information Required: false, Tunnel ID: 100.0.37.9
BGP routing table entry for imet 2302 100.0.30.9, Route Distinguisher: 100.0.30.9:2302
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302
      VNI: 15738000
      PMSI Tunnel: Ingress Replication, MPLS Label: 15738000, Leaf Information Required: false, Tunnel ID: 100.0.30.9
BGP routing table entry for imet 2302 100.0.37.9, Route Distinguisher: 100.0.37.9:2302
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2302:2302
      VNI: 2912
      PMSI Tunnel: Ingress Replication, MPLS Label: 2912, Leaf Information Required: false, Tunnel ID: 100.0.37.9
BGP routing table entry for imet 2303 100.0.0.34, Route Distinguisher: 100.0.0.4:2303
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2303:2303 Route-Origin-IP:100.0.0.34:0
      VNI: 770737
      PMSI Tunnel: Ingress Replication, MPLS Label: 770737, Leaf Information Required: false, Tunnel ID: 100.0.0.34
BGP routing table entry for imet 2303 100.0.30.9, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 15738016
      PMSI Tunnel: Ingress Replication, MPLS Label: 15738016, Leaf Information Required: false, Tunnel ID: 100.0.30.9
BGP routing table entry for imet 2303 100.0.37.9, Route Distinguisher: 100.0.37.9:2303
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 2928
      PMSI Tunnel: Ingress Replication, MPLS Label: 2928, Leaf Information Required: false, Tunnel ID: 100.0.37.9
BGP routing table entry for imet 2304 100.0.0.34, Route Distinguisher: 100.0.0.4:2303
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2303:2303 Route-Origin-IP:100.0.0.34:0
      VNI: 770833
      PMSI Tunnel: Ingress Replication, MPLS Label: 770833, Leaf Information Required: false, Tunnel ID: 100.0.0.34
BGP routing table entry for imet 2304 100.0.30.9, Route Distinguisher: 100.0.30.9:2303
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 15738032
      PMSI Tunnel: Ingress Replication, MPLS Label: 15738032, Leaf Information Required: false, Tunnel ID: 100.0.30.9
BGP routing table entry for imet 2304 100.0.37.9, Route Distinguisher: 100.0.37.9:2303
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2303:2303
      VNI: 2944
      PMSI Tunnel: Ingress Replication, MPLS Label: 2944, Leaf Information Required: false, Tunnel ID: 100.0.37.9
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
BGP routing table entry for ethernet-segment 0000:0000:0000:0000:0000 100.0.0.103, Route Distinguisher: 100.0.0.103:1
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (193.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:00:00:00:00
BGP routing table entry for ethernet-segment 0000:0000:0000:0111:0111 100.0.0.56, Route Distinguisher: 100.0.0.56:0
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: EvpnEsImportRt:00:00:00:00:00:01
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
BGP routing table entry for ip-prefix 10.10.103.103/32, Route Distinguisher: 100.0.0.103:1
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (193.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:02:00:00:01
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.202.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056 65202
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
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
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
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
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.40:1000
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.40:1000
 Paths: 1 available
  65040
    100.0.0.40 from 100.0.0.40 (100.0.0.40)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 20.10.4.0/24, Route Distinguisher: 100.0.0.4:2000
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 770528
BGP routing table entry for ip-prefix 20.10.32.0/24, Route Distinguisher: 100.0.37.9:2000
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 448
BGP routing table entry for ip-prefix 20.10.33.0/24, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 4032
BGP routing table entry for ip-prefix 20.10.108.0/24, Route Distinguisher: 3:2000
 Paths: 1 available
  65056 64512
    100.0.0.3 from 100.0.0.56 (100.0.0.56)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 992000
BGP routing table entry for ip-prefix 20.10.151.0/24, Route Distinguisher: 100.0.3.45:0
 Paths: 1 available
  65056 64512
    100.0.3.45 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 384128
BGP routing table entry for ip-prefix 20.10.151.0/24, Route Distinguisher: 100.0.3.48:0
 Paths: 1 available
  65056 64512
    100.0.3.48 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 384096
BGP routing table entry for ip-prefix 20.30.1.0/24, Route Distinguisher: 100.0.0.4:2000
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 770528
BGP routing table entry for ip-prefix 20.30.1.0/24, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 4032
BGP routing table entry for ip-prefix 20.30.1.0/24, Route Distinguisher: 100.0.37.9:2000
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 448
BGP routing table entry for ip-prefix 20.30.2.0/24, Route Distinguisher: 100.0.0.4:2000
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 770528
BGP routing table entry for ip-prefix 20.30.2.0/24, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 4032
BGP routing table entry for ip-prefix 20.30.2.0/24, Route Distinguisher: 100.0.37.9:2000
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 448
BGP routing table entry for ip-prefix 20.30.3.0/24, Route Distinguisher: 100.0.0.4:2000
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 770528
BGP routing table entry for ip-prefix 20.30.3.0/24, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 4032
BGP routing table entry for ip-prefix 20.30.3.0/24, Route Distinguisher: 100.0.37.9:2000
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 448
BGP routing table entry for ip-prefix 20.30.4.0/24, Route Distinguisher: 100.0.0.4:2000
 Paths: 1 available
  65056 64512
    100.0.0.34 from 100.0.0.56 (100.0.0.56)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 770528
BGP routing table entry for ip-prefix 20.30.4.0/24, Route Distinguisher: 100.0.30.9:2000
 Paths: 1 available
  65056 64512
    100.0.30.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 4032
BGP routing table entry for ip-prefix 20.30.4.0/24, Route Distinguisher: 100.0.37.9:2000
 Paths: 1 available
  65056 64512
    100.0.37.9 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 448
BGP routing table entry for ip-prefix 100.0.1.201/32, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65201
    100.0.0.201 from 100.0.0.201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:28:99:3a:8f:8f:6f
      VNI: 1000
BGP routing table entry for ip-prefix 100.0.1.202/32, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056 65202
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
BGP routing table entry for ip-prefix 100.0.1.203/32, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 100.0.1.204/32, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65204
    100.0.0.204 from 100.0.0.204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 100.9.9.0/24, Route Distinguisher: 100.0.3.60:0
 Paths: 1 available
  65056 64512
    100.0.3.60 from 100.0.0.56 (100.0.0.56)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1234:1234
      VNI: 384032
```

## show bgp evpn route-type smet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
BGP routing table entry for smet (S, G): (*, *) originating IP: 100.0.0.56, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan
      Multicast Flags: include
BGP routing table entry for smet (S, G): (*, 225.10.56.56) originating IP: 100.0.0.56, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan
      Multicast Flags: include
BGP routing table entry for smet (S, G): (*, 225.10.56.56) originating IP: 100.0.0.103, Route Distinguisher: 100.0.0.103:1
 Paths: 1 available
  65103
    100.0.0.103 from 100.0.0.103 (193.0.0.1)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan
      Multicast Flags: include
BGP routing table entry for smet (S, G): (*, 225.10.202.202) originating IP: 100.0.0.56, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan
      Multicast Flags: include
BGP routing table entry for smet (S, G): (*, 225.10.202.202) originating IP: 100.0.0.203, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65203
    100.0.0.203 from 100.0.0.203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan
      Multicast Flags: exclude
BGP routing table entry for smet (S, G): (*, 225.10.203.203) originating IP: 100.0.0.56, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    100.0.0.56 from 100.0.0.56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan
      Multicast Flags: include
BGP routing table entry for smet (S, G): (10.10.103.103, 225.10.203.203) originating IP: 100.0.0.206, Route Distinguisher: 100.0.0.206:1000
 Paths: 1 available
  65206
    100.0.0.206 from 100.0.0.206 (100.0.0.206)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan
      Multicast Flags: include
BGP routing table entry for smet (S, G): (10.10.203.203, 225.10.203.203) originating IP: 100.0.0.206, Route Distinguisher: 100.0.0.206:1000
 Paths: 1 available
  65206
    100.0.0.206 from 100.0.0.206 (100.0.0.206)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan
      Multicast Flags: include
```

## show bgp evpn route-type spmsi detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
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
 C        20.200.203.0/24
           directly connected, Ethernet3
 C        20.200.204.0/24
           directly connected, Ethernet4
 C        20.200.206.0/24
           directly connected, Ethernet5
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
20.200.201.201    0:00:25  2899.3a8f.8f6f  Ethernet1
20.200.203.203    0:00:18  3838.a621.e82f  Ethernet3
20.200.204.204    0:00:11  985d.82a2.04f9  Ethernet4
20.200.206.206    0:00:26  985d.82c4.0271  Ethernet5
20.56.200.56      0:00:18  407c.7dc4.ab9d  Ethernet11
20.103.200.103    0:00:05  0011.0100.0001  Ethernet12
20.45.200.45      0:00:21  6c31.0e7b.8b87  Ethernet13
20.46.200.46      0:00:24  6c31.0eb7.505f  Ethernet14
20.40.200.40      0:00:20  246c.8474.8ddb  Ethernet15
20.42.200.42      0:00:02  4014.827b.84ab  Ethernet16
20.44.200.40      0:00:19  5c5a.c773.4abb  Ethernet17
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
 C        20.200.203.0/24
           directly connected, Ethernet3
 C        20.200.204.0/24
           directly connected, Ethernet4
 C        20.200.206.0/24
           directly connected, Ethernet5
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
10.10.22.254      3:08:59  00aa.aaaa.aaaa  Vlan1022, not learned

VRF: 1040
Address         Age (sec)  Hardware Addr   Interface
10.10.40.254      1:32:57  00aa.aaaa.aaaa  Vlan1040, not learned

VRF: 1042
Address         Age (sec)  Hardware Addr   Interface
10.10.42.254      1:06:19  00aa.aaaa.aaaa  Vlan1042, not learned

VRF: 1044
Address         Age (sec)  Hardware Addr   Interface

VRF: 1045
Address         Age (sec)  Hardware Addr   Interface
10.10.45.254      1:40:34  00aa.aaaa.aaaa  Vlan1045, not learned

VRF: 1056
Address         Age (sec)  Hardware Addr   Interface
10.10.56.254      0:41:53  00aa.aaaa.aaaa  Vlan1056, not learned

VRF: 1201
Address         Age (sec)  Hardware Addr   Interface
10.10.201.254     1:43:15  00aa.aaaa.aaaa  Vlan1201, not learned

VRF: 1203
Address         Age (sec)  Hardware Addr   Interface
10.10.203.254     3:34:22  00aa.aaaa.aaaa  Vlan1203, not learned

VRF: 1301
Address         Age (sec)  Hardware Addr   Interface
10.30.1.254       2:19:58  00aa.aaaa.aaaa  Vlan1301, not learned

VRF: 1301-201
Address         Age (sec)  Hardware Addr   Interface

VRF: 1301-203
Address         Age (sec)  Hardware Addr   Interface

VRF: 1302
Address         Age (sec)  Hardware Addr   Interface
10.30.2.254       3:12:47  00aa.aaaa.aaaa  Vlan1302, not learned

VRF: 1302-201
Address         Age (sec)  Hardware Addr   Interface

VRF: 1302-203
Address         Age (sec)  Hardware Addr   Interface

VRF: 1303
Address         Age (sec)  Hardware Addr   Interface
10.30.3.254       2:29:34  00aa.aaaa.aaaa  Vlan1303, not learned

VRF: 1303-201
Address         Age (sec)  Hardware Addr   Interface

VRF: 1303-203
Address         Age (sec)  Hardware Addr   Interface

VRF: 1304
Address         Age (sec)  Hardware Addr   Interface
10.30.4.254       1:22:21  00aa.aaaa.aaaa  Vlan1304, Ethernet48

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
20.200.201.201    0:00:25  2899.3a8f.8f6f  Ethernet1
20.200.203.203    0:00:19  3838.a621.e82f  Ethernet3
20.200.204.204    0:00:11  985d.82a2.04f9  Ethernet4
20.200.206.206    0:00:27  985d.82c4.0271  Ethernet5
20.56.200.56      0:00:19  407c.7dc4.ab9d  Ethernet11
20.103.200.103    0:00:06  0011.0100.0001  Ethernet12
20.45.200.45      0:00:21  6c31.0e7b.8b87  Ethernet13
20.46.200.46      0:00:24  6c31.0eb7.505f  Ethernet14
20.40.200.40      0:00:20  246c.8474.8ddb  Ethernet15
20.42.200.42      0:00:02  4014.827b.84ab  Ethernet16
20.44.200.40      0:00:20  5c5a.c773.4abb  Ethernet17

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.20.2      0:00:41  bcea.fa02.6ce2  Management1
192.168.20.18     0:00:10  e484.29cd.e801  Management1
192.168.20.19     0:01:42  c407.7858.8001  Management1
192.168.20.21     0:01:05  7081.85c1.b801  Management1
192.168.20.22     0:03:07  c407.780a.9f04  Management1
192.168.20.23     0:03:07  c407.780a.7750  Management1
192.168.20.24     0:02:18  6c87.2089.ede5  Management1
192.168.20.25     0:01:36  6c87.2089.ece5  Management1
192.168.20.28     0:03:19  98a9.2d59.bae6  Management1
192.168.20.52     0:03:13  f83e.95dc.1289  Management1
192.168.21.47     0:04:20  5c5a.c7ff.8a0a  Management1
192.168.21.50     0:03:07  a84f.b1a5.5221  Management1
192.168.21.59     0:00:23  6607.f5d1.ae16  Management1

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
1040    246c.8474.8de0    DYNAMIC     Et48       1       1 day, 22:16:58 ago
1040    444c.a873.5c75    STATIC      Router
1042    4014.827b.84b0    DYNAMIC     Et48       1       1 day, 22:09:34 ago
1042    444c.a873.5c75    STATIC      Router
1045    0026.f002.0000    DYNAMIC     Et48       1       1 day, 22:29:26 ago
1045    444c.a873.5c75    STATIC      Router
1056    0014.0100.0001    DYNAMIC     Et48       1       0:39:43 ago
1056    0056.5656.5656    DYNAMIC     Et48       1       0:41:52 ago
1056    444c.a873.5c75    STATIC      Router
1201    444c.a873.5c75    STATIC      Router
1201    7483.ef0b.a4fb    DYNAMIC     Et48       1       18:32:17 ago
1203    0015.0100.0001    DYNAMIC     Et48       1       18:21:28 ago
1203    3838.a621.e82f    DYNAMIC     Et48       1       19:15:59 ago
1203    444c.a873.5c75    STATIC      Router
1203    985d.82a2.04f9    DYNAMIC     Et48       1       19:15:10 ago
1301    444c.a873.5c75    STATIC      Router
1301    7483.ef0b.a4fb    DYNAMIC     Et48       1       18:32:17 ago
1302    444c.a873.5c75    STATIC      Router
1302    7483.ef0b.a4fb    DYNAMIC     Et48       1       18:32:17 ago
1303    444c.a873.5c75    STATIC      Router
1303    7483.ef0b.a4fb    DYNAMIC     Et48       1       18:32:17 ago
1304    00aa.aaaa.aaaa    DYNAMIC     Et48       1       0:00:40 ago
1304    444c.a873.5c75    STATIC      Router
1304    7483.ef0b.a4fb    DYNAMIC     Et48       1       18:32:17 ago
Total Mac Addresses for this criterion: 25

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show l2rib output detail

```text
7483.ef0b.a4fb, VLAN 1301, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
7483.ef0b.a4fb, VLAN 1201, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
985d.82a2.04f9, VLAN 1203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
7483.ef0b.a4fb, VLAN 1303, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
3838.a621.e82f, VLAN 1203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
4014.827b.84b0, VLAN 1042, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0015.0100.0001, VLAN 1203, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0014.0100.0001, VLAN 1056, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
7483.ef0b.a4fb, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
00aa.aaaa.aaaa, VLAN 1304, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
7483.ef0b.a4fb, VLAN 1302, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
   Ethernet48
0056.5656.5656, VLAN 1056, seq 1, pref 16, learnedDynamicMac, source: Local Dynamic
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
Et3       A-PE13-203    0:01      0.0   0.0%        0      1.0   0.0%        1
Et4       A-PE14-204    0:01      3.0   0.0%        2      0.0   0.0%        0
Et5       A-PE16-206    0:01      0.0   0.0%        0      1.0   0.0%        1
Et11      Nokia-56      0:05      2.0   0.0%        1      1.9   0.0%        2
Et12      Keysight-103  0:05      0.9   0.0%        1      2.0   0.0%        1
Et48      Spine-host    0:05      4.1   0.1%        6      0.0   0.0%        0
Ma1                     0:05      0.2   0.0%        0     13.4   1.4%        1
```

