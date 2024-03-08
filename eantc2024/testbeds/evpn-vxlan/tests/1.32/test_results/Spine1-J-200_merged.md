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
  Description              Neighbor       V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  Cisco-41                 20.41.200.41   4 64512            127       145    0    0 00:19:59 Estab   1      1
  NOkia                    20.56.200.56   4 64512              0         0    0    0 00:27:45 Connect
  ANET-PE15                20.200.206.206 4 65206           1474      1476    0    0 19:17:53 Estab   3      3
                           100.0.0.56     4 64512              0         0    0    0 00:30:48 Active
                           100.0.3.41     4 64512            181      2862    0    0 00:19:52 Estab(NotNegotiated)
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.200, local AS number 65000
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
                           100.0.0.56  4 64512              0         0    0    0 00:30:48 Active
  ANET-PE15                100.0.0.206 4 65206           1453      6210    0    0 20:16:06 Estab   3      3
                           100.0.3.41  4 64512            181      2862    0    0 00:19:53 Estab   7      7
  H3C-22.EVPN              2000::22    4 65022           2198      6569    0    0 19:17:41 Estab   22     22
  H3C-23.EVPN              2000::23    4 65023           2185      6796    0    0 01:50:06 Estab   22     22
  CSCO-40.EVPN             2000::40    4 65040           1379      7351    0    0 19:04:37 Estab   15     15
  CSCO-42.EVPN             2000::42    4 65042           1376      7456    0    0 19:03:24 Estab   15     15
  CSCO-45.EVPN             2000::45    4 65045           1401      7227    0    0 19:01:33 Estab   12     12
  CSCO-46.EVPN             2000::46    4 65045           1416      7244    0    0 19:00:14 Estab   12     12
  ANET-201.EVPN            2000::201   4 65201           1930      7095    0    0 19:17:43 Estab   32     32
  ANET-202.EVPN            2000::202   4 65202           1961      7170    0    0 19:17:43 Estab   32     32
  ANET-203.EVPN            2000::203   4 65203           3167      6014    0    0 19:17:45 Estab   29     29
  ANET-204.EVPN            2000::204   4 65204           3033      6032    0    0 19:17:43 Estab   31     31
  NOK-56.EVPN              2001::56    4 65056           4069      9130    0    0 19:17:43 Estab   73     73
```

## show bgp evpn route-type auto-discovery detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
BGP routing table entry for auto-discovery 0 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
BGP routing table entry for auto-discovery 0 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 0 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1022
 Paths: 1 available
  65023
    2000::23 from 2000::23 (100.0.0.23)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
BGP routing table entry for auto-discovery 0 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1301
 Paths: 1 available
  65023
    2000::23 from 2000::23 (100.0.0.23)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1302
 Paths: 1 available
  65023
    2000::23 from 2000::23 (100.0.0.23)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1303
 Paths: 1 available
  65023
    2000::23 from 2000::23 (100.0.0.23)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1304
 Paths: 1 available
  65023
    2000::23 from 2000::23 (100.0.0.23)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1022
 Paths: 1 available
  65023
    2000::23 from 2000::23 (100.0.0.23)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1301
 Paths: 1 available
  65023
    2000::23 from 2000::23 (100.0.0.23)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1302
 Paths: 1 available
  65023
    2000::23 from 2000::23 (100.0.0.23)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1303
 Paths: 1 available
  65023
    2000::23 from 2000::23 (100.0.0.23)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0022:0023, Route Distinguisher: 100.0.0.23:1304
 Paths: 1 available
  65023
    2000::23 from 2000::23 (100.0.0.23)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:0000:0000:0123:0123, Route Distinguisher: 100.0.0.4:2301
 Paths: 1 available
  65056 64512
    100.0.0.34 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2301:2301 Route-Origin-IP:100.0.0.34:0
      VNI: 769952
BGP routing table entry for auto-discovery 0 0000:0000:0000:0123:0123, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  65056 64512
    100.0.37.9 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301
      VNI: 5728
BGP routing table entry for auto-discovery 0000:0000:0000:0123:0123, Route Distinguisher: 100.0.37.9:0
 Paths: 1 available
  65056 64512
    100.0.37.9 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 EvpnEsiLabel:375
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0201:0202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
BGP routing table entry for auto-discovery 0 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1303 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 1304 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
BGP routing table entry for auto-discovery 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.203:1
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0000:0000:0000:0203:0204, Route Distinguisher: 100.0.0.204:1
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 Route-Target-AS:1301:1301 Route-Target-AS:1302:1302 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:0
      VNI: 0
BGP routing table entry for auto-discovery 0 0011:1111:2222:2211:1111, Route Distinguisher: 100.0.3.41:3311
 Paths: 1 available
  64512
    100.0.3.41 from 100.0.3.41 (100.0.3.41)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:3301:3301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:00:00:00:00:00
      VNI: 3301
BGP routing table entry for auto-discovery 0011:1111:2222:2211:1111, Route Distinguisher: 100.0.3.41:2
 Paths: 1 available
  64512
    100.0.3.41 from 100.0.3.41 (100.0.3.41)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:3301:3301 TunnelEncap:tunnelTypeVxlan EvpnEsiLabel:24002 800a:0x04 0x64 0x00 0x03 0x29 0x80
      VNI: 0
BGP routing table entry for auto-discovery 0500:00fc:0000:0008:fd00, Route Distinguisher: 100.0.37.9:0
 Paths: 1 available
  65056 64512
    100.0.37.9 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 EvpnEsiLabel:372
      VNI: 0
```

## show bgp evpn route-type mac-ip detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
BGP routing table entry for mac-ip 0000.0181.0181, Route Distinguisher: 100.0.3.41:3311
 Paths: 1 available
  64512
    100.0.3.41 from 100.0.3.41 (100.0.3.41)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Community: 1:5641
      Extended Community: Route-Target-AS:3301:3301 TunnelEncap:tunnelTypeVxlan TunnelEncap:tunnelTypeMpls EvpnMacMobility:sticky EvpnRouterMac:00:00:00:00:00:00
      VNI: 3301 ESI: 0011:1111:2222:2211:1111
      D-PATH: 1:1:EVPN
