# Test results for PE41-J2-161

## show interfaces status

```text
Port       Name   Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1               notconnect   1        full   25G    Not Present                    
Et2               notconnect   1        full   25G    Not Present                    
Et3               notconnect   1        full   25G    Not Present                    
Et4               notconnect   1        full   25G    Not Present                    
Et5               connected    1        full   10G    10GBASE-SRL                    
Et6               notconnect   1        full   25G    Not Present                    
Et7               notconnect   1        full   25G    Not Present                    
Et8               notconnect   1        full   25G    Not Present                    
Et9               notconnect   1        full   25G    Not Present                    
Et10              connected    routed   full   10G    10GBASE-SR                     
Et11              connected    trunk    full   10G    10GBASE-LR                     
Et12              notconnect   1        full   25G    Not Present                    
Et13              notconnect   1        full   25G    Not Present                    
Et14              notconnect   1        full   25G    Not Present                    
Et15              notconnect   1        full   25G    Not Present                    
Et16              notconnect   1        full   25G    Not Present                    
Et17              notconnect   1        full   25G    Not Present                    
Et18              notconnect   1        full   25G    Not Present                    
Et19              notconnect   1        full   25G    Not Present                    
Et20              connected    routed   full   10G    10GBASE-SRL                    
Et21              notconnect   1        full   25G    Not Present                    
Et22              notconnect   1        full   25G    Not Present                    
Et23              notconnect   1        full   25G    Not Present                    
Et24              notconnect   1        full   25G    Not Present                    
Et25              notconnect   1        full   25G    Not Present                    
Et26              notconnect   1        full   25G    Not Present                    
Et27              notconnect   1        full   25G    Not Present                    
Et28              notconnect   1        full   25G    Not Present                    
Et29              notconnect   1        full   25G    Not Present                    
Et30              notconnect   1        full   25G    Not Present                    
Et31              notconnect   1        full   25G    Not Present                    
Et32              notconnect   1        full   25G    Not Present                    
Et33              notconnect   1        full   25G    Not Present                    
Et34              notconnect   1        full   25G    Not Present                    
Et35              notconnect   1        full   25G    Not Present                    
Et36              notconnect   1        full   25G    Not Present                    
Et37              errdisabled  1        full   25G    Not Present                    
Et38              errdisabled  1        full   25G    Not Present                    
Et39              connected    1        full   10G    10GBASE-SRL                    
Et40              connected    1        full   10G    10GBASE-SRL                    
Et41/1            notconnect   1        full   100G   Not Present                    
Et42/1            notconnect   1        full   100G   Not Present                    
Et43/1            notconnect   1        full   100G   Not Present                    
Et44/1            notconnect   1        full   100G   Not Present                    
Et45/1            notconnect   1        full   100G   Not Present                    
Et46/1            notconnect   1        full   100G   Not Present                    
Ma1               connected    routed   a-full a-1G   10/100/1000                    

```

## show lldp neighbors

```text
Last table change time   : 5:14:33 ago
Number of table inserts  : 8
Number of table deletes  : 1
Number of table drops    : 0
Number of table age-outs : 0

Port          Neighbor Device ID               Neighbor Port ID    TTL
---------- -------------------------------- ---------------------- ---
Et5           Harness3-J-175.ns.eantc.de       Ethernet3           120
Et10          Cisco342-9902                    TenGigE0/0/0/12     120
Et11          JNPR-398-QFX5120                 546                 120
Et20          Nokia-59-IXRe2                   1610899777          121
Et39          PE42-J2-162.ns.eantc.de          Ethernet39          120
Et40          PE42-J2-162.ns.eantc.de          Ethernet40          120
Ma1           extreme-x460-1                   42                  120

```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
srv6      default  Cisco342-9902    L2   Ethernet10         P2P               UP    29          00                  
srv6      default  Nokia-59-IXRe2   L2   Ethernet20         P2P               UP    27          00                  
```

## show tunnel fib

```text

