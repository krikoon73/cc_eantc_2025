# Test results for PE41-J2-161

## show version

```text
Arista DCS-7280SR3-40YC6-F
Hardware version: 11.02
Serial number: JPA2339P1RL
Hardware MAC address: 606b.5b2e.fe11
System MAC address: 606b.5b2e.fe11

Software image version: 4.32.0F-35668851.binoshmonsrv6EFTFeb20240 (engineering build)
Architecture: x86_64
Internal build version: 4.32.0F-35668851.binoshmonsrv6EFTFeb20240
Internal build ID: 93cbcec4-274c-4247-b5c2-478b9fcaa07c
Image format version: 3.0
Image optimization: Default

Uptime: 20 hours and 22 minutes
Total memory: 8099732 kB
Free memory: 5181140 kB

```

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
Last table change time   : 0:00:33 ago
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
srv6      default  Cisco342-9902    L2   Ethernet10         P2P               UP    26          00                  
srv6      default  Nokia-59-IXRe2   L2   Ethernet20         P2P               UP    21          00                  
```

## show segment-routing ipv6 locator

```text
SRv6 configuration for VRF default
Administrative status: enabled
Operational status: enabled
Encapsulation source address: 2002::161
Number of configured locators: 1

Locator uSID-LOC-161
State: active
Type: micro-SID
Micro-SID domain: SRv6-uSID-161
Prefix: fcbb:0:161::/48
IGP algorithm: SPF
Block length: 32
Function length: 16
Function allocator: micro-SID::SRv6-uSID-161
SID function value pools: default
```

## show segment-routing ipv6 locator std

```text
SRv6 configuration for VRF default
Administrative status: enabled
Operational status: enabled
Encapsulation source address: 2002::161
Number of configured locators: 1
```

## show segment-routing ipv6 sid function allocators

```text
SRv6 SID function allocators for VRF default

Allocator micro-SID::SRv6-uSID-161
Function length: 16
Locator users: uSID-LOC-161
Start   End  Size Usage        
----- ----- ----- -------------
    1  1023  1023 static       
 1024  5119  4096 bgp (dynamic)
 5120  9215  4096 bgp (dynamic)
 9216 65535 56320 unassigned   

```

## show segment-routing ipv6 capabilities

```text
```

## show segment-routing ipv6 route

```text
VRF default
Source Codes: B3 - BGP L3 VPN, S - Static
End Behaviors: End - Endpoint
               End.DT4 (6) - Endpoint with decapsulation and specific IPv4 (6) table lookup

B3  fcbb:0:161:400::/64, End.DT4 with NEXT-CSID, locator uSID-LOC-161
    via IPv4 lookup, VRF VPNv4-uSID
B3  fcbb:0:161:401::/64, End.DT6 with NEXT-CSID, locator uSID-LOC-161
    via IPv6 lookup, VRF VPNv4-uSID
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.161, local AS number 1
Neighbor Status Codes: m - Under maintenance
  Neighbor  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  2002::353 4 1               1601      1430    0    0 00:00:15 Estab   0      0
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
```

## show tunnel fib

```text

Type 'SRv6 Transport', index 100, endpoint fcbb:0:1029::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 101, endpoint fcbb:0:1338::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 102, endpoint fcbb:0:1344::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 103, endpoint fcbb:0:1162::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 104, endpoint fcbb:0:1302::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 105, endpoint fcbb:0:336::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 106, endpoint fcbb:0:59::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 107, endpoint fcbb:0:1011::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 108, endpoint fcbb:0:352::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 109, endpoint fcbb:0:1199::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 110, endpoint fcbb:0:1310::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 111, endpoint fcbb:0:307::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 112, endpoint fcbb:0:342::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 113, endpoint fcbb:0:1058::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 114, endpoint fcbb:0:316::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 115, endpoint fcbb:0:28::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 116, endpoint fcbb:0:1353::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161
```

## show bgp neighbors 2002::353 vpn-ipv4 advertised-routes detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
BGP routing table entry for IPv4 prefix 20.161.225.0/24, Route Distinguisher: 1:161
 Paths: 1 available
  Local
    2002::161 from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1:20
      Local SRv6 SID (VRF SID): fcbb:0:161:400::/64, End.DT4 with NEXT-CSID
```

## show bgp neighbors 2002::353 vpn-ipv6 advertised-routes detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
BGP routing table entry for IPv6 prefix 2001:20:161:225::/64, Route Distinguisher: 1:161
 Paths: 1 available
  Local
    2002::161 from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1:20
      Local SRv6 SID (VRF SID): fcbb:0:161:401::/64, End.DT6 with NEXT-CSID
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
 * >      RD: 10.0.0.11:1 IPv4 prefix 20.11.225.0/24
                                 2002::11              -       100     0       ? Or-ID: 10.0.0.11 C-LST: 100.0.0.53 
 * >      RD: 1:28 IPv4 prefix 20.28.225.0/24
                                 2002::28              0       100     0       ? Or-ID: 192.168.20.28 C-LST: 100.0.0.53 
 * >      RD: 1:29 IPv4 prefix 20.29.225.0/24
                                 2002::29              0       100     0       ? Or-ID: 192.168.20.29 C-LST: 100.0.0.53 
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
 * >      RD: 1:28 IPv6 prefix 2001:20:28:225::/64
                                 2002::28              0       100     0       ? Or-ID: 192.168.20.28 C-LST: 100.0.0.53 
 * >      RD: 1:29 IPv6 prefix 2001:20:29:225::/64
                                 2002::29              0       100     0       ? Or-ID: 192.168.20.29 C-LST: 100.0.0.53 
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
 * >      RD: 1:336 IPv6 prefix 2001:20:336:225::/64
                                 2002::336             -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
 * >      RD: 1:338 IPv6 prefix 2001:20:338:225::/64
                                 2002::338             -       100     0       ? Or-ID: 10.0.1.38 C-LST: 100.0.0.53 