BGP routing table entry for mac-ip 0000.0206.0206, Route Distinguisher: 100.0.0.206:3301
 Paths: 1 available
  65206
    100.0.0.206 from 100.0.0.206 (100.0.0.206)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:3301:3301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 3301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0020.1000.0001, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0001, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0001 1000:3000:1::201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0001 1000:3000:1::201, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7 EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0002, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0002, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0002 1000:3000:2::201, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83 EvpnNdFlags:pflag
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0002 1000:3000:2::201, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0005, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0005, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0005 1000:1000:201::201, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1201:1201 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1201 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.1000.0005 1000:1000:201::201, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7 EvpnNdFlags:pflag
      VNI: 1201 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 0020.3000.0001, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0001 1000:3000:1::203, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f EvpnNdFlags:pflag
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0001 1000:3000:1::203, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0002, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0002 1000:3000:2::203, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0002 1000:3000:2::203, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9 EvpnNdFlags:pflag
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0005, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0005 1000:1000:203::203, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f EvpnNdFlags:pflag
      VNI: 1203 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0020.3000.0005 1000:1000:203::203, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1203 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 0022.0000.0001 1000:3000:1::22, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:5 EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 0022.0000.0005 1000:1000:22::22, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1022 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 0022.0000.0005 fe80::222:ff:fe00:5, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:c4:07:78:0a:9f:31
      VNI: 1022 L3 VNI: 1000 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 0040.0100.0001, Route Distinguisher: 100.0.0.40:34068
 Paths: 1 available
  65040
    2000::40 from 2000::40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0040.0100.0001 1000:3000:1::40, Route Distinguisher: 100.0.0.40:34068
 Paths: 1 available
  65040
    2000::40 from 2000::40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0040.0100.0001 1000:3000:1:0:240:1ff:fe00:1, Route Distinguisher: 100.0.0.40:34068
 Paths: 1 available
  65040
    2000::40 from 2000::40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0040.0100.0002, Route Distinguisher: 100.0.0.40:34069
 Paths: 1 available
  65040
    2000::40 from 2000::40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0040.0100.0002 1000:3000:2::40, Route Distinguisher: 100.0.0.40:34069
 Paths: 1 available
  65040
    2000::40 from 2000::40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0040.0100.0002 1000:3000:2:0:240:1ff:fe00:2, Route Distinguisher: 100.0.0.40:34069
 Paths: 1 available
  65040
    2000::40 from 2000::40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0040.0100.0003, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65040
    2000::40 from 2000::40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan
      VNI: 1040 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0040.0100.0003 1000:1000:40::40, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65040
    2000::40 from 2000::40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1040 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0040.0100.0003 1000:1000:40:0:240:1ff:fe00:3, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65040
    2000::40 from 2000::40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:24:6c:84:74:8d:db
      VNI: 1040 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0042.0100.0001, Route Distinguisher: 100.0.0.42:34068
 Paths: 1 available
  65042
    2000::42 from 2000::42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0042.0100.0001 1000:3000:1::42, Route Distinguisher: 100.0.0.42:34068
 Paths: 1 available
  65042
    2000::42 from 2000::42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0042.0100.0001 1000:3000:1:0:242:1ff:fe00:1, Route Distinguisher: 100.0.0.42:34068
 Paths: 1 available
  65042
    2000::42 from 2000::42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0042.0100.0002, Route Distinguisher: 100.0.0.42:34069
 Paths: 1 available
  65042
    2000::42 from 2000::42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0042.0100.0002 1000:3000:2::42, Route Distinguisher: 100.0.0.42:34069
 Paths: 1 available
  65042
    2000::42 from 2000::42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0042.0100.0002 1000:3000:2:0:242:1ff:fe00:2, Route Distinguisher: 100.0.0.42:34069
 Paths: 1 available
  65042
    2000::42 from 2000::42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0042.0100.0003, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65042
    2000::42 from 2000::42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan
      VNI: 1042 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0042.0100.0003 1000:1000:42::42, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65042
    2000::42 from 2000::42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1042 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0042.0100.0003 1000:1000:42:0:242:1ff:fe00:3, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65042
    2000::42 from 2000::42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:40:14:82:7b:84:ab
      VNI: 1042 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0001, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65045
    2000::100 from 2000::45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0001, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65045
    2000::100 from 2000::46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0001 1000:3000:1::45, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65045
    2000::100 from 2000::45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0001 1000:3000:1::45, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65045
    2000::100 from 2000::46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1301 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0002, Route Distinguisher: 100.0.0.45:34069
 Paths: 1 available
  65045
    2000::100 from 2000::45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0002, Route Distinguisher: 100.0.0.46:34069
 Paths: 1 available
  65045
    2000::100 from 2000::46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0002 1000:3000:2::45, Route Distinguisher: 100.0.0.45:34069
 Paths: 1 available
  65045
    2000::100 from 2000::45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0002 1000:3000:2::45, Route Distinguisher: 100.0.0.46:34069
 Paths: 1 available
  65045
    2000::100 from 2000::46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1302 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0003, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65045
    2000::100 from 2000::45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0003, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65045
    2000::100 from 2000::46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan
      VNI: 1045 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0003 1000:1000:45::45, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65045
    2000::100 from 2000::45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0045.0100.0003 1000:1000:45::45, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65045
    2000::100 from 2000::46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:06:00:00:00:01:00
      VNI: 1045 L3 VNI: 1000 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0001, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0001 1000:3000:1::56, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0001 fe80::256:ff:fe00:1, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0002, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0002 1000:3000:2::56, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0002 fe80::256:ff:fe00:2, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0005, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0005 1000:1000:56::56, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 0056.0000.0005 fe80::256:ff:fe00:5, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa, Route Distinguisher: 100.0.0.4:2301
 Paths: 1 available
  65056 64512
    100.0.0.34 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2301:2301 Route-Origin-IP:100.0.0.34:0 EvpnMacMobility:sticky
      VNI: 769952 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.10.56.254, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.1.254, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 10.30.2.254, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 1000:1000:56::254, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 1000:3000:1::254, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa 1000:3000:2::254, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa fe80::2aa:aaff:feaa:aaaa, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1056 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa fe80::2aa:aaff:feaa:aaaa, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1301 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 00aa.aaaa.aaaa fe80::2aa:aaff:feaa:aaaa, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1302 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 0020.1000.0003, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0020.1000.0003, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0020.1000.0003 1000:3000:3::201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0020.1000.0003 1000:3000:3::201, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7 EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1303 0020.3000.0003, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0020.3000.0003, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0020.3000.0003 1000:3000:3::203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f EvpnNdFlags:pflag
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0020.3000.0003 1000:3000:3::203, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1303 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1303 0022.0000.0003, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0022:0023
BGP routing table entry for mac-ip 1303 0056.0000.0003, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 0056.0000.0003 1000:3000:3::56, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 0056.0000.0003 fe80::256:ff:fe00:3, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 10.30.3.254, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa 1000:3000:3::254, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1303 00aa.aaaa.aaaa fe80::2aa:aaff:feaa:aaaa, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1303 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 0020.1000.0004, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0020.1000.0004, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0020.1000.0004 1000:3000:4::201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0020.1000.0004 1000:3000:4::201, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7 EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0201:0202
BGP routing table entry for mac-ip 1304 0020.3000.0004, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 0020.3000.0004 1000:3000:4::203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f EvpnNdFlags:pflag
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 0020.3000.0004 1000:3000:4::203, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1304 L3 VNI: 1000 ESI: 0000:0000:0000:0203:0204
BGP routing table entry for mac-ip 1304 0056.0000.0004, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 0056.0000.0004 1000:3000:4::56, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 0056.0000.0004 fe80::256:ff:fe00:4, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 10.30.4.254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa 1000:3000:4::254, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 1304 00aa.aaaa.aaaa fe80::2aa:aaff:feaa:aaaa, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan EvpnMacMobility:sticky
      VNI: 1304 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2301 0012.0100.0002, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  65056 64512
    100.0.37.9 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301
      VNI: 5728 ESI: 0000:0000:0000:0123:0123