Type 'SRv6 Transport', index 102, endpoint fcbb:0:1344::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 105, endpoint fcbb:0:336::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 106, endpoint fcbb:0:59::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 108, endpoint fcbb:0:352::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 112, endpoint fcbb:0:342::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 116, endpoint fcbb:0:1353::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 117, endpoint fcbb:0:36::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 118, endpoint fcbb:0:20::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 129, endpoint fcbb:0:28::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 137, endpoint fcbb:0:1338::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 138, endpoint fcbb:0:1029::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 139, endpoint fcbb:0:1199::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 143, endpoint fcbb:0:1058::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 144, endpoint fcbb:0:1310::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 145, endpoint fcbb:0:307::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 147, endpoint fcbb:0:419::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 148, endpoint fcbb:0:1011::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 152, endpoint fcbb:0:316::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 162, endpoint fcbb:0:1302::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 163, endpoint fcbb:0:1162::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161
```

## show bgp vpn-ipv4

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 1011:1 IPv4 prefix 20.11.225.0/24
                                 2002::11              -       100     0       ? Or-ID: 10.0.0.11 C-LST: 100.0.0.53 
 * >      RD: 1:20 IPv4 prefix 20.20.225.0/24
                                 2002::20              0       100     0       ? Or-ID: 10.0.0.20 C-LST: 100.0.0.53 
 * >      RD: 1:28 IPv4 prefix 20.28.225.0/24
                                 2002::28              0       100     0       ? Or-ID: 192.168.20.28 C-LST: 100.0.0.53 
 * >      RD: 1:29 IPv4 prefix 20.29.225.0/24
                                 2002::29              0       100     0       ? Or-ID: 192.168.20.29 C-LST: 100.0.0.53 
 * >      RD: 1:36 IPv4 prefix 20.36.225.0/24
                                 2002::36              0       100     0       ? Or-ID: 192.168.20.36 C-LST: 100.0.0.53 
   %      RD: 1:49 IPv4 prefix 20.49.225.0/24
                                 2002::49              0       100     0       ? Or-ID: 10.0.0.49 C-LST: 100.0.0.53 
 * >      RD: 1:58 IPv4 prefix 20.58.225.0/24
                                 2002::58              -       100     0       i Or-ID: 10.0.0.58 C-LST: 100.0.0.53 
 * >      RD: 1:59 IPv4 prefix 20.59.225.0/24
                                 2002::59              -       100     0       i Or-ID: 10.0.0.59 C-LST: 100.0.0.53 
 * >      RD: 1:302 IPv4 prefix 20.102.225.0/24
                                 2002::302             -       100     0       i Or-ID: 10.0.1.2 C-LST: 100.0.0.53 
 * >      RD: 1:307 IPv4 prefix 20.107.225.0/24
                                 2002::307             -       100     0       i Or-ID: 10.0.1.7 C-LST: 100.0.0.53 
 * >      RD: 1:310 IPv4 prefix 20.110.225.0/24
                                 2002::310             -       100     0       i Or-ID: 10.0.1.10 C-LST: 100.0.0.53 
 * >      RD: 1:316 IPv4 prefix 20.116.225.0/24
                                 2002::316             -       100     0       i Or-ID: 10.0.1.16 C-LST: 100.0.0.53 
 * >      RD: 1:336 IPv4 prefix 20.136.225.0/24
                                 2002::336             -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
 * >      RD: 1:338 IPv4 prefix 20.138.225.0/24
                                 2002::338             -       100     0       ? Or-ID: 10.0.1.38 C-LST: 100.0.0.53 
 * >      RD: 1:342 IPv4 prefix 20.142.225.0/24
                                 2002::342             0       100     0       ? Or-ID: 100.0.0.42 C-LST: 100.0.0.53 
 * >      RD: 1:344 IPv4 prefix 20.144.225.0/24
                                 2002::344             0       100     0       ? Or-ID: 100.0.0.44 C-LST: 100.0.0.53 
 * >      RD: 1:352 IPv4 prefix 20.152.225.0/24
                                 2002::352             0       100     0       ? Or-ID: 100.0.0.52 C-LST: 100.0.0.53 
 * >      RD: 1:353 IPv4 prefix 20.153.225.0/24
                                 2002::353             0       100     0       ?
 * >      RD: 1:161 IPv4 prefix 20.161.225.0/24
                                 -                     -       -       0       i
 * >      RD: 1:1162 IPv4 prefix 20.162.225.0/24
                                 2002::162             -       100     0       i Or-ID: 100.0.0.162 C-LST: 100.0.0.53 
 * >      RD: 1:199 IPv4 prefix 20.199.225.0/24
                                 2002::199             0       100     0       ? Or-ID: 20.49.199.199 C-LST: 100.0.0.53 
 * >      RD: 1:419 IPv4 prefix 20.219.225.0/24
                                 2002::419             -       0       0       i Or-ID: 10.0.1.219 C-LST: 100.0.0.53 
```

## show bgp vpn-ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
BGP routing table entry for IPv4 prefix 20.11.225.0/24, Route Distinguisher: 1011:1
 Paths: 1 available
  Local
    2002::11 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.0.11, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1011:e001::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.20.225.0/24, Route Distinguisher: 1:20
 Paths: 1 available
  Local
    2002::20 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.0.20, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:20:e100::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.28.225.0/24, Route Distinguisher: 1:28
 Paths: 1 available
  Local
    2002::28 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 192.168.20.28, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:28:e100::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.29.225.0/24, Route Distinguisher: 1:29
 Paths: 1 available
  Local
    2002::29 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 192.168.20.29, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1029:e100::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.36.225.0/24, Route Distinguisher: 1:36
 Paths: 1 available
  Local
    2002::36 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 192.168.20.36, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:36:e13f::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.49.225.0/24, Route Distinguisher: 1:49
 Paths: 1 available
  Local
    2002::49 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, invalid, internal, pending resolution
      Originator: 10.0.0.49, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote MPLS label: 0
BGP routing table entry for IPv4 prefix 20.58.225.0/24, Route Distinguisher: 1:58
 Paths: 1 available
  Local
    2002::58 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.0.58, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1058:e017::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.59.225.0/24, Route Distinguisher: 1:59
 Paths: 1 available
  Local
    2002::59 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.0.59, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:59:e017::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.102.225.0/24, Route Distinguisher: 1:302
 Paths: 1 available
  Local
    2002::302 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.1.2, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1302:e000::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.107.225.0/24, Route Distinguisher: 1:307
 Paths: 1 available
  Local
    2002::307 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.1.7, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:307:e000::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.110.225.0/24, Route Distinguisher: 1:310
 Paths: 1 available
  Local
    2002::310 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.1.10, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1310:e000::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.116.225.0/24, Route Distinguisher: 1:316
 Paths: 1 available
  Local
    2002::316 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.1.16, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:316:e002::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.136.225.0/24, Route Distinguisher: 1:336
 Paths: 1 available
  Local
    2002::336 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.1.36, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:336:e664::/64, End.DT4
BGP routing table entry for IPv4 prefix 20.138.225.0/24, Route Distinguisher: 1:338
 Paths: 1 available
  Local
    2002::338 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.1.38, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1338:e666::/64, End.DT4