```

## show ipv6 route

```text

VRF: default
Displaying 70 of 75 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 I L2     2001:0:11:310::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:11:353::/64 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:19:344::/64 [115/90]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:20:36::/64 [115/60]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:0:28:316::/64 [115/30]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:0:28:336::/64 [115/40]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:0:29:58::/64 [115/80]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:36:58::/64 [115/70]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:0:49:199::/64 [115/90]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:58:310::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:58:419::/64 [115/80]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2001:0:59:161::/64 [0/0]
           via Ethernet20, directly connected
 I L2     2001:0:59:352::/64 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2001:0:161:342::/64 [0/0]
           via Ethernet10, directly connected
 I L2     2001:0:162:302::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:162:344::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:199:344::/64 [115/80]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:302:353::/64 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:307:352::/64 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:307:353::/64 [115/40]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:316:342::/64 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:1:20:36::/64 [115/50]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:1:28:36::/64 [115/50]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:1:29:38::/64 [115/100]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:1:38:49::/64 [115/100]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:1:59:352::/64 [115/20]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::11/128 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::20/128 [115/50]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::28/128 [115/30]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::29/128 [115/80]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::36/128 [115/60]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::49/128 [115/100]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::58/128 [115/70]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::59/128 [115/10]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2002::161/128 [0/0]
           via Loopback0, directly connected
 I L2     2002::162/128 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::199/128 [115/80]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::302/128 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::307/128 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::310/128 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::316/128 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::336/128 [115/50]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::338/128 [115/100]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::342/128 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::344/128 [115/80]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::352/128 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::353/128 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::419/128 [115/90]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002:0:29:338::/64 [115/90]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:20::/48 [115/50]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:28::/48 [115/30]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:36::/48 [115/60]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:59::/48 [115/10]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:307::/48 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:316::/48 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:336::/48 [115/40]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:342::/48 [115/11]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:352::/48 [115/21]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:419::/48 [115/80]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1011::/48 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1029::/48 [115/80]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1049::/48 [115/90]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1058::/48 [115/70]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1162::/48 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1199::/48 [115/80]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1302::/48 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1310::/48 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1338::/48 [115/90]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1344::/48 [115/71]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1353::/48 [115/41]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20

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

 C        100.0.0.161/32
           directly connected, Loopback0


VRF: EVPNv4-T5-uSID
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
           via fcbb:0:1011::/48, SRv6 Transport tunnel index 107, SRv6 SID fcbb:0:1011:e000::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.28.225.0/24 [200/0]
           via fcbb:0:28::/48, SRv6 Transport tunnel index 115, SRv6 SID fcbb:0:28:e100::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.29.225.0/24 [200/0]
           via fcbb:0:1029::/48, SRv6 Transport tunnel index 100, SRv6 SID fcbb:0:1029:e100::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.58.225.0/24 [200/0]
           via fcbb:0:1058::/48, SRv6 Transport tunnel index 113, SRv6 SID fcbb:0:1058:e017::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.59.225.0/24 [200/0]
           via fcbb:0:59::/48, SRv6 Transport tunnel index 106, SRv6 SID fcbb:0:59:e017::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.102.225.0/24 [200/0]
           via fcbb:0:1302::/48, SRv6 Transport tunnel index 104, SRv6 SID fcbb:0:1302:e000::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.107.225.0/24 [200/0]
           via fcbb:0:307::/48, SRv6 Transport tunnel index 111, SRv6 SID fcbb:0:307:e000::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.110.225.0/24 [200/0]
           via fcbb:0:1310::/48, SRv6 Transport tunnel index 110, SRv6 SID fcbb:0:1310:e000::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.116.225.0/24 [200/0]
           via fcbb:0:316::/48, SRv6 Transport tunnel index 114, SRv6 SID fcbb:0:316:e002::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.136.225.0/24 [200/0]
           via fcbb:0:336::/48, SRv6 Transport tunnel index 105, SRv6 SID fcbb:0:336:e664::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.138.225.0/24 [200/0]
           via fcbb:0:1338::/48, SRv6 Transport tunnel index 101, SRv6 SID fcbb:0:1338:e666::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
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
           via fcbb:0:1162::/48, SRv6 Transport tunnel index 103, SRv6 SID fcbb:0:1162:400::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.199.225.0/24 [200/0]
           via fcbb:0:1199::/48, SRv6 Transport tunnel index 109, SRv6 SID fcbb:0:1199:e1b7::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20


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