BGP routing table entry for mac-ip 2301 0012.0100.0002 20.30.1.68, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  65056 64512
    100.0.37.9 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301
      VNI: 5728 ESI: 0000:0000:0000:0123:0123
BGP routing table entry for mac-ip 2301 00aa.aaaa.aaaa, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  65056 64512
    100.0.37.9 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 EvpnMacMobility:sticky
      VNI: 5728 ESI: 0500:00fc:0000:0008:fd00
BGP routing table entry for mac-ip 2301 00aa.aaaa.aaaa 20.30.1.254, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  65056 64512
    100.0.37.9 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301
      VNI: 5728 ESI: 0500:00fc:0000:0008:fd00
BGP routing table entry for mac-ip 2301 60c7.8d2d.4416, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  65056 64512
    100.0.37.9 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 EvpnMacMobility:sticky
      VNI: 5728 ESI: 0000:0000:0000:0000:0000
BGP routing table entry for mac-ip 2301 60c7.8d2d.4416 20.30.1.201, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  65056 64512
    100.0.37.9 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301 EvpnMacMobility:sticky
      VNI: 5728 ESI: 0000:0000:0000:0000:0000
```

## show bgp evpn route-type imet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1022
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
      PMSI Tunnel: Ingress Replication, MPLS Label: 1022, Leaf Information Required: false, Tunnel ID: 2000::22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1301
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::22
BGP routing table entry for imet 100.0.0.22, Route Distinguisher: 100.0.0.22:1302
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::22
BGP routing table entry for imet 100.0.0.23, Route Distinguisher: 100.0.0.23:1022
 Paths: 1 available
  65023
    2000::23 from 2000::23 (100.0.0.23)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1022:1022 TunnelEncap:tunnelTypeVxlan
      VNI: 1022
      PMSI Tunnel: Ingress Replication, MPLS Label: 1022, Leaf Information Required: false, Tunnel ID: 2000::23
BGP routing table entry for imet 100.0.0.23, Route Distinguisher: 100.0.0.23:1301
 Paths: 1 available
  65023
    2000::23 from 2000::23 (100.0.0.23)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::23
BGP routing table entry for imet 100.0.0.23, Route Distinguisher: 100.0.0.23:1302
 Paths: 1 available
  65023
    2000::23 from 2000::23 (100.0.0.23)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::23
BGP routing table entry for imet 100.0.0.34, Route Distinguisher: 100.0.0.4:2301
 Paths: 1 available
  65056 64512
    100.0.0.34 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000 Route-Target-AS:2301:2301 Route-Origin-IP:100.0.0.34:0
      VNI: 769969
      PMSI Tunnel: Ingress Replication, MPLS Label: 769969, Leaf Information Required: false, Tunnel ID: 100.0.0.34
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:1103
 Paths: 1 available
  65056
    100.0.0.56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:1103:1103 TunnelEncap:tunnelTypeVxlan
      VNI: 1103
      PMSI Tunnel: Ingress Replication, MPLS Label: 1103, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.56, Route Distinguisher: 100.0.0.56:3301
 Paths: 1 available
  65056
    100.0.0.56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Community: 1:5641
      Extended Community: Route-Target-AS:3301:3301 TunnelEncap:tunnelTypeVxlan
      VNI: 3301
      PMSI Tunnel: Ingress Replication, MPLS Label: 3301, Leaf Information Required: false, Tunnel ID: 100.0.0.56
BGP routing table entry for imet 100.0.0.206, Route Distinguisher: 100.0.0.206:3301
 Paths: 1 available
  65206
    100.0.0.206 from 100.0.0.206 (100.0.0.206)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:3301:3301 TunnelEncap:tunnelTypeVxlan
      VNI: 3301
      PMSI Tunnel: Ingress Replication, MPLS Label: 3301, Leaf Information Required: false, Tunnel ID: 100.0.0.206
BGP routing table entry for imet 100.0.3.41, Route Distinguisher: 100.0.3.41:3311
 Paths: 1 available
  64512
    100.0.3.41 from 100.0.3.41 (100.0.3.41)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:3301:3301 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:00:00:00:00:00 L2 Attributes: control word
      VNI: 3301
      PMSI Tunnel: Ingress Replication, MPLS Label: 3301, Leaf Information Required: false, Tunnel ID: 100.0.3.41
BGP routing table entry for imet 2000::40, Route Distinguisher: 100.0.0.40:33807
 Paths: 1 available
  65040
    2000::40 from 2000::40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1040:1040 TunnelEncap:tunnelTypeVxlan
      VNI: 1040
      PMSI Tunnel: Ingress Replication, MPLS Label: 1040, Leaf Information Required: false, Tunnel ID: 2000::40
BGP routing table entry for imet 2000::40, Route Distinguisher: 100.0.0.40:34068
 Paths: 1 available
  65040
    2000::40 from 2000::40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::40
BGP routing table entry for imet 2000::40, Route Distinguisher: 100.0.0.40:34069
 Paths: 1 available
  65040
    2000::40 from 2000::40 (100.0.0.40)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::40
BGP routing table entry for imet 2000::42, Route Distinguisher: 100.0.0.42:33809
 Paths: 1 available
  65042
    2000::42 from 2000::42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1042:1042 TunnelEncap:tunnelTypeVxlan
      VNI: 1042
      PMSI Tunnel: Ingress Replication, MPLS Label: 1042, Leaf Information Required: false, Tunnel ID: 2000::42
BGP routing table entry for imet 2000::42, Route Distinguisher: 100.0.0.42:34068
 Paths: 1 available
  65042
    2000::42 from 2000::42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::42
BGP routing table entry for imet 2000::42, Route Distinguisher: 100.0.0.42:34069
 Paths: 1 available
  65042
    2000::42 from 2000::42 (100.0.0.42)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::42
BGP routing table entry for imet 2000::56, Route Distinguisher: 100.0.0.56:1056
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1056:1056 TunnelEncap:tunnelTypeVxlan
      VNI: 1056
      PMSI Tunnel: Ingress Replication, MPLS Label: 1056, Leaf Information Required: false, Tunnel ID: 2000::56
BGP routing table entry for imet 2000::56, Route Distinguisher: 100.0.0.56:1301
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::56
BGP routing table entry for imet 2000::56, Route Distinguisher: 100.0.0.56:1302
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::56
BGP routing table entry for imet 2000::100, Route Distinguisher: 100.0.0.45:33812
 Paths: 1 available
  65045
    2000::100 from 2000::45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan
      VNI: 1045
      PMSI Tunnel: Ingress Replication, MPLS Label: 1045, Leaf Information Required: false, Tunnel ID: 2000::100
BGP routing table entry for imet 2000::100, Route Distinguisher: 100.0.0.45:34068
 Paths: 1 available
  65045
    2000::100 from 2000::45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::100
BGP routing table entry for imet 2000::100, Route Distinguisher: 100.0.0.45:34069
 Paths: 1 available
  65045
    2000::100 from 2000::45 (100.0.0.45)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::100
BGP routing table entry for imet 2000::100, Route Distinguisher: 100.0.0.46:33812
 Paths: 1 available
  65045
    2000::100 from 2000::46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1045:1045 TunnelEncap:tunnelTypeVxlan
      VNI: 1045
      PMSI Tunnel: Ingress Replication, MPLS Label: 1045, Leaf Information Required: false, Tunnel ID: 2000::100
BGP routing table entry for imet 2000::100, Route Distinguisher: 100.0.0.46:34068
 Paths: 1 available
  65045
    2000::100 from 2000::46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::100
BGP routing table entry for imet 2000::100, Route Distinguisher: 100.0.0.46:34069
 Paths: 1 available
  65045
    2000::100 from 2000::46 (100.0.0.46)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::100
BGP routing table entry for imet 2000::201, Route Distinguisher: 100.0.0.201:1201
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
      PMSI Tunnel: Ingress Replication, MPLS Label: 1201, Leaf Information Required: false, Tunnel ID: 2000::201
BGP routing table entry for imet 2000::201, Route Distinguisher: 100.0.0.201:1301
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::201
BGP routing table entry for imet 2000::201, Route Distinguisher: 100.0.0.201:1302
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::201
BGP routing table entry for imet 2000::202, Route Distinguisher: 100.0.0.202:1201
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1201:1201 TunnelEncap:tunnelTypeVxlan
      VNI: 1201
      PMSI Tunnel: Ingress Replication, MPLS Label: 1201, Leaf Information Required: false, Tunnel ID: 2000::202
BGP routing table entry for imet 2000::202, Route Distinguisher: 100.0.0.202:1301
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::202
BGP routing table entry for imet 2000::202, Route Distinguisher: 100.0.0.202:1302
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::202
BGP routing table entry for imet 2000::203, Route Distinguisher: 100.0.0.203:1203
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
      PMSI Tunnel: Ingress Replication, MPLS Label: 1203, Leaf Information Required: false, Tunnel ID: 2000::203
BGP routing table entry for imet 2000::203, Route Distinguisher: 100.0.0.203:1301
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::203
BGP routing table entry for imet 2000::203, Route Distinguisher: 100.0.0.203:1302
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::203
BGP routing table entry for imet 2000::204, Route Distinguisher: 100.0.0.204:1203
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1203:1203 TunnelEncap:tunnelTypeVxlan
      VNI: 1203
      PMSI Tunnel: Ingress Replication, MPLS Label: 1203, Leaf Information Required: false, Tunnel ID: 2000::204
BGP routing table entry for imet 2000::204, Route Distinguisher: 100.0.0.204:1301
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1301:1301 TunnelEncap:tunnelTypeVxlan
      VNI: 1301
      PMSI Tunnel: Ingress Replication, MPLS Label: 1301, Leaf Information Required: false, Tunnel ID: 2000::204
BGP routing table entry for imet 2000::204, Route Distinguisher: 100.0.0.204:1302
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1302:1302 TunnelEncap:tunnelTypeVxlan
      VNI: 1302
      PMSI Tunnel: Ingress Replication, MPLS Label: 1302, Leaf Information Required: false, Tunnel ID: 2000::204
BGP routing table entry for imet 1303 100.0.0.22, Route Distinguisher: 100.0.0.22:1303
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 2000::22
BGP routing table entry for imet 1303 100.0.0.23, Route Distinguisher: 100.0.0.23:1303
 Paths: 1 available
  65023
    2000::23 from 2000::23 (100.0.0.23)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 2000::23
BGP routing table entry for imet 1303 2000::56, Route Distinguisher: 100.0.0.56:1303
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 2000::56
BGP routing table entry for imet 1303 2000::201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 2000::201
BGP routing table entry for imet 1303 2000::202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 2000::202
BGP routing table entry for imet 1303 2000::203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 2000::203
BGP routing table entry for imet 1303 2000::204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1303
      PMSI Tunnel: Ingress Replication, MPLS Label: 1303, Leaf Information Required: false, Tunnel ID: 2000::204
BGP routing table entry for imet 1304 100.0.0.22, Route Distinguisher: 100.0.0.22:1304
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 2000::22
BGP routing table entry for imet 1304 100.0.0.23, Route Distinguisher: 100.0.0.23:1304
 Paths: 1 available
  65023
    2000::23 from 2000::23 (100.0.0.23)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 2000::23
BGP routing table entry for imet 1304 2000::56, Route Distinguisher: 100.0.0.56:1304
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 2000::56
BGP routing table entry for imet 1304 2000::201, Route Distinguisher: 100.0.0.201:1303
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 2000::201
BGP routing table entry for imet 1304 2000::202, Route Distinguisher: 100.0.0.202:1303
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 2000::202
BGP routing table entry for imet 1304 2000::203, Route Distinguisher: 100.0.0.203:1303
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 2000::203
BGP routing table entry for imet 1304 2000::204, Route Distinguisher: 100.0.0.204:1303
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1303:1303 TunnelEncap:tunnelTypeVxlan
      VNI: 1304
      PMSI Tunnel: Ingress Replication, MPLS Label: 1304, Leaf Information Required: false, Tunnel ID: 2000::204
BGP routing table entry for imet 2301 100.0.37.9, Route Distinguisher: 100.0.37.9:2301
 Paths: 1 available
  65056 64512
    100.0.37.9 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2301:2301
      VNI: 5968
      PMSI Tunnel: Ingress Replication, MPLS Label: 5968, Leaf Information Required: false, Tunnel ID: 100.0.37.9
```