BGP routing table entry for IPv4 prefix 20.142.225.0/24, Route Distinguisher: 1:342
 Paths: 1 available
  Local
    2002::342 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.42, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:342:e002::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.144.225.0/24, Route Distinguisher: 1:344
 Paths: 1 available
  Local
    2002::344 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.44, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1344:e001::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.152.225.0/24, Route Distinguisher: 1:352
 Paths: 1 available
  Local
    2002::352 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.52, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:352:e002::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.153.225.0/24, Route Distinguisher: 1:353
 Paths: 1 available
  Local
    2002::353 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1353:e003::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.161.225.0/24, Route Distinguisher: 1:161
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1:20
      Local SRv6 SID (VRF SID): fcbb:0:161:400::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.162.225.0/24, Route Distinguisher: 1:1162
 Paths: 1 available
  Local
    2002::162 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.162, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1162:400::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.199.225.0/24, Route Distinguisher: 1:199
 Paths: 1 available
  Local
    2002::199 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 20.49.199.199, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1199:e1b7::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.219.225.0/24, Route Distinguisher: 1:419
 Paths: 1 available
  Local
    2002::419 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 0, weight 0, tag 0, valid, internal, best
      Originator: 10.0.1.219, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:419:e0b1::/64, End.DT6 with NEXT-CSID
```

## show bgp vpn-ipv6

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 1011:1 IPv6 prefix 2001:20:11:225::/64
                                 2002::11              -       100     0       ? Or-ID: 10.0.0.11 C-LST: 100.0.0.53 
 * >      RD: 1:20 IPv6 prefix 2001:20:20:225::/64
                                 2002::20              0       100     0       ? Or-ID: 10.0.0.20 C-LST: 100.0.0.53 
 * >      RD: 1:28 IPv6 prefix 2001:20:28:225::/64
                                 2002::28              0       100     0       ? Or-ID: 192.168.20.28 C-LST: 100.0.0.53 
 * >      RD: 1:29 IPv6 prefix 2001:20:29:225::/64
                                 2002::29              0       100     0       ? Or-ID: 192.168.20.29 C-LST: 100.0.0.53 
 * >      RD: 1:36 IPv6 prefix 2001:20:36:225::/64
                                 2002::36              0       100     0       ? Or-ID: 192.168.20.36 C-LST: 100.0.0.53 
   %      RD: 1:49 IPv6 prefix 2001:20:49:225::/64
                                 2002::49              0       100     0       ? Or-ID: 10.0.0.49 C-LST: 100.0.0.53 
 * >      RD: 1:58 IPv6 prefix 2001:20:58:225::/64
                                 2002::58              -       100     0       i Or-ID: 10.0.0.58 C-LST: 100.0.0.53 
 * >      RD: 1:59 IPv6 prefix 2001:20:59:225::/64
                                 2002::59              -       100     0       i Or-ID: 10.0.0.59 C-LST: 100.0.0.53 
 * >      RD: 1:302 IPv6 prefix 2001:20:102:225::/64
                                 2002::302             -       100     0       i Or-ID: 10.0.1.2 C-LST: 100.0.0.53 
 * >      RD: 1:307 IPv6 prefix 2001:20:107:225::/64
                                 2002::307             -       100     0       i Or-ID: 10.0.1.7 C-LST: 100.0.0.53 
 * >      RD: 1:310 IPv6 prefix 2001:20:110:225::/64
                                 2002::310             -       100     0       i Or-ID: 10.0.1.10 C-LST: 100.0.0.53 
 * >      RD: 1:316 IPv6 prefix 2001:20:116:225::/64
                                 2002::316             -       100     0       i Or-ID: 10.0.1.16 C-LST: 100.0.0.53 
 * >      RD: 1:342 IPv6 prefix 2001:20:142:225::/64
                                 2002::342             0       100     0       ? Or-ID: 100.0.0.42 C-LST: 100.0.0.53 
 * >      RD: 1:344 IPv6 prefix 2001:20:144:225::/64
                                 2002::344             0       100     0       ? Or-ID: 100.0.0.44 C-LST: 100.0.0.53 
 * >      RD: 1:352 IPv6 prefix 2001:20:152:225::/64
                                 2002::352             0       100     0       ? Or-ID: 100.0.0.52 C-LST: 100.0.0.53 
 * >      RD: 1:353 IPv6 prefix 2001:20:153:225::/64
                                 2002::353             0       100     0       ?
 * >      RD: 1:161 IPv6 prefix 2001:20:161:225::/64
                                 -                     -       -       0       i
 * >      RD: 1:1162 IPv6 prefix 2001:20:162:225::/64
                                 2002::162             -       100     0       i Or-ID: 100.0.0.162 C-LST: 100.0.0.53 
 * >      RD: 1:199 IPv6 prefix 2001:20:199:225::/64
                                 2002::199             0       100     0       ? Or-ID: 20.49.199.199 C-LST: 100.0.0.53 
   %      RD: 1:419 IPv6 prefix 2001:20:219:225::/64
                                 2002::419             -       0       0       i Or-ID: 10.0.1.219 C-LST: 100.0.0.53 
 * >      RD: 1:336 IPv6 prefix 2001:20:336:225::/64
                                 2002::336             -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
 * >      RD: 1:338 IPv6 prefix 2001:20:338:225::/64
                                 2002::338             -       100     0       ? Or-ID: 10.0.1.38 C-LST: 100.0.0.53 
```