## show ipv6 route vrf all

```text

VRF: default
Displaying 70 of 75 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 I L2     2001:0:11:310::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:11:353::/64 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:19:344::/64 [115/90]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:20:36::/64 [115/60]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:0:28:316::/64 [115/30]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:0:28:336::/64 [115/40]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:0:29:58::/64 [115/80]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:36:58::/64 [115/70]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:0:49:199::/64 [115/90]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:58:310::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:58:419::/64 [115/80]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2001:0:59:161::/64 [0/0]
           via Ethernet20, directly connected
 I L2     2001:0:59:352::/64 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2001:0:161:342::/64 [0/0]
           via Ethernet10, directly connected
 I L2     2001:0:162:302::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:162:344::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:199:344::/64 [115/80]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:302:353::/64 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:307:352::/64 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:307:353::/64 [115/40]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:316:342::/64 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:1:20:36::/64 [115/50]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:1:28:36::/64 [115/50]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:1:29:38::/64 [115/100]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:1:38:49::/64 [115/100]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:1:59:352::/64 [115/20]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::11/128 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::20/128 [115/50]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::28/128 [115/30]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::29/128 [115/80]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::36/128 [115/60]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::49/128 [115/100]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::58/128 [115/70]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::59/128 [115/10]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2002::161/128 [0/0]
           via Loopback0, directly connected
 I L2     2002::162/128 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::199/128 [115/80]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::302/128 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::307/128 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::310/128 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::316/128 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::336/128 [115/50]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::338/128 [115/100]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::342/128 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::344/128 [115/80]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::352/128 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::353/128 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::419/128 [115/90]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002:0:29:338::/64 [115/90]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:20::/48 [115/50]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:28::/48 [115/30]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:36::/48 [115/60]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:59::/48 [115/10]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:307::/48 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:316::/48 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:336::/48 [115/40]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:342::/48 [115/11]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:352::/48 [115/21]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:419::/48 [115/80]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1011::/48 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1029::/48 [115/80]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1049::/48 [115/90]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1058::/48 [115/70]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1162::/48 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1199::/48 [115/80]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1302::/48 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1310::/48 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1338::/48 [115/90]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1344::/48 [115/71]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1353::/48 [115/41]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20


VRF: EVPNv4-T5-uSID
Displaying 0 of 3 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route



VRF: VPNv4-uSID
Displaying 17 of 21 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 B I      2001:20:28:225::/64 [200/0]
           via fcbb:0:28::/48, SRv6 Transport tunnel index 115, SRv6 SID fcbb:0:28:e101::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:29:225::/64 [200/0]
           via fcbb:0:1029::/48, SRv6 Transport tunnel index 100, SRv6 SID fcbb:0:1029:e101::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:58:225::/64 [200/0]
           via fcbb:0:1058::/48, SRv6 Transport tunnel index 113, SRv6 SID fcbb:0:1058:e018::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:59:225::/64 [200/0]
           via fcbb:0:59::/48, SRv6 Transport tunnel index 106, SRv6 SID fcbb:0:59:e018::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:102:225::/64 [200/0]
           via fcbb:0:1302::/48, SRv6 Transport tunnel index 104, SRv6 SID fcbb:0:1302:e001::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:107:225::/64 [200/0]
           via fcbb:0:307::/48, SRv6 Transport tunnel index 111, SRv6 SID fcbb:0:307:e001::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:110:225::/64 [200/0]
           via fcbb:0:1310::/48, SRv6 Transport tunnel index 110, SRv6 SID fcbb:0:1310:e001::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:116:225::/64 [200/0]
           via fcbb:0:316::/48, SRv6 Transport tunnel index 114, SRv6 SID fcbb:0:316:e003::
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
           via fcbb:0:1162::/48, SRv6 Transport tunnel index 103, SRv6 SID fcbb:0:1162:401::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:199:225::/64 [200/0]
           via fcbb:0:1199::/48, SRv6 Transport tunnel index 109, SRv6 SID fcbb:0:1199:e1b8::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:336:225::/64 [200/0]
           via fcbb:0:336::/48, SRv6 Transport tunnel index 105, SRv6 SID fcbb:0:336:e665::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:338:225::/64 [200/0]
           via fcbb:0:1338::/48, SRv6 Transport tunnel index 101, SRv6 SID fcbb:0:1338:e667::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
              via fe80::fa7a:41ff:fe18:8910, Ethernet10


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

## show isis database detail

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: srv6 VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    CIEN-11-5169.00-00          411   7611  1194   1089 L2  0000.0000.0011.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: CIEN-11-5169
      Area addresses: 49.0001
      Interface address: 2001:0:11:353::11
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:11:310::310
        Global IPv6 Interface Address: 2001:0:11:310::11
        Adj-sid: 24002 flags: [L V F] weight: 0x0
      IS Neighbor          : Cisco353-8201-24H8FH.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:11:353::353
        Global IPv6 Interface Address: 2001:0:11:353::11
        Adj-sid: 24003 flags: [L V F] weight: 0x0
      Reachability         : 10.0.0.11/32 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:11:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::11/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:1011::/48 Metric: 10 Type: 1 Up
      Reachability          : 2002::310/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1310::/48 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:19:344::/64 Metric: 60 Type: 1 Up
      Reachability          : 2001:0:29:58::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 60 Type: 1 Up
      Reachability          : 2001:0:162:302::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:162:344::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:0:199:344::/64 Metric: 50 Type: 1 Up
      Reachability          : 2001:0:302:353::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:1:29:38::/64 Metric: 50 Type: 1 Up
      Reachability          : 2001:1:38:49::/64 Metric: 50 Type: 1 Up
      Reachability          : 2002::29/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::49/128 Metric: 60 Type: 1 Up
      Reachability          : 2002::58/128 Metric: 20 Type: 1 Up
      Reachability          : 2002::162/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::199/128 Metric: 50 Type: 1 Up
      Reachability          : 2002::302/128 Metric: 20 Type: 1 Up
      Reachability          : 2002::338/128 Metric: 50 Type: 1 Up
      Reachability          : 2002::344/128 Metric: 50 Type: 1 Up
      Reachability          : 2002::353/128 Metric: 20 Type: 1 Up
      Reachability          : 2002:0:29:338::/64 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1029::/48 Metric: 30 Type: 1 Up
      Reachability          : fcbb:0:1049::/48 Metric: 50 Type: 1 Up
      Reachability          : fcbb:0:1058::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:1162::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1199::/48 Metric: 50 Type: 1 Up
      Reachability          : fcbb:0:1302::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:1338::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1344::/48 Metric: 41 Type: 1 Up
      Reachability          : fcbb:0:1353::/48 Metric: 11 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 30 Type: 1 Up
      Reachability          : 2002::419/128 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:419::/48 Metric: 40 Type: 1 Up
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
    h3c_20_CR16010E-F.00-00       564  23467  1004    571 L2  0000.0000.0020.00-00  <>
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
    h3c_28_S12500R-2L.00-00       251  59659  1096    428 L2  0000.0000.0028.00-00  <>
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
    huawei_36.00-00             413  31563  1169    693 L2  0000.0000.0036.00-00  <>
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
    anet-161-R3.00-00           422  55992  1172    250 L2  0000.0000.0161.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 872 s
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
    JNPR-307-ACX7024.00-00       147  56726  1172    343 L2  0000.0000.0307.00-00  <>
      Remaining lifetime received: 700 s Modified to: 1200 s
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
      Reachability          : 2002::307/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:307:352::/64 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:307::/48 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:307:353::/64 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:307::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
      Router Capabilities: Router Id: 10.0.1.7 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    JNPR-310-ACX7100-48L.00-00       626  53148  1191   1238 L2  0000.0000.0310.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: JNPR-310-ACX7100-48L
      Area addresses: 49.0001
      Interface address: 10.0.1.10
      Reachability          : 2002::310/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:1310::/48 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:11:353::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:162:302::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:0:162:344::/64 Metric: 50 Type: 1 Up
      Reachability          : 2001:0:199:344::/64 Metric: 60 Type: 1 Up
      Reachability          : 2001:0:302:353::/64 Metric: 30 Type: 1 Up
      Reachability          : 2002::11/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::162/128 Metric: 50 Type: 1 Up
      Reachability          : 2002::302/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::344/128 Metric: 60 Type: 1 Up
      Reachability          : 2002::353/128 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:19:344::/64 Metric: 60 Type: 1 Up
      Reachability          : 2001:0:29:58::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 50 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:1:29:38::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:1:38:49::/64 Metric: 40 Type: 1 Up
      Reachability          : 2002::29/128 Metric: 20 Type: 1 Up
      Reachability          : 2002::49/128 Metric: 50 Type: 1 Up
      Reachability          : 2002::58/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::199/128 Metric: 50 Type: 1 Up
      Reachability          : 2002::338/128 Metric: 40 Type: 1 Up
      Reachability          : 2002:0:29:338::/64 Metric: 30 Type: 1 Up
      Reachability          : 2002::419/128 Metric: 30 Type: 1 Up
      SRv6 Locator: fcbb:0:1310::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1011::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1011::
      SRv6 Locator: fcbb:0:1162::/48 Topology: 0
        Metric: 50 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1162::
      SRv6 Locator: fcbb:0:1302::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:0:1302::
      SRv6 Locator: fcbb:0:1344::/48 Topology: 0
        Metric: 51 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1344::
      SRv6 Locator: fcbb:0:1353::/48 Topology: 0
        Metric: 21 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1353::
      SRv6 Locator: fcbb:0:1029::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1029::
      SRv6 Locator: fcbb:0:1049::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1049::
      SRv6 Locator: fcbb:0:1058::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1058::
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
      SRv6 Locator: fcbb:0:1338::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:0:1338::
      SRv6 Locator: fcbb:0:419::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:419:11::
      Router Capabilities: Router Id: 10.0.1.10 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    JNPR-310-ACX7100-48L.00-01       330  35458  1192    343 L2  0000.0000.0310.00-01  <>
      IS Neighbor          : CIEN-11-5169.00     Metric: 10
        IPv6 Neighbor Address: 2001:0:11:310::11
        Global IPv6 Interface Address: 2001:0:11:310::310
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::58
        Global IPv6 Interface Address: 2001:0:58:310::310
      Reachability          : 2001:0:11:310::/64 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1011::/48 Metric: 10 Type: 1 Down
      Reachability          : fcbb:0:1162::/48 Metric: 50 Type: 1 Down
      Reachability          : fcbb:0:1302::/48 Metric: 30 Type: 1 Down
      Reachability          : fcbb:0:1344::/48 Metric: 51 Type: 1 Down
      Reachability          : fcbb:0:1353::/48 Metric: 21 Type: 1 Down
      Reachability          : fcbb:0:1029::/48 Metric: 20 Type: 1 Down
      Reachability          : fcbb:0:1049::/48 Metric: 40 Type: 1 Down
      Reachability          : fcbb:0:1058::/48 Metric: 10 Type: 1 Down
      Reachability          : fcbb:0:1199::/48 Metric: 50 Type: 1 Down
      Reachability          : fcbb:0:1338::/48 Metric: 30 Type: 1 Down
      Reachability          : fcbb:0:419::/48 Metric: 20 Type: 1 Down
    JNPR-316-MX304.00-00        228  28540   555    369 L2  0000.0000.0316.00-00  <>
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
    ZTE_336_ZXR10_M6000-8SE.00-00       448   2265   825    474 L2  0000.0000.0336.00-00  <>
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
    Cisco342-9902.00-00         232  17526   487    417 L2  0000.0000.0342.00-00  <>
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
    Cisco352-N540.00-00         396  46182  1173    435 L2  0000.0000.0352.00-00  <>
      Remaining lifetime received: 1190 s Modified to: 1200 s
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
    Cisco353-8201-24H8FH.00-00       616  12540  1193   1356 L2  0000.0000.0353.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: Cisco353-8201-24H8FH
      Area addresses:
        49.0000.0000.0058.00
        49.0001
      Interface address: 2002::353
      IS Neighbor          : CIEN-11-5169.00     Metric: 10
        IPv6 Neighbor Address: 2001:0:11:353::11
        Global IPv6 Interface Address: 2001:0:11:353::353
      IS Neighbor          : JNPR-307-ACX7024.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:307:353::307
        Global IPv6 Interface Address: 2001:0:307:353::353
      Reachability          : 2001:0:11:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:302:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:307:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::49/128 Metric: 60 Type: 1 Up
      Reachability          : 2002::162/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::199/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::302/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::338/128 Metric: 60 Type: 1 Up
      Reachability          : 2002::344/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::353/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1353::/48 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:19:344::/64 Metric: 50 Type: 1 Up
      Reachability          : 2001:0:162:302::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:162:344::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:199:344::/64 Metric: 40 Type: 1 Up
      Reachability          : 2002::11/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::29/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::58/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::310/128 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:1049::/48 Metric: 50 Type: 1 Up
      Reachability          : fcbb:0:1162::/48 Metric: 30 Type: 1 Up
      Reachability          : fcbb:0:1199::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1344::/48 Metric: 31 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:29:58::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 50 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:1:29:38::/64 Metric: 60 Type: 1 Up
      Reachability          : 2001:1:38:49::/64 Metric: 60 Type: 1 Up
      Reachability          : 2002:0:29:338::/64 Metric: 50 Type: 1 Up
      Reachability          : fcbb:0:1011::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:1029::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1058::/48 Metric: 30 Type: 1 Up
      Reachability          : fcbb:0:1310::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:1338::/48 Metric: 50 Type: 1 Up
      Reachability          : 2002::419/128 Metric: 50 Type: 1 Up
      Reachability          : fcbb:0:419::/48 Metric: 50 Type: 1 Up
      Reachability          : fcbb:0:1302::/48 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:419::/48 Topology: 0
        Metric: 50 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1011::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1029::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1049::/48 Topology: 0
        Metric: 50 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1058::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1162::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1199::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1302::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1310::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1338::/48 Topology: 0
        Metric: 50 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1344::/48 Topology: 0
        Metric: 31 Algorithm: 0 Flags: []
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
    Nokia_58-SR1-3-SRv6.00-00       433  39737 62559    346 L2  0100.0000.0058.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia_58-SR1-3-SRv6
      Area addresses:
        49.0000.0000.0058.00
        49.0001
      Reachability          : fcbb:0:1199::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1344::/48 Metric: 51 Type: 1 Up
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
      SRv6 Locator: fcbb:0:1344::/48 Topology: 0
        Metric: 51 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1344::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.0.58 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0
    Nokia_58-SR1-3-SRv6.00-01       271  16697 65529   1377 L2  0100.0000.0058.00-01  <>
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
      Reachability          : 2001:0:19:344::/64 Metric: 50 Type: 1 Up
      Reachability          : 2001:0:29:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:162:302::/64 Metric: 50 Type: 1 Up
      Reachability          : 2001:0:162:344::/64 Metric: 60 Type: 1 Up
      Reachability          : 2001:0:199:344::/64 Metric: 60 Type: 1 Up
      Reachability          : 2001:0:302:353::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:1:29:38::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:1:38:49::/64 Metric: 30 Type: 1 Up
      Reachability          : 2002::11/128 Metric: 20 Type: 1 Up
      Reachability          : 2002::29/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::49/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::58/128 Metric: 0 Type: 1 Up
      Reachability          : 2002::162/128 Metric: 60 Type: 1 Up
      Reachability          : 2002::199/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::302/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::310/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::338/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::344/128 Metric: 60 Type: 1 Up
      Reachability          : 2002::353/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::419/128 Metric: 20 Type: 1 Up
      Reachability          : 2002:0:29:338::/64 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:419::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1011::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:1029::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1049::/48 Metric: 30 Type: 1 Up
      Reachability          : fcbb:0:1058::/48 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:1162::/48 Metric: 60 Type: 1 Up
      Reachability          : fcbb:0:1302::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1310::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1338::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:1353::/48 Metric: 31 Type: 1 Up
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
      SRv6 Locator: fcbb:0:1049::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1049::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:0:1058::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1058::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:0:1162::/48 Topology: 0
        Metric: 60 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1162::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:0:1302::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
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
      SRv6 Locator: fcbb:0:1353::/48 Topology: 0
        Metric: 31 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1353::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
    Nokia-59-IXRe2.00-00        202  46557  1173    488 L2  0100.0000.0059.00-00  <>
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
    Keys-Ixia-419.00-00         128  61391    64    351 L2  3800.0000.0419.00-00  <DefaultAtt>
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

## show isis segment-routing ipv6 locators

```text
Locator: fcbb:0:1058::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1058::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1058::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:161::/48
System ID: anet-161-R3
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:20::/48
System ID: h3c_20_CR16010E-F
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:316::/48
System ID: JNPR-316-MX304
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1199::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1199::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1199::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:342::/48
System ID: Cisco342-9902
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:419::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:419::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:419::/48
System ID: Keys-Ixia-419
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:419::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1302::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1302::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1302::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1049::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1049::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1049::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:36::/48
System ID: huawei_36
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1011::/48
System ID: CIEN-11-5169
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1011::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1011::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1011::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:307::/48
System ID: JNPR-307-ACX7024
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1310::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1310::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1310::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:352::/48
System ID: Cisco352-N540
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:59::/48
System ID: Nokia-59-IXRe2
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:28::/48
System ID: h3c_28_S12500R-2L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1353::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1353::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1353::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1029::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1029::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1029::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1162::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1162::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1162::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:336::/48
System ID: ZTE_336_ZXR10_M6000-8SE
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1338::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1338::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1338::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1344::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1344::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1344::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