## show bgp evpn route-type ethernet-segment detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
BGP routing table entry for ethernet-segment 0000:0000:0000:0022:0023 100.0.0.22, Route Distinguisher: 100.0.0.22:0
 Paths: 1 available
  65022
    2000::22 from 2000::22 (100.0.0.22)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: EvpnEsImportRt:00:00:00:00:00:00 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0022:0023 100.0.0.23, Route Distinguisher: 100.0.0.23:0
 Paths: 1 available
  65023
    2000::23 from 2000::23 (100.0.0.23)
      Origin IGP, metric 0, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: EvpnEsImportRt:00:00:00:00:00:00 DF Election: Preference 100
BGP routing table entry for ethernet-segment 0000:0000:0000:0123:0123 100.0.37.9, Route Distinguisher: 100.0.37.9:0
 Paths: 1 available
  65056 64512
    100.0.37.9 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: EvpnEsImportRt:00:00:00:00:00:01
BGP routing table entry for ethernet-segment 0000:0000:0000:0201:0202 2000::201, Route Distinguisher: 100.0.0.201:1
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:10:02:02 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0201:0202 2000::202, Route Distinguisher: 100.0.0.202:1
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:10:02:02 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0203:0204 2000::203, Route Distinguisher: 100.0.0.203:1
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:30:02:04 DF Election: Preference 200
BGP routing table entry for ethernet-segment 0000:0000:0000:0203:0204 2000::204, Route Distinguisher: 100.0.0.204:1
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: TunnelEncap:tunnelTypeVxlan EvpnEsImportRt:00:00:20:30:02:04 DF Election: Preference 100
BGP routing table entry for ethernet-segment 0011:1111:2222:2211:1111 100.0.0.56, Route Distinguisher: 100.0.0.56:0
 Paths: 1 available
  65056
    100.0.0.56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: EvpnEsImportRt:11:11:11:22:22:22