## show bgp vpn-ipv6 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
BGP routing table entry for IPv6 prefix 2001:20:11:225::/64, Route Distinguisher: 1011:1
 Paths: 1 available
  Local
    2002::11 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.0.11, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1011:e002::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:20:225::/64, Route Distinguisher: 1:20
 Paths: 1 available
  Local
    2002::20 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.0.20, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:20:e101::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:28:225::/64, Route Distinguisher: 1:28
 Paths: 1 available
  Local
    2002::28 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 192.168.20.28, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:28:e101::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:29:225::/64, Route Distinguisher: 1:29
 Paths: 1 available
  Local
    2002::29 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 192.168.20.29, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1029:e101::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:36:225::/64, Route Distinguisher: 1:36
 Paths: 1 available
  Local
    2002::36 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 192.168.20.36, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:36:e140::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:49:225::/64, Route Distinguisher: 1:49
 Paths: 1 available
  Local
    2002::49 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, invalid, internal, pending resolution
      Originator: 10.0.0.49, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote MPLS label: 0
BGP routing table entry for IPv6 prefix 2001:20:58:225::/64, Route Distinguisher: 1:58
 Paths: 1 available
  Local
    2002::58 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.0.58, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1058:e018::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:59:225::/64, Route Distinguisher: 1:59
 Paths: 1 available
  Local
    2002::59 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.0.59, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:59:e018::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:102:225::/64, Route Distinguisher: 1:302
 Paths: 1 available
  Local
    2002::302 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.1.2, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1302:e001::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:107:225::/64, Route Distinguisher: 1:307
 Paths: 1 available
  Local
    2002::307 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.1.7, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:307:e001::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:110:225::/64, Route Distinguisher: 1:310
 Paths: 1 available
  Local
    2002::310 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.1.10, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1310:e001::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:116:225::/64, Route Distinguisher: 1:316
 Paths: 1 available
  Local
    2002::316 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.1.16, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:316:e003::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:142:225::/64, Route Distinguisher: 1:342
 Paths: 1 available
  Local
    2002::342 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.42, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:342:e003::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:144:225::/64, Route Distinguisher: 1:344
 Paths: 1 available
  Local
    2002::344 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.44, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1344:e003::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:152:225::/64, Route Distinguisher: 1:352
 Paths: 1 available
  Local
    2002::352 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.52, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:352:e000::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:153:225::/64, Route Distinguisher: 1:353
 Paths: 1 available
  Local
    2002::353 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1353:e004::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:161:225::/64, Route Distinguisher: 1:161
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1:20
      Local SRv6 SID (VRF SID): fcbb:0:161:401::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:162:225::/64, Route Distinguisher: 1:1162
 Paths: 1 available
  Local
    2002::162 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.162, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1162:401::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:199:225::/64, Route Distinguisher: 1:199
 Paths: 1 available
  Local
    2002::199 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 20.49.199.199, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1199:e1b8::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:219:225::/64, Route Distinguisher: 1:419
 Paths: 1 available
  Local
    2002::419 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 0, weight 0, tag 0, invalid, internal, pending resolution
      Originator: 10.0.1.219, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote MPLS label: 0
BGP routing table entry for IPv6 prefix 2001:20:336:225::/64, Route Distinguisher: 1:336
 Paths: 1 available
  Local
    2002::336 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.1.36, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:336:e665::/64, End.DT6
BGP routing table entry for IPv6 prefix 2001:20:338:225::/64, Route Distinguisher: 1:338
 Paths: 1 available
  Local
    2002::338 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.1.38, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1338:e667::/64, End.DT6
```

## show ipv6 route vrf VPNv4-uSID

```text

VRF: VPNv4-uSID
Displaying 20 of 24 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 B I      2001:20:11:225::/64 [200/0]
           via fcbb:0:1011::/48, SRv6 Transport tunnel index 148, SRv6 SID fcbb:0:1011:e002::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:20:225::/64 [200/0]
           via fcbb:0:20::/48, SRv6 Transport tunnel index 118, SRv6 SID fcbb:0:20:e101::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:28:225::/64 [200/0]
           via fcbb:0:28::/48, SRv6 Transport tunnel index 129, SRv6 SID fcbb:0:28:e101::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:29:225::/64 [200/0]
           via fcbb:0:1029::/48, SRv6 Transport tunnel index 138, SRv6 SID fcbb:0:1029:e101::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:36:225::/64 [200/0]
           via fcbb:0:36::/48, SRv6 Transport tunnel index 117, SRv6 SID fcbb:0:36:e140::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:58:225::/64 [200/0]
           via fcbb:0:1058::/48, SRv6 Transport tunnel index 143, SRv6 SID fcbb:0:1058:e018::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:59:225::/64 [200/0]
           via fcbb:0:59::/48, SRv6 Transport tunnel index 106, SRv6 SID fcbb:0:59:e018::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:102:225::/64 [200/0]
           via fcbb:0:1302::/48, SRv6 Transport tunnel index 162, SRv6 SID fcbb:0:1302:e001::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:107:225::/64 [200/0]
           via fcbb:0:307::/48, SRv6 Transport tunnel index 145, SRv6 SID fcbb:0:307:e001::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:110:225::/64 [200/0]
           via fcbb:0:1310::/48, SRv6 Transport tunnel index 144, SRv6 SID fcbb:0:1310:e001::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:116:225::/64 [200/0]
           via fcbb:0:316::/48, SRv6 Transport tunnel index 152, SRv6 SID fcbb:0:316:e003::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:142:225::/64 [200/0]
           via fcbb:0:342::/48, SRv6 Transport tunnel index 112, SRv6 SID fcbb:0:342:e003::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:144:225::/64 [200/0]
           via fcbb:0:1344::/48, SRv6 Transport tunnel index 102, SRv6 SID fcbb:0:1344:e003::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:152:225::/64 [200/0]
           via fcbb:0:352::/48, SRv6 Transport tunnel index 108, SRv6 SID fcbb:0:352:e000::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:153:225::/64 [200/0]
           via fcbb:0:1353::/48, SRv6 Transport tunnel index 116, SRv6 SID fcbb:0:1353:e004::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2001:20:161:225::/64 [0/0]
           via Vlan20, directly connected
 B I      2001:20:162:225::/64 [200/0]
           via fcbb:0:1162::/48, SRv6 Transport tunnel index 163, SRv6 SID fcbb:0:1162:401::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:199:225::/64 [200/0]
           via fcbb:0:1199::/48, SRv6 Transport tunnel index 139, SRv6 SID fcbb:0:1199:e1b8::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:336:225::/64 [200/0]
           via fcbb:0:336::/48, SRv6 Transport tunnel index 105, SRv6 SID fcbb:0:336:e665::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:338:225::/64 [200/0]
           via fcbb:0:1338::/48, SRv6 Transport tunnel index 137, SRv6 SID fcbb:0:1338:e667::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20