```

## show interfaces

```text
Ethernet1 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe12 (bia 606b.5b2e.fe12)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet2 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe13 (bia 606b.5b2e.fe13)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet3 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe14 (bia 606b.5b2e.fe14)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet4 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe15 (bia 606b.5b2e.fe15)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet5 is up, line protocol is up (connected)
  Hardware is Ethernet, address is 606b.5b2e.fe16 (bia 606b.5b2e.fe16)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 10000000 kbit
  Full-duplex, 10Gb/s, auto negotiation: off, uni-link: disabled
  Up 20 hours, 18 minutes, 28 seconds
  Loopback Mode : None
  2 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 7 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 497 bps (0.0% with framing overhead), 1 packets/sec
     2437 packets input, 494711 bytes
     Received 0 broadcasts, 2437 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     38262 packets output, 5030480 bytes
     Sent 0 broadcasts, 38262 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet6 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe17 (bia 606b.5b2e.fe17)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet7 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe18 (bia 606b.5b2e.fe18)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet8 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe19 (bia 606b.5b2e.fe19)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet9 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe1a (bia 606b.5b2e.fe1a)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet10 is up, line protocol is up (connected)
  Hardware is Ethernet, address is 606b.5b2e.fe11
  IPv6 link-local address is fe80::626b:5bff:fe2e:fe11/64
  IPv6 global unicast address(es):
    2001:0:161:342::161, subnet is 2001:0:161:342::/64
  IP MTU 9214 bytes, Ethernet MRU 10240 bytes, BW 10000000 kbit
  Full-duplex, 10Gb/s, auto negotiation: off, uni-link: disabled
  Up 20 hours, 18 minutes, 30 seconds
  Loopback Mode : None
  2 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 22.7 Mbps (0.2% with framing overhead), 2749 packets/sec
  5 seconds output rate 17.5 Mbps (0.2% with framing overhead), 2124 packets/sec
     13037571 packets input, 13353017193 bytes
     Received 0 broadcasts, 13086 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     8809349 packets output, 7502094784 bytes
     Sent 0 broadcasts, 21413 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet11 is up, line protocol is up (connected)
  Hardware is Ethernet, address is 606b.5b2e.fe1c (bia 606b.5b2e.fe1c)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 10000000 kbit
  Full-duplex, 10Gb/s, auto negotiation: off, uni-link: disabled
  Up 20 hours, 18 minutes, 30 seconds
  Loopback Mode : None
  2 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 16.0 Mbps (0.2% with framing overhead), 2007 packets/sec
  5 seconds output rate 18.9 Mbps (0.2% with framing overhead), 2369 packets/sec
     9449353 packets input, 7433063990 bytes
     Received 4 broadcasts, 2678 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     9816263 packets output, 9707950718 bytes
     Sent 0 broadcasts, 38679 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet12 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe1d (bia 606b.5b2e.fe1d)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet13 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe1e (bia 606b.5b2e.fe1e)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet14 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe1f (bia 606b.5b2e.fe1f)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet15 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe20 (bia 606b.5b2e.fe20)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet16 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe21 (bia 606b.5b2e.fe21)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet17 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe22 (bia 606b.5b2e.fe22)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet18 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe23 (bia 606b.5b2e.fe23)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet19 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe24 (bia 606b.5b2e.fe24)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet20 is up, line protocol is up (connected)
  Hardware is Ethernet, address is 606b.5b2e.fe11
  IPv6 link-local address is fe80::626b:5bff:fe2e:fe11/64
  IPv6 global unicast address(es):
    2001:0:59:161::161, subnet is 2001:0:59:161::/64
  IP MTU 9214 bytes, Ethernet MRU 10240 bytes, BW 10000000 kbit
  Full-duplex, 10Gb/s, auto negotiation: off, uni-link: disabled
  Up 36 seconds
  Loopback Mode : None
  4 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 19.1 Mbps (0.2% with framing overhead), 2314 packets/sec
  5 seconds output rate 15.5 Mbps (0.2% with framing overhead), 1877 packets/sec
     10402635 packets input, 9707140835 bytes
     Received 0 broadcasts, 20665 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     8709272 packets output, 8916743188 bytes
     Sent 0 broadcasts, 21139 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet21 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe26 (bia 606b.5b2e.fe26)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet22 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe27 (bia 606b.5b2e.fe27)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet23 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe28 (bia 606b.5b2e.fe28)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet24 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe29 (bia 606b.5b2e.fe29)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet25 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe2a (bia 606b.5b2e.fe2a)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet26 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe2b (bia 606b.5b2e.fe2b)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet27 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe2c (bia 606b.5b2e.fe2c)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet28 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe2d (bia 606b.5b2e.fe2d)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet29 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe2e (bia 606b.5b2e.fe2e)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet30 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe2f (bia 606b.5b2e.fe2f)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet31 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe30 (bia 606b.5b2e.fe30)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet32 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe31 (bia 606b.5b2e.fe31)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet33 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe32 (bia 606b.5b2e.fe32)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet34 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe33 (bia 606b.5b2e.fe33)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet35 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe34 (bia 606b.5b2e.fe34)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet36 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe35 (bia 606b.5b2e.fe35)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet37 is down, line protocol is notpresent (errdisabled)
  Hardware is Ethernet, address is 0000.0000.0000 (bia 606b.5b2e.fe36)
  Ethernet MTU 0 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: n/a
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet38 is down, line protocol is notpresent (errdisabled)
  Hardware is Ethernet, address is 0000.0000.0000 (bia 606b.5b2e.fe37)
  Ethernet MTU 0 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: n/a
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet39 is up, line protocol is up (connected)
  Hardware is Ethernet, address is 606b.5b2e.fe38 (bia 606b.5b2e.fe38)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 10000000 kbit
  Full-duplex, 10Gb/s, auto negotiation: off, uni-link: disabled
  Up 20 hours, 18 minutes, 28 seconds
  Loopback Mode : None
  2 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 498 bps (0.0% with framing overhead), 1 packets/sec
  5 seconds output rate 9 bps (0.0% with framing overhead), 0 packets/sec
     38967 packets input, 5119499 bytes
     Received 0 broadcasts, 38967 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     2445 packets output, 627427 bytes
     Sent 0 broadcasts, 2445 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet40 is up, line protocol is up (connected)
  Hardware is Ethernet, address is 606b.5b2e.fe39 (bia 606b.5b2e.fe39)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 10000000 kbit
  Full-duplex, 10Gb/s, auto negotiation: off, uni-link: disabled
  Up 20 hours, 18 minutes, 28 seconds
  Loopback Mode : None
  2 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 498 bps (0.0% with framing overhead), 1 packets/sec
  5 seconds output rate 9 bps (0.0% with framing overhead), 0 packets/sec
     38968 packets input, 5119622 bytes
     Received 0 broadcasts, 38968 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     2440 packets output, 626812 bytes
     Sent 0 broadcasts, 2440 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet41/1 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe3a (bia 606b.5b2e.fe3a)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 100000000 kbit
  Full-duplex, 100Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet42/1 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe3e (bia 606b.5b2e.fe3e)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 100000000 kbit
  Full-duplex, 100Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet43/1 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe40 (bia 606b.5b2e.fe40)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 100000000 kbit
  Full-duplex, 100Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet44/1 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe44 (bia 606b.5b2e.fe44)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 100000000 kbit
  Full-duplex, 100Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet45/1 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe46 (bia 606b.5b2e.fe46)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 100000000 kbit
  Full-duplex, 100Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet46/1 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe4a (bia 606b.5b2e.fe4a)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 100000000 kbit
  Full-duplex, 100Gb/s, auto negotiation: off, uni-link: disabled
  Down 20 hours, 18 minutes, 49 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 0 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 0 bps (0.0% with framing overhead), 0 packets/sec
     0 packets input, 0 bytes
     Received 0 broadcasts, 0 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     0 packets output, 0 bytes
     Sent 0 broadcasts, 0 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Loopback0 is up, line protocol is up (connected)
  Hardware is Loopback
  Description: Router-ID
  Internet address is 100.0.0.161/32
  Broadcast address is 255.255.255.255
  IPv6 link-local address is fe80::ff:fe00:0/64
  IPv6 global unicast address(es):
    2002::161, subnet is 2002::161/128
  IP MTU 65535 bytes (default)
  Up 20 hours, 19 minutes, 51 seconds
