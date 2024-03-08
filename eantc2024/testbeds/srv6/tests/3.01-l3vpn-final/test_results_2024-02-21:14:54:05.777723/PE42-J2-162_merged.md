# Test results for PE42-J2-162

## show interfaces status

```text
Port       Name   Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1               notconnect   1        full   25G    Not Present                    
Et2               notconnect   1        full   25G    Not Present                    
Et3               notconnect   1        full   25G    Not Present                    
Et4               notconnect   1        full   25G    Not Present                    
Et5               notconnect   1        full   10G    10GBASE-SRL                    
Et6               notconnect   1        full   25G    Not Present                    
Et7               notconnect   1        full   25G    Not Present                    
Et8               notconnect   1        full   25G    Not Present                    
Et9               notconnect   1        full   25G    Not Present                    
Et10              connected    routed   full   10G    10GBASE-SRL                    
Et11              notconnect   1        full   25G    Not Present                    
Et12              connected    trunk    full   10G    10GBASE-LR                     
Et13              notconnect   1        full   25G    Not Present                    
Et14              notconnect   1        full   25G    Not Present                    
Et15              notconnect   1        full   25G    Not Present                    
Et16              notconnect   1        full   25G    Not Present                    
Et17              notconnect   1        full   25G    Not Present                    
Et18              notconnect   1        full   25G    Not Present                    
Et19              notconnect   1        full   25G    Not Present                    
Et20              connected    routed   full   10G    10GBASE-SR                     
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
Last table change time   : 0:03:46 ago
Number of table inserts  : 14
Number of table deletes  : 8
Number of table drops    : 0
Number of table age-outs : 0

Port          Neighbor Device ID            Neighbor Port ID    TTL
---------- ----------------------------- ---------------------- ---
Et10          JNPR-302-MX204                564                 120
Et12          JNPR-398-QFX5120              548                 120
Et20          Cisco344-N57B1                TenGigE0/0/0/0/0    120
Et39          PE41-J2-161.ns.eantc.de       Ethernet39          120
Et40          PE41-J2-161.ns.eantc.de       Ethernet40          120
Ma1           extreme-x460-1                22                  120

```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
srv6      default  JNPR-302-MX204   L1   Ethernet10         P2P               UP    19          01                  
srv6      default  Cisco344-N57B1   L1   Ethernet20         P2P               UP    21          00                  
```

## show tunnel fib

```text

Type 'SRv6 Transport', index 15, endpoint fcbb:0:1344::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 48, endpoint fcbb:0:1338::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 55, endpoint fcbb:0:1199::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 131, endpoint fcbb:0:1353::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 165, endpoint fcbb:0:352::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 169, endpoint fcbb:0:336::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 170, endpoint fcbb:0:59::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 171, endpoint fcbb:0:342::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 172, endpoint fcbb:0:161::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 175, endpoint fcbb:0:36::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 176, endpoint fcbb:0:20::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 189, endpoint fcbb:0:1029::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 190, endpoint fcbb:0:28::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 199, endpoint fcbb:0:1058::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 200, endpoint fcbb:0:1310::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 201, endpoint fcbb:0:307::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 203, endpoint fcbb:0:419::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 204, endpoint fcbb:0:1011::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 207, endpoint fcbb:0:316::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 212, endpoint fcbb:0:1302::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162
```

## show bgp vpn-ipv4

```text
BGP routing table information for VRF default
Router identifier 100.0.0.162, local AS number 1
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
                                 2002::161             -       100     0       i Or-ID: 100.0.0.161 C-LST: 100.0.0.53 
 * >      RD: 1:1162 IPv4 prefix 20.162.225.0/24
                                 -                     -       -       0       i
 * >      RD: 1:199 IPv4 prefix 20.199.225.0/24
                                 2002::199             0       100     0       ? Or-ID: 20.49.199.199 C-LST: 100.0.0.53 
 * >      RD: 1:419 IPv4 prefix 20.219.225.0/24
                                 2002::419             -       0       0       i Or-ID: 10.0.1.219 C-LST: 100.0.0.53 