BGP routing table entry for ethernet-segment 0011:1111:2222:2211:1111 100.0.3.41, Route Distinguisher: 100.0.3.41:0
 Paths: 2 available
  64512
    100.0.3.41 from 100.0.3.41 (100.0.3.41)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: EvpnEsImportRt:11:11:11:22:22:22 DF Election: Modulus-based
  65056 64512
    100.0.3.41 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external
      Extended Community: EvpnEsImportRt:11:11:11:22:22:22 DF Election: Modulus-based
BGP routing table entry for ethernet-segment 0048:5648:5648:5648:5648 100.0.0.56, Route Distinguisher: 100.0.0.56:0
 Paths: 1 available
  65056
    100.0.0.56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: EvpnEsImportRt:48:56:48:56:48:56
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
BGP routing table entry for ip-prefix 10.10.56.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.201.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.10.203.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.1.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.2.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.3.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.56:1000
 Paths: 1 available
  65056
    2000::56 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:00:01:00:00:00:56
      VNI: 1000
      D-PATH: 2:2:None
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.201:1000
 Paths: 1 available
  65201
    2000::201 from 2000::201 (100.0.0.201)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 Route-Target-AS:65205:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:22:83
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.202:1000
 Paths: 1 available
  65202
    2000::202 from 2000::202 (100.0.0.202)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:2c:dd:e9:0b:25:b7
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.203:1000
 Paths: 1 available
  65203
    2000::203 from 2000::203 (100.0.0.203)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:38:38:a6:21:e8:2f
      VNI: 1000
BGP routing table entry for ip-prefix 10.30.4.0/24, Route Distinguisher: 100.0.0.204:1000
 Paths: 1 available
  65204
    2000::204 from 2000::204 (100.0.0.204)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1000:1000 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:a2:04:f9
      VNI: 1000
BGP routing table entry for ip-prefix 20.30.1.0/24, Route Distinguisher: 100.0.0.4:2000
 Paths: 1 available
  65056 64512
    100.0.0.34 from 2001::56 (100.0.0.56)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 770096
BGP routing table entry for ip-prefix 20.30.1.0/24, Route Distinguisher: 100.0.37.9:2000
 Paths: 1 available
  65056 64512
    100.0.37.9 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 5760
BGP routing table entry for ip-prefix 20.30.1.201/32, Route Distinguisher: 100.0.37.9:2000
 Paths: 1 available
  65056 64512
    100.0.37.9 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 5760
BGP routing table entry for ip-prefix 20.30.1.254/32, Route Distinguisher: 100.0.37.9:2000
 Paths: 1 available
  65056 64512
    100.0.37.9 from 2001::56 (100.0.0.56)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, external
      Extended Community: Route-Target-AS:2000:2000
      VNI: 5760
BGP routing table entry for ip-prefix 30.30.1.0/24, Route Distinguisher: 100.0.0.26:1000
 Paths: 1 available
  65206
    100.0.0.206 from 100.0.0.206 (100.0.0.206)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Extended Community: Route-Target-AS:1023:1023 TunnelEncap:tunnelTypeVxlan EvpnRouterMac:98:5d:82:c4:02:71
      VNI: 1000
BGP routing table entry for ip-prefix 30.30.1.0/24, Route Distinguisher: 100.0.3.41:0
 Paths: 1 available
  64512
    100.0.3.41 from 100.0.3.41 (100.0.3.41)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Community: 1:5641
      Extended Community: Route-Target-AS:1023:1023 TunnelEncap:tunnelTypeVxlan TunnelEncap:tunnelTypeMpls EvpnRouterMac:f8:7a:41:6d:d0:f0
      VNI: 1000
      D-PATH: 1:1:EVPN
BGP routing table entry for ip-prefix 30.30.2.0/24, Route Distinguisher: 100.0.3.41:0
 Paths: 1 available
  64512
    100.0.3.41 from 100.0.3.41 (100.0.3.41)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, external, best
      Community: 1:5641
      Extended Community: Route-Target-AS:1023:1023 TunnelEncap:tunnelTypeVxlan TunnelEncap:tunnelTypeMpls EvpnRouterMac:f8:7a:41:6d:d0:f0
      VNI: 1000
      D-PATH: 1:1:EVPN