```

## show ip route vrf VPNv4-uSID

```text

VRF: VPNv4-uSID
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

 B I      20.11.225.0/24 [200/0]
           via fcbb:0:1011::/48, SRv6 Transport tunnel index 148, SRv6 SID fcbb:0:1011:e001::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.20.225.0/24 [200/0]
           via fcbb:0:20::/48, SRv6 Transport tunnel index 118, SRv6 SID fcbb:0:20:e100::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.28.225.0/24 [200/0]
           via fcbb:0:28::/48, SRv6 Transport tunnel index 129, SRv6 SID fcbb:0:28:e100::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.29.225.0/24 [200/0]
           via fcbb:0:1029::/48, SRv6 Transport tunnel index 138, SRv6 SID fcbb:0:1029:e100::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.36.225.0/24 [200/0]
           via fcbb:0:36::/48, SRv6 Transport tunnel index 117, SRv6 SID fcbb:0:36:e13f::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.58.225.0/24 [200/0]
           via fcbb:0:1058::/48, SRv6 Transport tunnel index 143, SRv6 SID fcbb:0:1058:e017::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.59.225.0/24 [200/0]
           via fcbb:0:59::/48, SRv6 Transport tunnel index 106, SRv6 SID fcbb:0:59:e017::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.102.225.0/24 [200/0]
           via fcbb:0:1302::/48, SRv6 Transport tunnel index 162, SRv6 SID fcbb:0:1302:e000::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.107.225.0/24 [200/0]
           via fcbb:0:307::/48, SRv6 Transport tunnel index 145, SRv6 SID fcbb:0:307:e000::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.110.225.0/24 [200/0]
           via fcbb:0:1310::/48, SRv6 Transport tunnel index 144, SRv6 SID fcbb:0:1310:e000::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.116.225.0/24 [200/0]
           via fcbb:0:316::/48, SRv6 Transport tunnel index 152, SRv6 SID fcbb:0:316:e002::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.136.225.0/24 [200/0]
           via fcbb:0:336::/48, SRv6 Transport tunnel index 105, SRv6 SID fcbb:0:336:e664::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.138.225.0/24 [200/0]
           via fcbb:0:1338::/48, SRv6 Transport tunnel index 137, SRv6 SID fcbb:0:1338:e666::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.142.225.0/24 [200/0]
           via fcbb:0:342::/48, SRv6 Transport tunnel index 112, SRv6 SID fcbb:0:342:e002::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.144.225.0/24 [200/0]
           via fcbb:0:1344::/48, SRv6 Transport tunnel index 102, SRv6 SID fcbb:0:1344:e001::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.152.225.0/24 [200/0]
           via fcbb:0:352::/48, SRv6 Transport tunnel index 108, SRv6 SID fcbb:0:352:e002::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.153.225.0/24 [200/0]
           via fcbb:0:1353::/48, SRv6 Transport tunnel index 116, SRv6 SID fcbb:0:1353:e003::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        20.161.225.0/24 [0/0]
           via Vlan20, directly connected
 B I      20.162.225.0/24 [200/0]
           via fcbb:0:1162::/48, SRv6 Transport tunnel index 163, SRv6 SID fcbb:0:1162:400::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.199.225.0/24 [200/0]
           via fcbb:0:1199::/48, SRv6 Transport tunnel index 139, SRv6 SID fcbb:0:1199:e1b7::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.219.225.0/24 [200/0]
           via fcbb:0:419::/48, SRv6 Transport tunnel index 147, SRv6 SID fcbb:0:419:e0b1::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20