```

## show bgp vpn-ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.162, local AS number 1
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
    2002::161 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.161, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:161:400::/64, End.DT4 with NEXT-CSID
BGP routing table entry for IPv4 prefix 20.162.225.0/24, Route Distinguisher: 1:1162
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1:20
      Local SRv6 SID (VRF SID): fcbb:0:1162:400::/64, End.DT4 with NEXT-CSID
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
Router identifier 100.0.0.162, local AS number 1
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
                                 2002::161             -       100     0       i Or-ID: 100.0.0.161 C-LST: 100.0.0.53 
 * >      RD: 1:1162 IPv6 prefix 2001:20:162:225::/64
                                 -                     -       -       0       i
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
Router identifier 100.0.0.162, local AS number 1
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
    2002::161 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.161, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:161:401::/64, End.DT6 with NEXT-CSID
BGP routing table entry for IPv6 prefix 2001:20:162:225::/64, Route Distinguisher: 1:1162
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1:20
      Local SRv6 SID (VRF SID): fcbb:0:1162:401::/64, End.DT6 with NEXT-CSID
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
Codes: C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 B I      2001:20:11:225::/64 [200/0]
           via fcbb:0:1011::/48, SRv6 Transport tunnel index 204, SRv6 SID fcbb:0:1011:e002::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:20:225::/64 [200/0]
           via fcbb:0:20::/48, SRv6 Transport tunnel index 176, SRv6 SID fcbb:0:20:e101::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:28:225::/64 [200/0]
           via fcbb:0:28::/48, SRv6 Transport tunnel index 190, SRv6 SID fcbb:0:28:e101::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:29:225::/64 [200/0]
           via fcbb:0:1029::/48, SRv6 Transport tunnel index 189, SRv6 SID fcbb:0:1029:e101::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:36:225::/64 [200/0]
           via fcbb:0:36::/48, SRv6 Transport tunnel index 175, SRv6 SID fcbb:0:36:e140::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:58:225::/64 [200/0]
           via fcbb:0:1058::/48, SRv6 Transport tunnel index 199, SRv6 SID fcbb:0:1058:e018::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:59:225::/64 [200/0]
           via fcbb:0:59::/48, SRv6 Transport tunnel index 170, SRv6 SID fcbb:0:59:e018::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:102:225::/64 [200/0]
           via fcbb:0:1302::/48, SRv6 Transport tunnel index 212, SRv6 SID fcbb:0:1302:e001::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:107:225::/64 [200/0]
           via fcbb:0:307::/48, SRv6 Transport tunnel index 201, SRv6 SID fcbb:0:307:e001::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:110:225::/64 [200/0]
           via fcbb:0:1310::/48, SRv6 Transport tunnel index 200, SRv6 SID fcbb:0:1310:e001::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:116:225::/64 [200/0]
           via fcbb:0:316::/48, SRv6 Transport tunnel index 207, SRv6 SID fcbb:0:316:e003::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:142:225::/64 [200/0]
           via fcbb:0:342::/48, SRv6 Transport tunnel index 171, SRv6 SID fcbb:0:342:e003::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:144:225::/64 [200/0]
           via fcbb:0:1344::/48, SRv6 Transport tunnel index 15, SRv6 SID fcbb:0:1344:e003::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:152:225::/64 [200/0]
           via fcbb:0:352::/48, SRv6 Transport tunnel index 165, SRv6 SID fcbb:0:352:e000::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:153:225::/64 [200/0]
           via fcbb:0:1353::/48, SRv6 Transport tunnel index 131, SRv6 SID fcbb:0:1353:e004::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:161:225::/64 [200/0]
           via fcbb:0:161::/48, SRv6 Transport tunnel index 172, SRv6 SID fcbb:0:161:401::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 C        2001:20:162:225::/64 [0/0]
           via Vlan20, directly connected
 B I      2001:20:199:225::/64 [200/0]
           via fcbb:0:1199::/48, SRv6 Transport tunnel index 55, SRv6 SID fcbb:0:1199:e1b8::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:336:225::/64 [200/0]
           via fcbb:0:336::/48, SRv6 Transport tunnel index 169, SRv6 SID fcbb:0:336:e665::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:338:225::/64 [200/0]
           via fcbb:0:1338::/48, SRv6 Transport tunnel index 48, SRv6 SID fcbb:0:1338:e667::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10

```

## show ip route vrf VPNv4-uSID