```

## show bgp evpn route-type smet detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
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

 B E      10.10.206.0/24 [20/0]
           via 20.200.206.206, Ethernet6
 C        20.41.200.0/24
           directly connected, Ethernet23
 C        20.56.200.0/24
           directly connected, Ethernet11
 C        20.200.206.0/24
           directly connected, Ethernet6
 C        100.0.0.200/32
           directly connected, Loopback0
 B E      100.0.0.206/32 [20/0]
           via 20.200.206.206, Ethernet6
 B E      100.0.3.41/32 [20/0]
           via 20.41.200.41, Ethernet23

```

## show ip arp

```text
Address         Age (sec)  Hardware Addr   Interface
20.200.206.206    0:00:09  985d.82c4.0271  Ethernet6
20.56.200.56      1:05:11  407c.7dc4.ab9d  Ethernet11
20.41.200.41      0:00:50  f87a.4118.8ab5  Ethernet23
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

 B E      10.10.206.0/24 [20/0]
           via 20.200.206.206, Ethernet6
 C        20.41.200.0/24
           directly connected, Ethernet23
 C        20.56.200.0/24
           directly connected, Ethernet11
 C        20.200.206.0/24
           directly connected, Ethernet6
 C        100.0.0.200/32
           directly connected, Loopback0
 B E      100.0.0.206/32 [20/0]
           via 20.200.206.206, Ethernet6
 B E      100.0.3.41/32 [20/0]
           via 20.41.200.41, Ethernet23


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
20.200.206.206    0:00:09  985d.82c4.0271  Ethernet6
20.56.200.56      1:05:12  407c.7dc4.ab9d  Ethernet11
20.41.200.41      0:00:50  f87a.4118.8ab5  Ethernet23

VRF: mgmt
Address         Age (sec)  Hardware Addr   Interface
192.168.20.1      0:00:00  90e2.bac7.8074  Management1
192.168.20.201    0:03:20  2cdd.e90b.2282  Management1
192.168.21.50     0:02:49  a84f.b1a5.5221  Management1
192.168.21.59     0:00:35  6607.f5d1.ae16  Management1
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
Router identifier 100.0.0.200, local AS number 65000
```

## show bgp evpn instance

```text
```

## show ipv6 interface brief

```text
Interface  Status    MTU  IPv6 Address                  Addr State  Addr Source
---------- ------- ------ ----------------------------- ----------- -----------
Et1        up       1500  fe80::464c:a8ff:fe73:5c75/64  up          link local 
Et2        up       1500  fe80::464c:a8ff:fe73:5c75/64  up          link local 
Et3        up       1500  fe80::464c:a8ff:fe73:5c75/64  up          link local 
Et4        up       1500  fe80::464c:a8ff:fe73:5c75/64  up          link local 
Et11       up       1500  fe80::464c:a8ff:fe73:5c75/64  up          link local 
Et12       up       1500  fe80::464c:a8ff:fe73:5c75/64  up          link local 
Et13       up       1500  fe80::464c:a8ff:fe73:5c75/64  up          link local 
Et14       up       1500  fe80::464c:a8ff:fe73:5c75/64  up          link local 
Et15       up       1500  fe80::464c:a8ff:fe73:5c75/64  up          link local 
Et16       up       1500  fe80::464c:a8ff:fe73:5c75/64  up          link local 
Et24       up       1500  fe80::464c:a8ff:fe73:5c75/64  up          link local 
Et25       up       1500  fe80::464c:a8ff:fe73:5c75/64  up          link local 
Et26       up       1500  fe80::464c:a8ff:fe73:5c75/64  up          link local 
Lo0        up      65535  fe80::ff:fe00:0/64            up          link local 
                          2000::200/128                 up          config     

```

## show ipv6 bgp summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.200, local AS number 65000
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor                       V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
                           fe80::266c:84ff:fe74:8ddc%Et15 4 65040           1149      1369    0    0 19:04:49 Estab   1      1
                           fe80::2edd:e9ff:fe0b:2283%Et1  4 65201           1572      1659    0    0 19:17:52 Estab   1      1
                           fe80::2edd:e9ff:fe0b:25b7%Et2  4 65202           1583      1679    0    0 19:17:52 Estab   1      1
                           fe80::3a38:a6ff:fe21:e82f%Et3  4 65203           1587      1666    0    0 19:17:52 Estab   1      1
                           fe80::4214:82ff:fe7b:84ac%Et16 4 65042           1148      1372    0    0 19:03:36 Estab   1      1
                           fe80::427c:7dff:fec4:ab9d%Et11 4 65056           2657      3173    0    0 19:17:52 Estab   2      2
                           fe80::6e31:eff:fe7b:8b88%Et13  4 65045           1153      1364    0    0 19:01:44 Estab   3      3
                           fe80::6e31:eff:feb7:5060%Et14  4 65045           1157      1363    0    0 19:00:26 Estab   3      3
                           fe80::9a5d:82ff:fea2:4f9%Et4   4 65204           1589      1675    0    0 19:17:52 Estab   1      1
                           fe80::c607:78ff:fe0a:777d%Et25 4 65023            138       145    0    0 01:50:14 Estab   1      1
                           fe80::c607:78ff:fe0a:9f31%Et26 4 65022             71        81    0    0 00:53:33 Estab   1      1
```

## show ipv6 bgp

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
RPKI Origin Validation codes: V - valid, I - invalid, U - unknown
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
 * >      2000::22/128           fe80::c607:78ff:fe0a:9f31%Et26 0       -          100     0       65022 i
 * >      2000::23/128           fe80::c607:78ff:fe0a:777d%Et25 0       -          100     0       65023 i
 * >      2000::40/128           fe80::266c:84ff:fe74:8ddc%Et15 0       -          100     0       65040 ?
 * >      2000::42/128           fe80::4214:82ff:fe7b:84ac%Et16 0       -          100     0       65042 ?
 * >Ec    2000::45/128           fe80::6e31:eff:fe7b:8b88%Et13 0       -          100     0       65045 ?
 *  ec    2000::45/128           fe80::6e31:eff:feb7:5060%Et14 0       -          100     0       65045 ?
 * >Ec    2000::46/128           fe80::6e31:eff:feb7:5060%Et14 0       -          100     0       65045 ?
 *  ec    2000::46/128           fe80::6e31:eff:fe7b:8b88%Et13 0       -          100     0       65045 ?
 * >      2000::56/128           fe80::427c:7dff:fec4:ab9d%Et11 0       -          100     0       65056 ?
 * >Ec    2000::100/128          fe80::6e31:eff:fe7b:8b88%Et13 0       -          100     0       65045 ?
 *  ec    2000::100/128          fe80::6e31:eff:feb7:5060%Et14 0       -          100     0       65045 ?
 * >      2000::200/128          -                     -       -          -       0       i
 * >      2000::201/128          fe80::2edd:e9ff:fe0b:2283%Et1 0       -          100     0       65201 i
 * >      2000::202/128          fe80::2edd:e9ff:fe0b:25b7%Et2 0       -          100     0       65202 i
 * >      2000::203/128          fe80::3a38:a6ff:fe21:e82f%Et3 0       -          100     0       65203 i
 * >      2000::204/128          fe80::9a5d:82ff:fea2:4f9%Et4 0       -          100     0       65204 i
 * >      2001::56/128           fe80::427c:7dff:fec4:ab9d%Et11 0       -          100     0       65056 i
```