Management1 is up, line protocol is up (connected)
  Hardware is Ethernet, address is 606b.5b2e.fe10 (bia 606b.5b2e.fe10)
  Internet address is 192.168.20.161/23
  Broadcast address is 255.255.255.255
  IP MTU 1500 bytes (default), BW 1000000 kbit
  Full-duplex, 1Gb/s, auto negotiation: on, uni-link: n/a
  Up 20 hours, 19 minutes, 45 seconds
  Loopback Mode : None
  4 link status changes since last clear
  Last clearing of "show interface" counters 20:22:38 ago
  5 seconds input rate 41.7 kbps (0.0% with framing overhead), 38 packets/sec
  5 seconds output rate 109 kbps (0.0% with framing overhead), 27 packets/sec
     245683 packets input, 34730075 bytes
     Received 166101 broadcasts, 60881 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     20659 packets output, 10792814 bytes
     Sent 15 broadcasts, 2442 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Vlan20 is up, line protocol is up (connected)
  Hardware is Vlan, address is 606b.5b2e.fe11 (bia 606b.5b2e.fe11)
  Internet address is 20.161.225.161/24
  Broadcast address is 255.255.255.255
  IPv6 link-local address is fe80::626b:5bff:fe2e:fe11/64
  IPv6 global unicast address(es):
    2001:20:161:225::161, subnet is 2001:20:161:225::/64
  IP MTU 1500 bytes (default)
  Up 20 hours, 18 minutes, 30 seconds