```text

VRF: VPNv4-uSID
Codes: C - connected, S - static, K - kernel, 
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
           via fcbb:0:1011::/48, SRv6 Transport tunnel index 204, SRv6 SID fcbb:0:1011:e001::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.20.225.0/24 [200/0]
           via fcbb:0:20::/48, SRv6 Transport tunnel index 176, SRv6 SID fcbb:0:20:e100::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.28.225.0/24 [200/0]
           via fcbb:0:28::/48, SRv6 Transport tunnel index 190, SRv6 SID fcbb:0:28:e100::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.29.225.0/24 [200/0]
           via fcbb:0:1029::/48, SRv6 Transport tunnel index 189, SRv6 SID fcbb:0:1029:e100::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.36.225.0/24 [200/0]
           via fcbb:0:36::/48, SRv6 Transport tunnel index 175, SRv6 SID fcbb:0:36:e13f::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.58.225.0/24 [200/0]
           via fcbb:0:1058::/48, SRv6 Transport tunnel index 199, SRv6 SID fcbb:0:1058:e017::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.59.225.0/24 [200/0]
           via fcbb:0:59::/48, SRv6 Transport tunnel index 170, SRv6 SID fcbb:0:59:e017::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.102.225.0/24 [200/0]
           via fcbb:0:1302::/48, SRv6 Transport tunnel index 212, SRv6 SID fcbb:0:1302:e000::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.107.225.0/24 [200/0]
           via fcbb:0:307::/48, SRv6 Transport tunnel index 201, SRv6 SID fcbb:0:307:e000::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.110.225.0/24 [200/0]
           via fcbb:0:1310::/48, SRv6 Transport tunnel index 200, SRv6 SID fcbb:0:1310:e000::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.116.225.0/24 [200/0]
           via fcbb:0:316::/48, SRv6 Transport tunnel index 207, SRv6 SID fcbb:0:316:e002::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.136.225.0/24 [200/0]
           via fcbb:0:336::/48, SRv6 Transport tunnel index 169, SRv6 SID fcbb:0:336:e664::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.138.225.0/24 [200/0]
           via fcbb:0:1338::/48, SRv6 Transport tunnel index 48, SRv6 SID fcbb:0:1338:e666::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.142.225.0/24 [200/0]
           via fcbb:0:342::/48, SRv6 Transport tunnel index 171, SRv6 SID fcbb:0:342:e002::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.144.225.0/24 [200/0]
           via fcbb:0:1344::/48, SRv6 Transport tunnel index 15, SRv6 SID fcbb:0:1344:e001::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.152.225.0/24 [200/0]
           via fcbb:0:352::/48, SRv6 Transport tunnel index 165, SRv6 SID fcbb:0:352:e002::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.153.225.0/24 [200/0]
           via fcbb:0:1353::/48, SRv6 Transport tunnel index 131, SRv6 SID fcbb:0:1353:e003::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.161.225.0/24 [200/0]
           via fcbb:0:161::/48, SRv6 Transport tunnel index 172, SRv6 SID fcbb:0:161:400::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 C        20.162.225.0/24 [0/0]
           via Vlan20, directly connected
 B I      20.199.225.0/24 [200/0]
           via fcbb:0:1199::/48, SRv6 Transport tunnel index 55, SRv6 SID fcbb:0:1199:e1b7::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.219.225.0/24 [200/0]
           via fcbb:0:419::/48, SRv6 Transport tunnel index 203, SRv6 SID fcbb:0:419:e0b1::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10

```

## show isis database detail