## show ipv6 route

```text

VRF: default
Displaying 14 of 17 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 B E      2000::22/128 [20/0]
           via fe80::c607:78ff:fe0a:9f31, Ethernet26
 B E      2000::23/128 [20/0]
           via fe80::c607:78ff:fe0a:777d, Ethernet25
 B E      2000::40/128 [20/0]
           via fe80::266c:84ff:fe74:8ddc, Ethernet15
 B E      2000::42/128 [20/0]
           via fe80::4214:82ff:fe7b:84ac, Ethernet16
 B E      2000::45/128 [20/0]
           via fe80::6e31:eff:fe7b:8b88, Ethernet13
           via fe80::6e31:eff:feb7:5060, Ethernet14
 B E      2000::46/128 [20/0]
           via fe80::6e31:eff:fe7b:8b88, Ethernet13
           via fe80::6e31:eff:feb7:5060, Ethernet14
 B E      2000::56/128 [20/0]
           via fe80::427c:7dff:fec4:ab9d, Ethernet11
 B E      2000::100/128 [20/0]
           via fe80::6e31:eff:fe7b:8b88, Ethernet13
           via fe80::6e31:eff:feb7:5060, Ethernet14
 C        2000::200/128 [0/0]
           via Loopback0, directly connected
 B E      2000::201/128 [20/0]
           via fe80::2edd:e9ff:fe0b:2283, Ethernet1
 B E      2000::202/128 [20/0]
           via fe80::2edd:e9ff:fe0b:25b7, Ethernet2
 B E      2000::203/128 [20/0]
           via fe80::3a38:a6ff:fe21:e82f, Ethernet3
 B E      2000::204/128 [20/0]
           via fe80::9a5d:82ff:fea2:4f9, Ethernet4
 B E      2001::56/128 [20/0]
           via fe80::427c:7dff:fec4:ab9d, Ethernet11

```

## show ipv6 bgp vrf all

```text
BGP routing table information for VRF default
Router identifier 100.0.0.200, local AS number 65000
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
RPKI Origin Validation codes: V - valid, I - invalid, U - unknown
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
 * >      2000::22/128           fe80::c607:78ff:fe0a:9f31%Et26 0       -          100     0       65022 i
 * >      2000::23/128           fe80::c607:78ff:fe0a:777d%Et25 0       -          100     0       65023 i
 * >      2000::40/128           fe80::266c:84ff:fe74:8ddc%Et15 0       -          100     0       65040 ?
 * >      2000::42/128           fe80::4214:82ff:fe7b:84ac%Et16 0       -          100     0       65042 ?
 * >Ec    2000::45/128           fe80::6e31:eff:fe7b:8b88%Et13 0       -          100     0       65045 ?
 *  ec    2000::45/128           fe80::6e31:eff:feb7:5060%Et14 0       -          100     0       65045 ?
 * >Ec    2000::46/128           fe80::6e31:eff:feb7:5060%Et14 0       -          100     0       65045 ?
 *  ec    2000::46/128           fe80::6e31:eff:fe7b:8b88%Et13 0       -          100     0       65045 ?
 * >      2000::56/128           fe80::427c:7dff:fec4:ab9d%Et11 0       -          100     0       65056 ?
 * >Ec    2000::100/128          fe80::6e31:eff:fe7b:8b88%Et13 0       -          100     0       65045 ?
 *  ec    2000::100/128          fe80::6e31:eff:feb7:5060%Et14 0       -          100     0       65045 ?
 * >      2000::200/128          -                     -       -          -       0       i
 * >      2000::201/128          fe80::2edd:e9ff:fe0b:2283%Et1 0       -          100     0       65201 i
 * >      2000::202/128          fe80::2edd:e9ff:fe0b:25b7%Et2 0       -          100     0       65202 i
 * >      2000::203/128          fe80::3a38:a6ff:fe21:e82f%Et3 0       -          100     0       65203 i
 * >      2000::204/128          fe80::9a5d:82ff:fea2:4f9%Et4 0       -          100     0       65204 i
 * >      2001::56/128           fe80::427c:7dff:fec4:ab9d%Et11 0       -          100     0       65056 i
```

## show ipv6 route vrf all

```text

VRF: default
Displaying 14 of 17 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 B E      2000::22/128 [20/0]
           via fe80::c607:78ff:fe0a:9f31, Ethernet26
 B E      2000::23/128 [20/0]
           via fe80::c607:78ff:fe0a:777d, Ethernet25
 B E      2000::40/128 [20/0]
           via fe80::266c:84ff:fe74:8ddc, Ethernet15
 B E      2000::42/128 [20/0]
           via fe80::4214:82ff:fe7b:84ac, Ethernet16
 B E      2000::45/128 [20/0]
           via fe80::6e31:eff:fe7b:8b88, Ethernet13
           via fe80::6e31:eff:feb7:5060, Ethernet14
 B E      2000::46/128 [20/0]
           via fe80::6e31:eff:fe7b:8b88, Ethernet13
           via fe80::6e31:eff:feb7:5060, Ethernet14
 B E      2000::56/128 [20/0]
           via fe80::427c:7dff:fec4:ab9d, Ethernet11
 B E      2000::100/128 [20/0]
           via fe80::6e31:eff:fe7b:8b88, Ethernet13
           via fe80::6e31:eff:feb7:5060, Ethernet14
 C        2000::200/128 [0/0]
           via Loopback0, directly connected
 B E      2000::201/128 [20/0]
           via fe80::2edd:e9ff:fe0b:2283, Ethernet1
 B E      2000::202/128 [20/0]
           via fe80::2edd:e9ff:fe0b:25b7, Ethernet2
 B E      2000::203/128 [20/0]
           via fe80::3a38:a6ff:fe21:e82f, Ethernet3
 B E      2000::204/128 [20/0]
           via fe80::9a5d:82ff:fea2:4f9, Ethernet4
 B E      2001::56/128 [20/0]
           via fe80::427c:7dff:fec4:ab9d, Ethernet11


VRF: mgmt
Displaying 0 of 3 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route


! IPv6 routing not enabled
```