```

## show interfaces counters rates

```text
Port      Name      Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Et1                  0:05      0.0   0.0%        0      0.0   0.0%        0
Et2                  0:05      0.0   0.0%        0      0.0   0.0%        0
Et3                  0:05      0.0   0.0%        0      0.0   0.0%        0
Et4                  0:05      0.0   0.0%        0      0.0   0.0%        0
Et5                  0:05      0.0   0.0%        0      0.0   0.0%        0
Et6                  0:05      0.0   0.0%        0      0.0   0.0%        0
Et7                  0:05      0.0   0.0%        0      0.0   0.0%        0
Et8                  0:05      0.0   0.0%        0      0.0   0.0%        0
Et9                  0:05      0.0   0.0%        0      0.0   0.0%        0
Et10                 0:05     22.7   0.2%        2     17.5   0.2%        2
Et11                 0:05     16.0   0.2%        2     18.9   0.2%        2
Et12                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et13                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et14                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et15                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et16                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et17                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et18                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et19                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et20                 0:05     19.1   0.2%        2     15.5   0.2%        1
Et21                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et22                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et23                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et24                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et25                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et26                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et27                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et28                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et29                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et30                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et31                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et32                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et33                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et34                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et35                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et36                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et37                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et38                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et39                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et40                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et41/1               0:05      0.0   0.0%        0      0.0   0.0%        0
Et42/1               0:05      0.0   0.0%        0      0.0   0.0%        0
Et43/1               0:05      0.0   0.0%        0      0.0   0.0%        0
Et44/1               0:05      0.0   0.0%        0      0.0   0.0%        0
Et45/1               0:05      0.0   0.0%        0      0.0   0.0%        0
Et46/1               0:05      0.0   0.0%        0      0.0   0.0%        0
Ma1                  0:05      0.0   0.0%        0      0.1   0.0%        0
```

## show bgp neighbors 2002::353 vpn-ipv4 received-routes

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 10.0.0.11:1 IPv4 prefix 20.11.225.0/24
                                 2002::11              -       100     0       ? Or-ID: 10.0.0.11 C-LST: 100.0.0.53 
 * >      RD: 1:28 IPv4 prefix 20.28.225.0/24
                                 2002::28              0       100     0       ? Or-ID: 192.168.20.28 C-LST: 100.0.0.53 
 * >      RD: 1:29 IPv4 prefix 20.29.225.0/24
                                 2002::29              0       100     0       ? Or-ID: 192.168.20.29 C-LST: 100.0.0.53 
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
 * >      RD: 1:1162 IPv4 prefix 20.162.225.0/24
                                 2002::162             -       100     0       i Or-ID: 100.0.0.162 C-LST: 100.0.0.53 
 * >      RD: 1:199 IPv4 prefix 20.199.225.0/24
                                 2002::199             0       100     0       ? Or-ID: 20.49.199.199 C-LST: 100.0.0.53 
```

## show bgp neighbors 2002::353 vpn-ipv4 received-routes detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
BGP routing table entry for IPv4 prefix 20.11.225.0/24, Route Distinguisher: 10.0.0.11:1
 Paths: 1 available
  Local
    2002::11 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.0.11, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      Remote SRv6 SID: fcbb:0:1011:e000::/64, End.DT4 with NEXT-CSID
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
```