```text

IS-IS Instance: srv6 VRF: default
  IS-IS Level 1 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS Flags
    CIEN-11-5169.00-00          608  11757  1084    529 L1 <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0x8E(IPv6)
      Hostname: CIEN-11-5169
      Area addresses: 49.0001
      Interface address: 2001:0:11:353::11
      IS Neighbor          : Cisco353-8201-24H8FH.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:11:353::353
        Global IPv6 Interface Address: 2001:0:11:353::11
        Adj-sid: 24001 flags: [L V F] weight: 0x0
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:11:310::310
        Global IPv6 Interface Address: 2001:0:11:310::11
        Adj-sid: 24000 flags: [L V F] weight: 0x0
      Reachability         : 10.0.0.11/32 Metric: 0 Type: 1 Up
      Reachability          : 2002::11/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:11:353::/64 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1011::/48 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:1011::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1011::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      Router Capabilities: Router Id: 10.0.0.11 Flags: []
        SRv6 Capability: Flags: []
        SR Capability: Flags: [V]
          SRGB Base: 16000 Range: 8000
        Algorithms:  0
    h3c_29_S12500R-2L.00-00       270  55827   572    430 L1 <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: h3c_29_S12500R-2L
      Area addresses: 49.0001
      Interface address: 2001:0:29:58::29
      Interface address: 2002::29
      Interface address: 2002:0:29:338::29
      IS Neighbor          : ZTE_338_ZXR10_M6000-4SE.00 Metric: 10
        IPv6 Neighbor Address: 2001:1:29:38::38
        Global IPv6 Interface Address: 2002:0:29:338::29
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:29:58::58
        Global IPv6 Interface Address: 2001:0:29:58::29
      Reachability          : 2001:0:29:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::29/128 Metric: 0 Type: 1 Up
      Reachability          : 2002:0:29:338::/64 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1029::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:1029::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1029::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 0
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
    Ericsson_6676_49.00-00       289  60398  1091    486 L1 <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Ericsson_6676_49
      Area addresses: 49.0001
      Interface address: 10.0.0.49
      Interface address: 2002::49
      IS Neighbor          : ZTE_338_ZXR10_M6000-4SE.00 Metric: 10
        IPv4 Interface Address: 21.38.49.49
        IPv6 Neighbor Address: 2001:1:38:49::38
        Global IPv6 Interface Address: 2001:1:38:49::49
      IS Neighbor          : huawei_199.00       Metric: 10
        IPv4 Interface Address: 20.49.199.49
        IPv6 Neighbor Address: 2001:0:49:199::199
        Global IPv6 Interface Address: 2001:0:49:199::49
      Reachability         : 10.0.0.49/32 Metric: 10 Type: 1 Up
      Reachability         : 21.38.49.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.49.199.0/24 Metric: 10 Type: 1 Up
      Reachability          : 2002::49/128 Metric: 10 Type: 1 Up
      Reachability          : 2001:1:38:49::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1049::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:1049::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1049::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.0.49 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0
    anet-162-R3.00-00           231   7469   920    250 L1 <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 620 s
      NLPID: 0x8E(IPv6)
      Hostname: anet-162-R3
      Area addresses: 49.0001
      Interface address: 2001:0:162:302::162
      Interface address: 2001:0:162:344::162
      Interface address: 2002::162
      IS Neighbor          : JNPR-302-MX204.00   Metric: 10
      IS Neighbor          : Cisco344-N57B1.00   Metric: 1000
      Reachability          : fcbb:0:1162::/48 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:162:302::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:162:344::/64 Metric: 1000 Type: 1 Up
      Reachability          : 2002::162/128 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:1162::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1162::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      Router Capabilities: Router Id: 100.0.0.162 Flags: []
        Area leader priority: 250 algorithm: 0
        SRv6 Capability: Flags: []
    huawei_199.00-00            275  57755   707    694 L1 <>
      NLPID: 0x8E(IPv6)
      Hostname: huawei_199
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Interface address: 2002::199
      Interface address: 2001:0:49:199::199
      Interface address: 2001:0:199:344::199
      IS Neighbor          : Ericsson_6676_49.00 Metric: 10
      IS Neighbor          : Cisco344-N57B1.00   Metric: 10
      Reachability          : 2001:0:49:199::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::199/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:1199::/48 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:199:344::/64 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:1199::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
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
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
    JNPR-302-MX204.00-00        238  56427   951    351 L1 <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0x8E(IPv6)
      Hostname: JNPR-302-MX204
      Area addresses: 49.0001
      Interface address: 10.0.1.2
      IS Neighbor          : anet-162-R3.00      Metric: 10
        Global IPv6 Interface Address: 2001:0:162:302::302
      IS Neighbor          : Cisco353-8201-24H8FH.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:302:353::353
        Global IPv6 Interface Address: 2001:0:302:353::302
      Reachability          : 2002::302/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:162:302::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:302:353::/64 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1302::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:1302::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:0:1302::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.1.2 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    JNPR-310-ACX7100-48L.00-00       791  23222  1032   1248 L2 <DefaultAtt>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0x8E(IPv6)
      Hostname: JNPR-310-ACX7100-48L
      Area addresses: 49.0001
      Interface address: 10.0.1.10
      Reachability          : 2001:0:58:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:310:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::310/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:20:36::/64 Metric: 30 Type: 1 Down
      Reachability          : 2001:0:28:316::/64 Metric: 60 Type: 1 Down
      Reachability          : 2001:0:28:336::/64 Metric: 60 Type: 1 Down
      Reachability          : 2001:1:20:36::/64 Metric: 40 Type: 1 Down
      Reachability          : 2001:1:28:36::/64 Metric: 50 Type: 1 Down
      Reachability          : 2002::20/128 Metric: 30 Type: 1 Down
      Reachability          : 2002::28/128 Metric: 50 Type: 1 Down
      Reachability          : 2002::36/128 Metric: 20 Type: 1 Down
      Reachability          : 2002::336/128 Metric: 50 Type: 1 Down
      Reachability          : 2001:0:59:161::/64 Metric: 50 Type: 1 Down
      Reachability          : 2001:0:59:352::/64 Metric: 40 Type: 1 Down
      Reachability          : 2001:0:161:342::/64 Metric: 60 Type: 1 Down
      Reachability          : 2001:0:307:352::/64 Metric: 30 Type: 1 Down
      Reachability          : 2001:0:307:353::/64 Metric: 20 Type: 1 Down
      Reachability          : 2001:0:316:342::/64 Metric: 70 Type: 1 Down
      Reachability          : 2001:1:59:352::/64 Metric: 50 Type: 1 Down
      Reachability          : 2002::59/128 Metric: 40 Type: 1 Down
      Reachability          : 2002::161/128 Metric: 60 Type: 1 Down
      Reachability          : 2002::307/128 Metric: 20 Type: 1 Down
      Reachability          : 2002::342/128 Metric: 70 Type: 1 Down
      Reachability          : 2002::352/128 Metric: 40 Type: 1 Down
      Reachability          : fcbb:0:1310::/48 Metric: 0 Type: 1 Up
      Reachability          : 2002::316/128 Metric: 60 Type: 1 Down
      Reachability          : 2001:0:11:310::/64 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:1310::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:20::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: [D]
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:20::
        SRv6 SID End
          SID : fcbb:0:20:e102::
        SRv6 SID End with PSP USP USD
          SID : fcbb:0:20:e103::
      SRv6 Locator: fcbb:0:28::/48 Topology: 0
        Metric: 50 Algorithm: 0 Flags: [D]
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:28::
      SRv6 Locator: fcbb:0:36::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: [D]
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:36::
        SRv6 SID Un Supported
          SID : fcbb:0:36:e103::
        SRv6 SID End
          SID : fcbb:0:36:e104::
        SRv6 SID End with PSP
          SID : fcbb:0:36:e105::
        SRv6 SID End with PSP USP USD
          SID : fcbb:0:36:e106::
      SRv6 Locator: fcbb:0:59::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: [D]
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:59::
      SRv6 Locator: fcbb:0:161::/48 Topology: 0
        Metric: 60 Algorithm: 0 Flags: [D]
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:161::
      SRv6 Locator: fcbb:0:307::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: [D]
      SRv6 Locator: fcbb:0:336::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: [D]
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:0:336::
      SRv6 Locator: fcbb:0:342::/48 Topology: 0
        Metric: 61 Algorithm: 0 Flags: [D]
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:342::
      SRv6 Locator: fcbb:0:352::/48 Topology: 0
        Metric: 31 Algorithm: 0 Flags: [D]
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:352::
      SRv6 Locator: fcbb:0:1353::/48 Topology: 0
        Metric: 11 Algorithm: 0 Flags: [D]
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1353::
      SRv6 Locator: fcbb:0:316::/48 Topology: 0
        Metric: 60 Algorithm: 0 Flags: [D]
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:0:316::
      Router Capabilities: Router Id: 10.0.1.10 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    JNPR-310-ACX7100-48L.00-01       521  36306  1033    372 L2 <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      IS Neighbor          : Cisco353-8201-24H8FH.00 Metric: 10
        Global IPv6 Interface Address: 2001:0:310:353::353
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::58
        Global IPv6 Interface Address: 2001:0:58:310::310
      IS Neighbor          : CIEN-11-5169.00     Metric: 10
        IPv6 Neighbor Address: 2001:0:11:310::11
        Global IPv6 Interface Address: 2001:0:11:310::310
      Reachability          : fcbb:0:20::/48 Metric: 30 Type: 1 Down
      Reachability          : fcbb:0:28::/48 Metric: 50 Type: 1 Down
      Reachability          : fcbb:0:36::/48 Metric: 20 Type: 1 Down
      Reachability          : fcbb:0:59::/48 Metric: 40 Type: 1 Down
      Reachability          : fcbb:0:161::/48 Metric: 60 Type: 1 Down
      Reachability          : fcbb:0:307::/48 Metric: 20 Type: 1 Down
      Reachability          : fcbb:0:336::/48 Metric: 40 Type: 1 Down
      Reachability          : fcbb:0:342::/48 Metric: 61 Type: 1 Down
      Reachability          : fcbb:0:352::/48 Metric: 31 Type: 1 Down
      Reachability          : fcbb:0:1353::/48 Metric: 11 Type: 1 Down
      Reachability          : fcbb:0:316::/48 Metric: 60 Type: 1 Down
    ZTE_338_ZXR10_M6000-4SE.00-00       330   3549   476    501 L2 <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: ZTE_338_ZXR10_M6000-4SE
      Area addresses: 49.0001
      Interface address: 10.0.1.38
      Interface address: 2002::338
      IS Neighbor          : h3c_29_S12500R-2L.00 Metric: 10
        IPv6 Neighbor Address: 2002:0:29:338::29
        Global IPv6 Interface Address: 2001:1:29:38::38
      IS Neighbor          : Ericsson_6676_49.00 Metric: 10
        IPv4 Neighbor Address: 21.38.49.49
        IPv4 Interface Address: 21.38.49.38
        IPv6 Neighbor Address: 2001:1:38:49::49
        Global IPv6 Interface Address: 2001:1:38:49::38
        Adj-sid: 965536 flags: [L V] weight: 0x0
      Reachability         : 10.0.1.38/32 Metric: 10 Type: 1 Up
      Reachability         : 21.38.49.0/24 Metric: 10 Type: 1 Up
      Reachability          : 2001:1:29:38::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:1:38:49::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::338/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1338::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:1338::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:0:1338::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.1.38 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 4096
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  20
        SRv6 Capability: Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 900000 Range: 65536
        Algorithms:  0, 1
    Cisco344-N57B1.00-00        226   1873   969    418 L1 <>
      NLPID: 0x8E(IPv6)
      Hostname: Cisco344-N57B1
      Area addresses: 49.0001
      Interface address: 2002::344
      IS Neighbor          : anet-162-R3.00      Metric: 1000
        Global IPv6 Interface Address: 2001:0:162:344::344
      IS Neighbor          : huawei_199.00       Metric: 10
        IPv6 Neighbor Address: 2001:0:199:344::199
        Global IPv6 Interface Address: 2001:0:199:344::344
      Reachability          : 2001:0:162:344::/64 Metric: 1000 Type: 1 Up
      Reachability          : 2001:0:199:344::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::344/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1344::/48 Metric: 1 Type: 1 Up
      SRv6 Locator: fcbb:0:1344::/48 Topology: 0
        Metric: 1 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1344::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Cisco353-8201-24H8FH.00-00       861  12431   953   1323 L2 <DefaultAtt>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0x8E(IPv6)
      Hostname: Cisco353-8201-24H8FH
      Area addresses: 49.0001
      Interface address: 2002::353
      IS Neighbor          : CIEN-11-5169.00     Metric: 10
        IPv6 Neighbor Address: 2001:0:11:353::11
        Global IPv6 Interface Address: 2001:0:11:353::353
      IS Neighbor          : JNPR-302-MX204.00   Metric: 10
        IPv6 Neighbor Address: 2001:0:302:353::302
        Global IPv6 Interface Address: 2001:0:302:353::353
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
      Reachability          : 2001:0:59:352::/64 Metric: 30 Type: 1 Down
      Reachability          : 2001:0:302:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:307:352::/64 Metric: 20 Type: 1 Down
      Reachability          : 2001:0:307:353::/64 Metric: 10 Type: 1 Down
      Reachability          : 2002::28/128 Metric: 60 Type: 1 Down
      Reachability          : 2002::59/128 Metric: 30 Type: 1 Down
      Reachability          : 2002::307/128 Metric: 10 Type: 1 Down
      Reachability          : 2002::352/128 Metric: 30 Type: 1 Down
      Reachability          : 2002::353/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:59::/48 Metric: 30 Type: 1 Down
      Reachability          : fcbb:0:307::/48 Metric: 10 Type: 1 Down
      Reachability          : fcbb:0:1353::/48 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:28:336::/64 Metric: 70 Type: 1 Down
      Reachability          : 2001:0:59:161::/64 Metric: 40 Type: 1 Down
      Reachability          : 2001:1:59:352::/64 Metric: 40 Type: 1 Down
      Reachability          : 2002::20/128 Metric: 40 Type: 1 Down
      Reachability          : 2002::36/128 Metric: 30 Type: 1 Down
      Reachability          : 2002::161/128 Metric: 50 Type: 1 Down
      Reachability          : 2002::316/128 Metric: 60 Type: 1 Down
      Reachability          : 2002::336/128 Metric: 60 Type: 1 Down
      Reachability          : 2002::342/128 Metric: 60 Type: 1 Down
      Reachability          : fcbb:0:161::/48 Metric: 50 Type: 1 Down
      Reachability          : fcbb:0:352::/48 Metric: 21 Type: 1 Down
      Reachability          : 2001:0:11:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:20:36::/64 Metric: 40 Type: 1 Down
      Reachability          : 2001:0:28:316::/64 Metric: 70 Type: 1 Down
      Reachability          : 2001:0:161:342::/64 Metric: 50 Type: 1 Down
      Reachability          : 2001:0:316:342::/64 Metric: 60 Type: 1 Down
      Reachability          : 2001:1:20:36::/64 Metric: 50 Type: 1 Down
      Reachability          : 2001:1:28:36::/64 Metric: 60 Type: 1 Down
      Reachability          : fcbb:0:20::/48 Metric: 40 Type: 1 Down
      Reachability          : fcbb:0:28::/48 Metric: 60 Type: 1 Down
      Reachability          : fcbb:0:36::/48 Metric: 30 Type: 1 Down
      Reachability          : fcbb:0:316::/48 Metric: 60 Type: 1 Down
      Reachability          : fcbb:0:336::/48 Metric: 50 Type: 1 Down
      Reachability          : fcbb:0:342::/48 Metric: 51 Type: 1 Down
      Reachability          : fcbb:0:1353::/48 Metric: 41 Type: 1 Down
      SRv6 Locator: fcbb:0:20::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: [D]
      SRv6 Locator: fcbb:0:28::/48 Topology: 0
        Metric: 60 Algorithm: 0 Flags: [D]
      SRv6 Locator: fcbb:0:36::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: [D]
      SRv6 Locator: fcbb:0:59::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: [D]
      SRv6 Locator: fcbb:0:161::/48 Topology: 0
        Metric: 50 Algorithm: 0 Flags: [D]
      SRv6 Locator: fcbb:0:307::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: [D]
      SRv6 Locator: fcbb:0:316::/48 Topology: 0
        Metric: 60 Algorithm: 0 Flags: [D]
      SRv6 Locator: fcbb:0:336::/48 Topology: 0
        Metric: 50 Algorithm: 0 Flags: [D]
      SRv6 Locator: fcbb:0:342::/48 Topology: 0
        Metric: 51 Algorithm: 0 Flags: [D]
      SRv6 Locator: fcbb:0:352::/48 Topology: 0
        Metric: 21 Algorithm: 0 Flags: [D]
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
    Nokia_58-SR1-3-SRv6.00-00       358  11214 61631    161 L2 <DefaultAtt>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia_58-SR1-3-SRv6
      Area addresses:
        49.0000
        49.0001
      SRv6 Locator: fcbb:1:1058::/48 Topology: 0
        Metric: 0 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:1058::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.0.58 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0
    Nokia_58-SR1-3-SRv6.00-01       362  47994 59931   1050 L2 <>
      Interface address: 10.0.0.58
      Interface address: 2001:0:29:58::58
      Interface address: 2001:0:36:58::58
      Interface address: 2001:0:58:310::58
      Interface address: 2001:0:58:419::58
      Interface address: 2002::58
      IS Neighbor          : h3c_29_S12500R-2L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:29:58::29
        Global IPv6 Interface Address: 2001:0:29:58::58
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::310
        Global IPv6 Interface Address: 2001:0:58:310::58
      Reachability         : 10.0.0.58/32 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:20:36::/64 Metric: 20 Type: 1 Down
      Reachability          : 2001:0:28:316::/64 Metric: 50 Type: 1 Down
      Reachability          : 2001:0:28:336::/64 Metric: 50 Type: 1 Down
      Reachability          : 2001:0:29:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:59:161::/64 Metric: 60 Type: 1 Down
      Reachability          : 2001:0:59:352::/64 Metric: 50 Type: 1 Down
      Reachability          : 2001:0:161:342::/64 Metric: 70 Type: 1 Down
      Reachability          : 2001:0:307:352::/64 Metric: 40 Type: 1 Down
      Reachability          : 2001:0:307:353::/64 Metric: 30 Type: 1 Down
      Reachability          : 2001:0:316:342::/64 Metric: 60 Type: 1 Down
      Reachability          : 2001:1:20:36::/64 Metric: 30 Type: 1 Down
      Reachability          : 2001:1:28:36::/64 Metric: 40 Type: 1 Down
      Reachability          : 2001:1:59:352::/64 Metric: 60 Type: 1 Down
      Reachability          : fcbb:0:59::/48 Metric: 50 Type: 1 Down
      Reachability          : fcbb:0:161::/48 Metric: 70 Type: 1 Down
      Reachability          : fcbb:0:307::/48 Metric: 30 Type: 1 Down
      Reachability          : fcbb:0:316::/48 Metric: 50 Type: 1 Down
      Reachability          : fcbb:0:336::/48 Metric: 30 Type: 1 Down
      Reachability          : fcbb:0:342::/48 Metric: 61 Type: 1 Down
      Reachability          : fcbb:0:352::/48 Metric: 41 Type: 1 Down
      SRv6 Locator: fcbb:0:59::/48 Topology: 0
        Metric: 50 Algorithm: 0 Flags: [D]
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:59::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:0:161::/48 Topology: 0
        Metric: 70 Algorithm: 0 Flags: [D]
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:161::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:0:307::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: [D]
      SRv6 Locator: fcbb:0:316::/48 Topology: 0
        Metric: 50 Algorithm: 0 Flags: [D]
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:0:316::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:0:336::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: [D]
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:0:336::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:0:342::/48 Topology: 0
        Metric: 61 Algorithm: 0 Flags: [D]
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:342::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:0:352::/48 Topology: 0
        Metric: 41 Algorithm: 0 Flags: [D]
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:352::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
    Nokia_58-SR1-3-SRv6.00-02        26  22771 61741    834 L2 <>
      IS Neighbor          : Keys-Ixia-419.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:58:419::419
        Global IPv6 Interface Address: 2001:0:58:419::58
      Reachability          : 2002::20/128 Metric: 20 Type: 1 Down
      Reachability          : 2002::28/128 Metric: 40 Type: 1 Down
      Reachability          : 2002::36/128 Metric: 10 Type: 1 Down
      Reachability          : 2002::58/128 Metric: 0 Type: 1 Up
      Reachability          : 2002::59/128 Metric: 50 Type: 1 Down
      Reachability          : 2002::161/128 Metric: 70 Type: 1 Down
      Reachability          : 2002::307/128 Metric: 30 Type: 1 Down
      Reachability          : 2002::316/128 Metric: 50 Type: 1 Down
      Reachability          : 2002::336/128 Metric: 40 Type: 1 Down
      Reachability          : 2002::342/128 Metric: 70 Type: 1 Down
      Reachability          : 2002::352/128 Metric: 50 Type: 1 Down
      Reachability          : fcbb:0:20::/48 Metric: 20 Type: 1 Down
      Reachability          : fcbb:0:28::/48 Metric: 40 Type: 1 Down
      Reachability          : fcbb:0:36::/48 Metric: 10 Type: 1 Down
      Reachability          : fcbb:0:1058::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:20::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: [D]
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
      SRv6 Locator: fcbb:0:28::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: [D]
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:28::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 0
      SRv6 Locator: fcbb:0:36::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: [D]
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
      SRv6 Locator: fcbb:0:1058::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1058::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
    Keys-Ixia-419.00-00         158  46061   783    351 L2 <DefaultAtt>
      Remaining lifetime received: 1198 s Modified to: 1200 s
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