## show bgp ipv6 unicast summary lldp

```text
BGP summary information for VRF default
Router identifier 100.0.0.200, local AS number 65000
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor                       LLDP Neighbor                  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
                           fe80::266c:84ff:fe74:8ddc%Et15 Cisco_40_N9K-C93180YC-FX3      4 65040           1149      1370    0    0 19:04:50 Estab   1      1
                           fe80::2edd:e9ff:fe0b:2283%Et1  PE11-JP-201.ns.eantc.de        4 65201           1572      1659    0    0 19:17:53 Estab   1      1
                           fe80::2edd:e9ff:fe0b:25b7%Et2  PE12-JP-202.ns.eantc.de        4 65202           1583      1679    0    0 19:17:53 Estab   1      1
                           fe80::3a38:a6ff:fe21:e82f%Et3  PE13-T3-203.ns.eantc.de        4 65203           1587      1666    0    0 19:17:53 Estab   1      1
                           fe80::4214:82ff:fe7b:84ac%Et16 Cisco_42_N9K-C93400LD-H1       4 65042           1148      1372    0    0 19:03:37 Estab   1      1
                           fe80::427c:7dff:fec4:ab9d%Et11 185b.0089.c3cc                 4 65056           2657      3173    0    0 19:17:53 Estab   2      2
                           fe80::6e31:eff:fe7b:8b88%Et13  Cisco_45_N9K-C93240YC-FX2      4 65045           1153      1364    0    0 19:01:45 Estab   3      3
                           fe80::6e31:eff:feb7:5060%Et14  Cisco_46_N9K-C93240YC-FX2      4 65045           1157      1363    0    0 19:00:27 Estab   3      3
                           fe80::9a5d:82ff:fea2:4f9%Et4   PE14-T3-204.ns.eantc.de        4 65204           1589      1675    0    0 19:17:53 Estab   1      1
                           fe80::c607:78ff:fe0a:777d%Et25 h3c_23_S6850-56HF              4 65023            138       145    0    0 01:50:15 Estab   1      1
                           fe80::c607:78ff:fe0a:9f31%Et26 h3c_22_S6850-56HF              4 65022             71        81    0    0 00:53:34 Estab   1      1
```

## show ipv6 neighbors vrf all

```text

VRF: default
IPv6 Address                                  Age Hardware Addr   Interface
fe80::2edd:e9ff:fe0b:2283                 0:00:03 2cdd.e90b.2283  Et1
fe80::2edd:e9ff:fe0b:25b7                 0:00:15 2cdd.e90b.25b7  Et2
fe80::3a38:a6ff:fe21:e82f                 0:00:10 3838.a621.e82f  Et3
fe80::9a5d:82ff:fea2:4f9                  0:00:13 985d.82a2.04f9  Et4
fe80::427c:7dff:fec4:ab9d                 0:00:21 407c.7dc4.ab9d  Et11
fe80::6e31:eff:fe7b:8b88                  0:00:34 6c31.0e7b.8b87  Et13
fe80::6e31:eff:feb7:5060                  0:00:27 6c31.0eb7.505f  Et14
fe80::266c:84ff:fe74:8ddc                 0:00:16 246c.8474.8ddb  Et15
fe80::4214:82ff:fe7b:84ac                 0:00:08 4014.827b.84ab  Et16
fe80::c607:78ff:fe0a:777d                 0:00:04 c407.780a.777d  Et25
fe80::c607:78ff:fe0a:9f31                 0:00:12 c407.780a.9f31  Et26

VRF: mgmt
IPv6 Address                                  Age Hardware Addr   Interface
```

## show ipv6 neighbors remote

```text
ARP remote bindings
VLAN IP Address MAC Address    Source         
---- ---------- -------------- ---------------
```

## show ipv6 nd ra neighbors

```text
VRF: default
   Interface              IPv6 Address           Last RA Received
---------------- ------------------------------- ----------------
   Ethernet1        fe80::2edd:e9ff:fe0b:2283      0:02:02 ago   
   Ethernet2        fe80::2edd:e9ff:fe0b:25b7      0:01:31 ago   
   Ethernet3        fe80::3a38:a6ff:fe21:e82f      0:02:42 ago   
   Ethernet4        fe80::9a5d:82ff:fea2:4f9       0:02:38 ago   
   Ethernet11       fe80::427c:7dff:fec4:ab9d      0:00:06 ago   
   Ethernet13       fe80::6e31:eff:fe7b:8b88       0:00:03 ago   
   Ethernet14       fe80::6e31:eff:feb7:5060       0:00:02 ago   
   Ethernet15       fe80::266c:84ff:fe74:8ddc      0:00:01 ago   
   Ethernet16       fe80::4214:82ff:fe7b:84ac      0:00:01 ago   
   Ethernet25       fe80::c607:78ff:fe0a:777d      0:07:15 ago   
   Ethernet26       fe80::c607:78ff:fe0a:9f31      0:02:16 ago   

```

## show ipv6 nd ra neighbors vrf tenant-a

```text
```

## show interfaces counters rates | nz

```text
Port      Name         Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Et1       A-PE11-201    0:01      0.3   0.0%        0      0.4   0.0%        0
Et2       A-PE12-202    0:01      0.2   0.0%        0      0.2   0.0%        0
Et3       A-PE13-203    0:01      0.3   0.0%        0      0.3   0.0%        0
Et4       A-PE14-204    0:01      0.2   0.0%        0      0.3   0.0%        0
Et11      Nokia-56      0:01      0.8   0.0%        0      0.9   0.0%        0
Et13      Cisco-45-N9K  0:01      0.2   0.0%        0      0.1   0.0%        0
Et14      Cisco-46-N9K  0:01      0.2   0.0%        0      0.1   0.0%        0
Et15      Cisco-40-N9K  0:01      0.2   0.0%        0      0.2   0.0%        0
Et16      Cisco-42-N9K  0:01      0.2   0.0%        0      0.2   0.0%        0
Et24      JNPR 314      0:01      0.0   0.0%        0      0.0   0.0%        0
Ma1                     0:01      0.1   0.0%        0      0.2   0.0%        0
```