```

## show isis database detail

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: srv6 VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    h3c_20_CR16010E-F.00-00       591   9670   725    571 L2  0000.0000.0020.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: h3c_20_CR16010E-F
      Area addresses: 49.0000
      Interface address: 2001:0:20:36::20
      Interface address: 2001:1:20:36::20
      Interface address: 2002::20
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:20:36::36
        Global IPv6 Interface Address: 2001:0:20:36::20
      IS Neighbor          : ZTE_336_ZXR10_M6000-8SE.00 Metric: 10
        IPv6 Neighbor Address: 2001:1:20:36::36
        Global IPv6 Interface Address: 2001:1:20:36::20
      Reachability          : 2001:0:20:36::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:1:20:36::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::20/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:20::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:20::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:20::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 0
        SRv6 SID End
          SID : fcbb:0:20:e102::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP USP USD
          SID : fcbb:0:20:e103::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
    h3c_28_S12500R-2L.00-00       280  64475  1099    428 L2  0000.0000.0028.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: h3c_28_S12500R-2L
      Area addresses: 49
      Interface address: 2001:0:28:316::28
      Interface address: 2001:0:28:336::28
      Interface address: 2002::28
      IS Neighbor          : JNPR-316-MX304.00   Metric: 10
        IPv6 Neighbor Address: 2001:0:28:316::316
        Global IPv6 Interface Address: 2001:0:28:316::28
      IS Neighbor          : ZTE_336_ZXR10_M6000-8SE.00 Metric: 10
        IPv6 Neighbor Address: 2001:1:28:36::36
        Global IPv6 Interface Address: 2001:0:28:336::28
      Reachability          : 2001:0:28:316::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:28:336::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::28/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:28::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:28::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:28::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 0
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
    huawei_36.00-00             434  20832   606    693 L2  0000.0000.0036.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: huawei_36
      Area addresses: 49.0000
      Topology: 0 (IPv4)
      Interface address: 2001:0:20:36::36
      Interface address: 2002::36
      Interface address: 2001:0:36:58::36
      IS Neighbor          : h3c_20_CR16010E-F.00 Metric: 10
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
      Reachability          : 2001:0:20:36::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::36/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:36::/48 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:36::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:36::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
        SRv6 SID Un Supported
          SID : fcbb:0:36:e103::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 64
        SRv6 SID End
          SID : fcbb:0:36:e104::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP
          SID : fcbb:0:36:e105::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP USP USD
          SID : fcbb:0:36:e106::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
    anet-161-R3.00-00           450  41684   912    250 L2  0000.0000.0161.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 612 s
      NLPID: 0x8E(IPv6)
      Hostname: anet-161-R3
      Area addresses: 49.0000
      Interface address: 2001:0:59:161::161
      Interface address: 2001:0:161:342::161
      Interface address: 2002::161
      IS Neighbor          : Nokia-59-IXRe2.00   Metric: 10
      IS Neighbor          : Cisco342-9902.00    Metric: 10
      Reachability          : fcbb:0:161::/48 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:59:161::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:161:342::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::161/128 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:161::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:161::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      Router Capabilities: Router Id: 100.0.0.161 Flags: []
        Area leader priority: 250 algorithm: 0
        SRv6 Capability: Flags: []
    JNPR-307-ACX7024.00-00       172  22786   914    343 L2  0000.0000.0307.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: JNPR-307-ACX7024
      Area addresses: 49.0000
      Interface address: 10.0.1.7
      IS Neighbor          : Cisco352-N540.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:307:352::352
        Global IPv6 Interface Address: 2001:0:307:352::307
      IS Neighbor          : Cisco353-8201-24H8FH.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:307:353::353
        Global IPv6 Interface Address: 2001:0:307:353::307
      Reachability          : 2001:0:307:352::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:307:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::307/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:307::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:307::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
      Router Capabilities: Router Id: 10.0.1.7 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    JNPR-310-ACX7100-48L.00-00       736  58986  1033   1304 L2  0000.0000.0310.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: JNPR-310-ACX7100-48L
      Area addresses: 49.0001
      Interface address: 10.0.1.10
      IS Neighbor          : Cisco353-8201-24H8FH.00 Metric: 10
        Global IPv6 Interface Address: 2001:0:310:353::353
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::58
        Global IPv6 Interface Address: 2001:0:58:310::310
      Reachability          : 2001:0:58:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:310:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::310/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:162:302::/64 Metric: 30 Type: 1 Up
      Reachability          : 2002::162/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::199/128 Metric: 50 Type: 1 Up
      Reachability          : 2002::302/128 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:1310::/48 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:11:353::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:302:353::/64 Metric: 20 Type: 1 Up
      Reachability          : 2002::353/128 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:1162::/48 Metric: 40 Type: 1 Down
      Reachability          : fcbb:0:1302::/48 Metric: 20 Type: 1 Down
      Reachability          : 2001:0:29:58::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 50 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:1:29:38::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:1:38:49::/64 Metric: 40 Type: 1 Up
      Reachability          : 2002::29/128 Metric: 20 Type: 1 Up
      Reachability          : 2002::49/128 Metric: 50 Type: 1 Up
      Reachability          : 2002::58/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::338/128 Metric: 40 Type: 1 Up
      Reachability          : 2002:0:29:338::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:162:344::/64 Metric: 1030 Type: 1 Up
      Reachability          : 2001:0:199:344::/64 Metric: 60 Type: 1 Up
      Reachability          : 2002::344/128 Metric: 70 Type: 1 Up
      Reachability          : 2002::419/128 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::11/128 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:1310::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1162::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1162::
      SRv6 Locator: fcbb:0:1302::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:0:1302::
      SRv6 Locator: fcbb:0:1029::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1029::
      SRv6 Locator: fcbb:0:1049::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1049::
      SRv6 Locator: fcbb:0:1338::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:0:1338::
      SRv6 Locator: fcbb:0:1199::/48 Topology: 0
        Metric: 50 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1199::
        SRv6 SID Un Supported
          SID : fcbb:0:1199:e17b::
        SRv6 SID End
          SID : fcbb:0:1199:e17d::
        SRv6 SID End with PSP
          SID : fcbb:0:1199:e17e::
        SRv6 SID End with PSP USP USD
          SID : fcbb:0:1199:e17f::
      SRv6 Locator: fcbb:0:1344::/48 Topology: 0
        Metric: 61 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1344::
      SRv6 Locator: fcbb:0:419::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:419:11::
      SRv6 Locator: fcbb:0:1011::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1011::
      Router Capabilities: Router Id: 10.0.1.10 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    JNPR-310-ACX7100-48L.00-01       427   4653  1033    200 L2  0000.0000.0310.00-01  <>
      Reachability          : fcbb:0:1029::/48 Metric: 20 Type: 1 Down
      Reachability          : fcbb:0:1049::/48 Metric: 40 Type: 1 Down
      Reachability          : fcbb:0:1058::/48 Metric: 10 Type: 1 Down
      Reachability          : fcbb:0:1338::/48 Metric: 30 Type: 1 Down
      Reachability          : fcbb:0:1199::/48 Metric: 50 Type: 1 Down
      Reachability          : fcbb:0:1344::/48 Metric: 61 Type: 1 Down
      Reachability          : fcbb:0:419::/48 Metric: 20 Type: 1 Down
      Reachability          : fcbb:0:1011::/48 Metric: 10 Type: 1 Down
      SRv6 Locator: fcbb:0:1058::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1058::
    JNPR-316-MX304.00-00        260  11933   784    369 L2  0000.0000.0316.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: JNPR-316-MX304
      Area addresses: 49.0000
      Interface address: 10.0.1.16
      IS Neighbor          : h3c_28_S12500R-2L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:28:316::28
        Global IPv6 Interface Address: 2001:0:28:316::316
      IS Neighbor          : Cisco342-9902.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:316:342::342
        Global IPv6 Interface Address: 2001:0:316:342::316
      Reachability          : 2001:0:28:316::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:316:342::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::316/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:316::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:316::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:0:316::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.1.16 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    ZTE_336_ZXR10_M6000-8SE.00-00       476  53237   977    474 L2  0000.0000.0336.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: ZTE_336_ZXR10_M6000-8SE
      Area addresses: 49.0000
      Interface address: 10.0.1.36
      Interface address: 2002::336
      IS Neighbor          : h3c_20_CR16010E-F.00 Metric: 10
        IPv6 Neighbor Address: 2001:1:20:36::20
        Global IPv6 Interface Address: 2001:1:20:36::36
      IS Neighbor          : h3c_28_S12500R-2L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:28:336::28
        Global IPv6 Interface Address: 2001:1:28:36::36
      Reachability         : 10.0.1.36/32 Metric: 10 Type: 1 Up
      Reachability          : 2001:1:20:36::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:1:28:36::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::336/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:336::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:336::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:0:336::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.1.36 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 4096
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  20
        SRv6 Capability: Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 900000 Range: 65536
        Algorithms:  0, 1
    Cisco342-9902.00-00         257   4496  1174    417 L2  0000.0000.0342.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: Cisco342-9902
      Area addresses: 49.0001
      Interface address: 2002::342
      IS Neighbor          : anet-161-R3.00      Metric: 10
        Global IPv6 Interface Address: 2001:0:161:342::342
      IS Neighbor          : JNPR-316-MX304.00   Metric: 10
        IPv6 Neighbor Address: 2001:0:316:342::316
        Global IPv6 Interface Address: 2001:0:316:342::342
      Reachability          : 2001:0:161:342::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:316:342::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::342/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:342::/48 Metric: 1 Type: 1 Up
      SRv6 Locator: fcbb:0:342::/48 Topology: 0
        Metric: 1 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:342::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Cisco352-N540.00-00         420  33918  1190    435 L2  0000.0000.0352.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: Cisco352-N540
      Area addresses: 49.0001
      Interface address: 2002::352
      IS Neighbor          : JNPR-307-ACX7024.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:307:352::307
        Global IPv6 Interface Address: 2001:0:307:352::352
      IS Neighbor          : Nokia-59-IXRe2.00   Metric: 10
        IPv6 Neighbor Address: 2001:1:59:352::59
        Global IPv6 Interface Address: 2001:0:59:352::352
      Reachability          : 2001:0:59:352::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:307:352::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::352/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:352::/48 Metric: 1 Type: 1 Up
      SRv6 Locator: fcbb:0:352::/48 Topology: 0
        Metric: 1 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:352::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Cisco353-8201-24H8FH.00-00       697  12837   863   1315 L2  0000.0000.0353.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: Cisco353-8201-24H8FH
      Area addresses:
        49.0000
        49.0001
      Interface address: 2002::353
      IS Neighbor          : JNPR-307-ACX7024.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:307:353::307
        Global IPv6 Interface Address: 2001:0:307:353::353
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
      Reachability          : 2001:0:302:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:307:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::29/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::49/128 Metric: 60 Type: 1 Up
      Reachability          : 2002::162/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::199/128 Metric: 60 Type: 1 Up
      Reachability          : 2002::302/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::344/128 Metric: 80 Type: 1 Up
      Reachability          : 2002::353/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1029::/48 Metric: 30 Type: 1 Up
      Reachability          : fcbb:0:1353::/48 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:29:58::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 60 Type: 1 Up
      Reachability          : 2001:0:162:302::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:162:344::/64 Metric: 1020 Type: 1 Up
      Reachability          : 2001:0:199:344::/64 Metric: 70 Type: 1 Up
      Reachability          : 2002::338/128 Metric: 50 Type: 1 Up
      Reachability          : 2002:0:29:338::/64 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1011::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:1049::/48 Metric: 50 Type: 1 Up
      Reachability          : fcbb:0:1162::/48 Metric: 30 Type: 1 Up
      Reachability          : fcbb:0:1199::/48 Metric: 60 Type: 1 Up
      Reachability          : fcbb:0:1310::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1344::/48 Metric: 71 Type: 1 Up
      Reachability          : 2001:0:11:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:310:353::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:1:29:38::/64 Metric: 50 Type: 1 Up
      Reachability          : 2001:1:38:49::/64 Metric: 50 Type: 1 Up
      Reachability          : 2002::11/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::58/128 Metric: 20 Type: 1 Up
      Reachability          : 2002::310/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:419::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1058::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:1338::/48 Metric: 40 Type: 1 Up
      Reachability          : 2002::419/128 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1302::/48 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:419::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1011::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1029::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1049::/48 Topology: 0
        Metric: 50 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1058::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1162::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1199::/48 Topology: 0
        Metric: 60 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1302::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1310::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1338::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1344::/48 Topology: 0
        Metric: 71 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1353::/48 Topology: 0
        Metric: 1 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1353::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Nokia_58-SR1-3-SRv6.00-00       457  37084 61749    743 L2  0100.0000.0058.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia_58-SR1-3-SRv6
      Area addresses:
        49.0000
        49.0001
      Reachability          : 2001:0:49:199::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:0:162:302::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:0:162:344::/64 Metric: 1040 Type: 1 Up
      Reachability          : 2001:0:199:344::/64 Metric: 50 Type: 1 Up
      Reachability          : 2001:0:302:353::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:310:353::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:1:29:38::/64 Metric: 30 Type: 1 Up
      Reachability          : fcbb:0:1049::/48 Metric: 30 Type: 1 Up
      Reachability          : fcbb:0:1162::/48 Metric: 50 Type: 1 Up
      Reachability          : fcbb:0:1199::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1302::/48 Metric: 30 Type: 1 Up
      Reachability          : fcbb:0:1310::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1338::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:1344::/48 Metric: 51 Type: 1 Up
      Reachability          : fcbb:0:1353::/48 Metric: 21 Type: 1 Up
      SRv6 Locator: fcbb:0:1049::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1049::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:0:1162::/48 Topology: 0
        Metric: 50 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1162::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:0:1199::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1199::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
        SRv6 SID Un Supported
          SID : fcbb:0:1199:e17b::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 64
        SRv6 SID End
          SID : fcbb:0:1199:e17d::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP
          SID : fcbb:0:1199:e17e::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP USP USD
          SID : fcbb:0:1199:e17f::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:0:1302::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:0:1302::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:0:1310::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1338::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:0:1338::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:0:1344::/48 Topology: 0
        Metric: 51 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1344::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:0:1353::/48 Topology: 0
        Metric: 21 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1353::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.0.58 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0
    Nokia_58-SR1-3-SRv6.00-01       335  17926 64517   1259 L2  0100.0000.0058.00-01  <>
      Interface address: 10.0.0.58
      Interface address: 2001:0:36:58::58
      Interface address: 2001:0:58:310::58
      Interface address: 2001:0:58:419::58
      Interface address: 2002::58
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:36:58::36
        Global IPv6 Interface Address: 2001:0:36:58::58
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::310
        Global IPv6 Interface Address: 2001:0:58:310::58
      IS Neighbor          : Keys-Ixia-419.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:58:419::419
        Global IPv6 Interface Address: 2001:0:58:419::58
      Reachability         : 10.0.0.58/32 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:11:353::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:29:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:1:38:49::/64 Metric: 30 Type: 1 Up
      Reachability          : 2002::11/128 Metric: 20 Type: 1 Up
      Reachability          : 2002::29/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::49/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::58/128 Metric: 0 Type: 1 Up
      Reachability          : 2002::162/128 Metric: 50 Type: 1 Up
      Reachability          : 2002::199/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::302/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::310/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::338/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::344/128 Metric: 60 Type: 1 Up
      Reachability          : 2002::353/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::419/128 Metric: 20 Type: 1 Up
      Reachability          : 2002:0:29:338::/64 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:419::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1011::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:1029::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1058::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:419::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:419:11::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:0:1011::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1011::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:0:1029::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1029::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 0
      SRv6 Locator: fcbb:0:1058::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1058::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:1:1058::/48 Topology: 0
        Metric: 0 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:1058::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
    Nokia-59-IXRe2.00-00        233  30716   664    488 L2  0100.0000.0059.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-59-IXRe2
      Area addresses: 49.0000.0000.0059.00
      Interface address: 10.0.0.59
      Interface address: 2001:0:59:161::59
      Interface address: 2001:1:59:352::59
      Interface address: 2002::59
      IS Neighbor          : Cisco352-N540.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:59:352::352
        Global IPv6 Interface Address: 2001:1:59:352::59
      IS Neighbor          : anet-161-R3.00      Metric: 10
        Global IPv6 Interface Address: 2001:0:59:161::59
      Reachability         : 10.0.0.59/32 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:59:161::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:1:59:352::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::59/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:59::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:59::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:59::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.0.59 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0
    Keys-Ixia-419.00-00         158  46061   785    351 L2  3800.0000.0419.00-00  <DefaultAtt>
      NLPID: 0xCC(IPv4) 0x8E(IPv6) 0x81(CLNP)
      Hostname: Keys-Ixia-419
      Area addresses: 49.0001
      Interface address: 2001:0:58:419::419
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:419::58
        Global IPv6 Interface Address: 2001:0:58:419::419
      Reachability          : 2002::419/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:419::/48 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:419::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:419:11::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.1.119 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0
```

