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

Uptime: 49 minutes
Total memory: 8099732 kB
Free memory: 5218600 kB

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
Last table change time   : 0:44:52 ago
Number of table inserts  : 7
Number of table deletes  : 0
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
srv6      default  Nokia-59-IXRe2   L2   Ethernet20         P2P               UP    22          00                  
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
  2002::353 4 1                158        65    0    0 00:39:01 Estab   0      0
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
```

## show tunnel fib

```text

Type 'SRv6 Transport', index 25, endpoint fcbb:0:1162::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 27, endpoint fcbb:0:1344::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 28, endpoint fcbb:0:352::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 29, endpoint fcbb:0:342::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 30, endpoint fcbb:0:1353::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 31, endpoint fcbb:0:1029::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 34, endpoint fcbb:0:28::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 35, endpoint fcbb:0:1338::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 36, endpoint fcbb:0:1199::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 37, endpoint fcbb:0:336::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161
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
   %      RD: 1:20 IPv4 prefix 20.20.225.0/24
                                 2002::20              0       100     0       ? Or-ID: 10.0.0.20 C-LST: 100.0.0.53 
 * >      RD: 1:28 IPv4 prefix 20.28.225.0/24
                                 2002::28              0       100     0       ? Or-ID: 192.168.20.28 C-LST: 100.0.0.53 
 * >      RD: 1:29 IPv4 prefix 20.29.225.0/24
                                 2002::29              0       100     0       ? Or-ID: 192.168.20.29 C-LST: 100.0.0.53 
   %      RD: 1:36 IPv4 prefix 20.36.225.0/24
                                 2002::36              0       100     0       ? Or-ID: 192.168.20.36 C-LST: 100.0.0.53 
   %      RD: 1:49 IPv4 prefix 20.49.225.0/24
                                 2002::49              0       100     0       ? Or-ID: 10.0.0.49 C-LST: 100.0.0.53 
   %      RD: 1:302 IPv4 prefix 20.102.225.0/24
                                 2002::302             -       100     0       i Or-ID: 10.0.1.2 C-LST: 100.0.0.53 
   %      RD: 1:307 IPv4 prefix 20.107.225.0/24
                                 2002::307             -       100     0       i Or-ID: 10.0.1.7 C-LST: 100.0.0.53 
   %      RD: 1:310 IPv4 prefix 20.110.225.0/24
                                 2002::310             -       100     0       i Or-ID: 10.0.1.10 C-LST: 100.0.0.53 
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
   %      RD: 1:199 IPv4 prefix 20.199.225.0/24
                                 2002::199             0       100     0       ? Or-ID: 20.49.199.199 C-LST: 100.0.0.53 
   %      RD: 1:419 IPv4 prefix 20.225.225.0/24
                                 2002::419             -       0       0       i Or-ID: 192.0.0.1 C-LST: 100.0.0.53 
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
   %      RD: 1:419 IPv6 prefix 2001:0:419:419::/64
                                 2002::419             -       0       0       i Or-ID: 192.0.0.1 C-LST: 100.0.0.53 
   %      RD: 1:20 IPv6 prefix 2001:20:20:225::/64
                                 2002::20              0       100     0       ? Or-ID: 10.0.0.20 C-LST: 100.0.0.53 
 * >      RD: 1:28 IPv6 prefix 2001:20:28:225::/64
                                 2002::28              0       100     0       ? Or-ID: 192.168.20.28 C-LST: 100.0.0.53 
 * >      RD: 1:29 IPv6 prefix 2001:20:29:225::/64
                                 2002::29              0       100     0       ? Or-ID: 192.168.20.29 C-LST: 100.0.0.53 
   %      RD: 1:36 IPv6 prefix 2001:20:36:225::/64
                                 2002::36              0       100     0       ? Or-ID: 192.168.20.36 C-LST: 100.0.0.53 
   %      RD: 1:49 IPv6 prefix 2001:20:49:225::/64
                                 2002::49              0       100     0       ? Or-ID: 10.0.0.49 C-LST: 100.0.0.53 
   %      RD: 1:302 IPv6 prefix 2001:20:102:225::/64
                                 2002::302             -       100     0       i Or-ID: 10.0.1.2 C-LST: 100.0.0.53 
   %      RD: 1:307 IPv6 prefix 2001:20:107:225::/64
                                 2002::307             -       100     0       i Or-ID: 10.0.1.7 C-LST: 100.0.0.53 
   %      RD: 1:310 IPv6 prefix 2001:20:110:225::/64
                                 2002::310             -       100     0       i Or-ID: 10.0.1.10 C-LST: 100.0.0.53 
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
Displaying 69 of 74 IPv6 routing table entries
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
 I L2     fcbb:0:307::/48 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:316::/48 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:336::/48 [115/40]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:342::/48 [115/11]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:352::/48 [115/21]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:419::/48 [115/80]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:48a::/48 [115/90]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1011::/48 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1029::/48 [115/80]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1049::/48 [115/90]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1162::/48 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1199::/48 [115/80]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1302::/48 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
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

 B I      20.28.225.0/24 [200/0]
           via fcbb:0:28::/48, SRv6 Transport tunnel index 34, SRv6 SID fcbb:0:28:e102::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.29.225.0/24 [200/0]
           via fcbb:0:1029::/48, SRv6 Transport tunnel index 31, SRv6 SID fcbb:0:1029:e102::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.136.225.0/24 [200/0]
           via fcbb:0:336::/48, SRv6 Transport tunnel index 37, SRv6 SID fcbb:0:336:e664::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.138.225.0/24 [200/0]
           via fcbb:0:1338::/48, SRv6 Transport tunnel index 35, SRv6 SID fcbb:0:1338:e666::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.142.225.0/24 [200/0]
           via fcbb:0:342::/48, SRv6 Transport tunnel index 29, SRv6 SID fcbb:0:342:e002::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.144.225.0/24 [200/0]
           via fcbb:0:1344::/48, SRv6 Transport tunnel index 27, SRv6 SID fcbb:0:1344:e001::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.152.225.0/24 [200/0]
           via fcbb:0:352::/48, SRv6 Transport tunnel index 28, SRv6 SID fcbb:0:352:e002::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.153.225.0/24 [200/0]
           via fcbb:0:1353::/48, SRv6 Transport tunnel index 30, SRv6 SID fcbb:0:1353:e003::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        20.161.225.0/24 [0/0]
           via Vlan20, directly connected
 B I      20.162.225.0/24 [200/0]
           via fcbb:0:1162::/48, SRv6 Transport tunnel index 25, SRv6 SID fcbb:0:1162:400::
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
Displaying 69 of 74 IPv6 routing table entries
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
 I L2     fcbb:0:307::/48 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:316::/48 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:336::/48 [115/40]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:342::/48 [115/11]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:352::/48 [115/21]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:419::/48 [115/80]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:48a::/48 [115/90]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1011::/48 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1029::/48 [115/80]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1049::/48 [115/90]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1162::/48 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1199::/48 [115/80]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1302::/48 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
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
Displaying 7 of 11 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 B I      2001:20:28:225::/64 [200/0]
           via fcbb:0:28::/48, SRv6 Transport tunnel index 34, SRv6 SID fcbb:0:28:e103::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:29:225::/64 [200/0]
           via fcbb:0:1029::/48, SRv6 Transport tunnel index 31, SRv6 SID fcbb:0:1029:e103::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 C        2001:20:161:225::/64 [0/0]
           via Vlan20, directly connected
 B I      2001:20:162:225::/64 [200/0]
           via fcbb:0:1162::/48, SRv6 Transport tunnel index 25, SRv6 SID fcbb:0:1162:401::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:199:225::/64 [200/0]
           via fcbb:0:1199::/48, SRv6 Transport tunnel index 36, SRv6 SID fcbb:0:1199:e000:0:1:0:22
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:336:225::/64 [200/0]
           via fcbb:0:336::/48, SRv6 Transport tunnel index 37, SRv6 SID fcbb:0:336:e665::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:338:225::/64 [200/0]
           via fcbb:0:1338::/48, SRv6 Transport tunnel index 35, SRv6 SID fcbb:0:1338:e667::
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
    CIEN-11-5169.00-00          225   4869  1166   1077 L2  0000.0000.0011.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: CIEN-11-5169
      Area addresses: 49.0001
      Interface address: 2001:0:11:310::11
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:11:310::310
        Global IPv6 Interface Address: 2001:0:11:310::11
        Adj-sid: 24001 flags: [L V F] weight: 0x0
      IS Neighbor          : Cisco353-8201-24H8FH.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:11:353::353
        Global IPv6 Interface Address: 2001:0:11:353::11
        Adj-sid: 24000 flags: [L V F] weight: 0x0
      Reachability         : 10.0.0.11/32 Metric: 0 Type: 1 Up
      Reachability          : 2002::11/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:1011::/48 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:11:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:19:344::/64 Metric: 60 Type: 1 Up
      Reachability          : 2001:0:29:58::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 60 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 30 Type: 1 Up
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
      Reachability          : 2002::302/128 Metric: 20 Type: 1 Up
      Reachability          : 2002::310/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::338/128 Metric: 50 Type: 1 Up
      Reachability          : 2002::344/128 Metric: 50 Type: 1 Up
      Reachability          : 2002::353/128 Metric: 20 Type: 1 Up
      Reachability          : 2002::419/128 Metric: 40 Type: 1 Up
      Reachability          : 2002:0:29:338::/64 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:316::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:419::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:48a::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1162::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1199::/48 Metric: 50 Type: 1 Up
      Reachability          : fcbb:0:1310::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1344::/48 Metric: 41 Type: 1 Up
      Reachability          : fcbb:0:1353::/48 Metric: 11 Type: 1 Up
      Reachability          : 2002::199/128 Metric: 50 Type: 1 Up
      Reachability          : fcbb:0:1029::/48 Metric: 30 Type: 1 Up
      Reachability          : fcbb:0:1338::/48 Metric: 40 Type: 1 Up
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
    h3c_20_CR16010E-F.00-00       455  15099   810    863 L2  0000.0000.0020.00-00  <>
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
        SRv6 SID Un Supported
          SID : fcbb:0:20::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 0
        SRv6 SID Un Supported
          SID : fcbb:0:20:e100::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:20:e101::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID Un Supported
          SID : fcbb:0:20:e102::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID Un Supported
          SID : fcbb:0:20:e103::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End
          SID : fcbb:0:20:e104::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP USP USD
          SID : fcbb:0:20:e105::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
    h3c_28_S12500R-2L.00-00       136  18723   858    428 L2  0000.0000.0028.00-00  <>
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
    huawei_36.00-00             302  47600   756    781 L2  0000.0000.0036.00-00  <>
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
      Reachability          : 2001:0:36:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::36/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:36::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:36::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID Un Supported
          SID : fcbb:0:36::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
        SRv6 SID Un Supported
          SID : fcbb:0:36:e141::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 64
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:36:e142::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 64
        SRv6 SID End
          SID : fcbb:0:36:e143::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP
          SID : fcbb:0:36:e144::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP USP USD
          SID : fcbb:0:36:e145::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
    anet-161-R3.00-00           326  33648   611    250 L2  0000.0000.0161.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 311 s
      NLPID: 0x8E(IPv6)
      Hostname: anet-161-R3
      Area addresses: 49.0000
      Interface address: 2001:0:59:161::161
      Interface address: 2001:0:161:342::161
      Interface address: 2002::161
      IS Neighbor          : Cisco342-9902.00    Metric: 10
      IS Neighbor          : Nokia-59-IXRe2.00   Metric: 10
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
    JNPR-307-ACX7024.00-00        46  57609   392    343 L2  0000.0000.0307.00-00  <>
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
      Reachability          : 2001:0:307:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::307/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:307:352::/64 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:307::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:307::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
      Router Capabilities: Router Id: 10.0.1.7 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    JNPR-310-ACX7100-48L.00-00       436  28842  1067   1283 L2  0000.0000.0310.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: JNPR-310-ACX7100-48L
      Area addresses: 49.0001
      Interface address: 10.0.1.10
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::58
        Global IPv6 Interface Address: 2001:0:58:310::310
      Reachability          : 2001:0:58:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::310/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:29:58::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 20 Type: 1 Up
      Reachability          : 2002::58/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::29/128 Metric: 20 Type: 1 Up
      Reachability          : 2002:0:29:338::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:1:29:38::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:1:38:49::/64 Metric: 40 Type: 1 Up
      Reachability          : 2002::338/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::419/128 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:19:344::/64 Metric: 60 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 50 Type: 1 Up
      Reachability          : 2002::49/128 Metric: 50 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 10 Type: 1 Up
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
      Reachability          : 2002::199/128 Metric: 50 Type: 1 Up
      Reachability          : fcbb:0:1310::/48 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:1029::/48 Metric: 20 Type: 1 Down
      Reachability          : fcbb:0:1338::/48 Metric: 30 Type: 1 Down
      SRv6 Locator: fcbb:0:1310::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:316::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:0:316::
      SRv6 Locator: fcbb:0:419::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:419:11::
      SRv6 Locator: fcbb:0:1011::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1011::
      SRv6 Locator: fcbb:0:1049::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1049::
      SRv6 Locator: fcbb:0:1162::/48 Topology: 0
        Metric: 50 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1162::
      SRv6 Locator: fcbb:0:1199::/48 Topology: 0
        Metric: 50 Algorithm: 0 Flags: []
        SRv6 SID Un Supported
          SID : fcbb:0:1199::
        SRv6 SID Un Supported
          SID : fcbb:0:1199:e13f::
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1199:e140::
        SRv6 SID End
          SID : fcbb:0:1199:e141::
        SRv6 SID End with PSP
          SID : fcbb:0:1199:e142::
        SRv6 SID End with PSP USP USD
          SID : fcbb:0:1199:e143::
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
      Router Capabilities: Router Id: 10.0.1.10 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    JNPR-310-ACX7100-48L.00-01       129  57274  1067    263 L2  0000.0000.0310.00-01  <>
      IS Neighbor          : CIEN-11-5169.00     Metric: 10
        IPv6 Neighbor Address: 2001:0:11:310::11
        Global IPv6 Interface Address: 2001:0:11:310::310
      Reachability          : fcbb:0:316::/48 Metric: 30 Type: 1 Down
      Reachability          : fcbb:0:419::/48 Metric: 20 Type: 1 Down
      Reachability          : fcbb:0:1011::/48 Metric: 10 Type: 1 Down
      Reachability          : fcbb:0:1049::/48 Metric: 40 Type: 1 Down
      Reachability          : fcbb:0:1162::/48 Metric: 50 Type: 1 Down
      Reachability          : fcbb:0:1199::/48 Metric: 50 Type: 1 Down
      Reachability          : fcbb:0:1344::/48 Metric: 51 Type: 1 Down
      Reachability          : fcbb:0:1353::/48 Metric: 21 Type: 1 Down
      SRv6 Locator: fcbb:0:1338::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:0:1338::
    JNPR-316-MX304.00-00        123  65357  1132    369 L2  0000.0000.0316.00-00  <>
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
      Reachability          : 2002::316/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:1302::/48 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:28:316::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:316:342::/64 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:1302::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:0:1302::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.1.16 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    ZTE_336_ZXR10_M6000-8SE.00-00       355  56422   699    474 L2  0000.0000.0336.00-00  <>
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
    Cisco342-9902.00-00         130  28838  1135    417 L2  0000.0000.0342.00-00  <>
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
    Cisco352-N540.00-00         297  19006  1145    435 L2  0000.0000.0352.00-00  <>
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
    Cisco353-8201-24H8FH.00-00       426   3218  1088   1323 L2  0000.0000.0353.00-00  <>
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
      Reachability          : 2001:0:162:302::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:162:344::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:302:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:307:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::11/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::162/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::302/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::310/128 Metric: 20 Type: 1 Up
      Reachability          : 2002::353/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:316::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1353::/48 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:29:58::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 40 Type: 1 Up
      Reachability          : 2002::29/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::58/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::419/128 Metric: 50 Type: 1 Up
      Reachability          : 2002:0:29:338::/64 Metric: 50 Type: 1 Up
      Reachability          : fcbb:0:419::/48 Metric: 50 Type: 1 Up
      Reachability          : fcbb:0:1011::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:1162::/48 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:19:344::/64 Metric: 50 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 50 Type: 1 Up
      Reachability          : 2001:0:199:344::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:1:29:38::/64 Metric: 60 Type: 1 Up
      Reachability          : 2001:1:38:49::/64 Metric: 60 Type: 1 Up
      Reachability          : 2002::49/128 Metric: 60 Type: 1 Up
      Reachability          : 2002::338/128 Metric: 60 Type: 1 Up
      Reachability          : 2002::344/128 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1049::/48 Metric: 50 Type: 1 Up
      Reachability          : fcbb:0:1199::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1310::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:1338::/48 Metric: 50 Type: 1 Up
      Reachability          : fcbb:0:1344::/48 Metric: 31 Type: 1 Up
      Reachability          : 2002::199/128 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1029::/48 Metric: 40 Type: 1 Up
      SRv6 Locator: fcbb:0:316::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:419::/48 Topology: 0
        Metric: 50 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1011::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1029::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1049::/48 Topology: 0
        Metric: 50 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1162::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1199::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
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
    Nokia_58-SR1-3-SRv6.00-00       408  22551 64227    180 L2  0100.0000.0058.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia_58-SR1-3-SRv6
      Area addresses:
        49.0000.0000.0058.00
        49.0001
      Reachability          : fcbb:0:1029::/48 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:1029::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1029::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 0
      Router Capabilities: Router Id: 10.0.0.58 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0
    Nokia_58-SR1-3-SRv6.00-01       177  51049 64597   1387 L2  0100.0000.0058.00-01  <>
      Interface address: 10.0.0.58
      Interface address: 2001:0:36:58::58
      Interface address: 2001:0:58:310::58
      Interface address: 2001:0:58:419::58
      Interface address: 2002::58
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::310
        Global IPv6 Interface Address: 2001:0:58:310::58
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:36:58::36
        Global IPv6 Interface Address: 2001:0:36:58::58
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
      Reachability          : fcbb:0:316::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:419::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1011::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:1049::/48 Metric: 30 Type: 1 Up
      Reachability          : fcbb:0:1162::/48 Metric: 60 Type: 1 Up
      Reachability          : fcbb:0:1199::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1310::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1338::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:1344::/48 Metric: 51 Type: 1 Up
      Reachability          : fcbb:0:1353::/48 Metric: 31 Type: 1 Up
      SRv6 Locator: fcbb:0:316::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:0:316::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
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
      SRv6 Locator: fcbb:0:1049::/48 Topology: 0
        Metric: 30 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1049::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:0:1162::/48 Topology: 0
        Metric: 60 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1162::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:0:1199::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
        SRv6 SID Un Supported
          SID : fcbb:0:1199::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
        SRv6 SID Un Supported
          SID : fcbb:0:1199:e13f::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 64
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1199:e140::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 64
        SRv6 SID End
          SID : fcbb:0:1199:e141::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP
          SID : fcbb:0:1199:e142::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP USP USD
          SID : fcbb:0:1199:e143::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
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
        Metric: 31 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1353::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
    Nokia-59-IXRe2.00-00         71  54395  1177    310 L2  0100.0000.0059.00-00  <>
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
      Router Capabilities: Router Id: 10.0.0.59 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0
    Keys-Ixia-419.00-00          24  49255   630    351 L2  3800.0000.0419.00-00  <DefaultAtt>
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
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:316::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:316::/48
System ID: Cisco353-8201-24H8FH
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
System ID: JNPR-316-MX304
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Up 44 minutes, 56 seconds
  Loopback Mode : None
  2 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
  5 seconds input rate 3 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 498 bps (0.0% with framing overhead), 1 packets/sec
     90 packets input, 18270 bytes
     Received 0 broadcasts, 90 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     1413 packets output, 185902 bytes
     Sent 0 broadcasts, 1413 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet6 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe17 (bia 606b.5b2e.fe17)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Up 44 minutes, 58 seconds
  Loopback Mode : None
  2 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
  5 seconds input rate 243 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 502 bps (0.0% with framing overhead), 0 packets/sec
     510740 packets input, 521800896 bytes
     Received 0 broadcasts, 568 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     257555 packets output, 264803071 bytes
     Sent 0 broadcasts, 801 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet11 is up, line protocol is up (connected)
  Hardware is Ethernet, address is 606b.5b2e.fe1c (bia 606b.5b2e.fe1c)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 10000000 kbit
  Full-duplex, 10Gb/s, auto negotiation: off, uni-link: disabled
  Up 44 minutes, 58 seconds
  Loopback Mode : None
  2 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
  5 seconds input rate 192 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 495 bps (0.0% with framing overhead), 1 packets/sec
     551482 packets input, 436050278 bytes
     Received 1 broadcasts, 116 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     446026 packets output, 438499062 bytes
     Sent 0 broadcasts, 1430 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet12 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe1d (bia 606b.5b2e.fe1d)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Up 44 minutes, 58 seconds
  Loopback Mode : None
  2 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
  5 seconds input rate 321 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 668 bps (0.0% with framing overhead), 1 packets/sec
     308375 packets input, 317100954 bytes
     Received 0 broadcasts, 830 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     310234 packets output, 318892876 bytes
     Sent 0 broadcasts, 801 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet21 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe26 (bia 606b.5b2e.fe26)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 25000000 kbit
  Full-duplex, 25Gb/s, auto negotiation: off, uni-link: disabled
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Up 44 minutes, 56 seconds
  Loopback Mode : None
  2 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
  5 seconds input rate 496 bps (0.0% with framing overhead), 1 packets/sec
  5 seconds output rate 6 bps (0.0% with framing overhead), 0 packets/sec
     1438 packets input, 188934 bytes
     Received 0 broadcasts, 1438 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     98 packets output, 24248 bytes
     Sent 0 broadcasts, 98 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet40 is up, line protocol is up (connected)
  Hardware is Ethernet, address is 606b.5b2e.fe39 (bia 606b.5b2e.fe39)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 10000000 kbit
  Full-duplex, 10Gb/s, auto negotiation: off, uni-link: disabled
  Up 44 minutes, 56 seconds
  Loopback Mode : None
  2 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
  5 seconds input rate 496 bps (0.0% with framing overhead), 1 packets/sec
  5 seconds output rate 6 bps (0.0% with framing overhead), 0 packets/sec
     1439 packets input, 189057 bytes
     Received 0 broadcasts, 1439 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     93 packets output, 23633 bytes
     Sent 0 broadcasts, 93 multicast
     0 output errors, 0 collisions
     0 late collision, 0 deferred, 0 output discards
     0 PAUSE output
Ethernet41/1 is down, line protocol is notpresent (notconnect)
  Hardware is Ethernet, address is 606b.5b2e.fe3a (bia 606b.5b2e.fe3a)
  Ethernet MTU 10218 bytes, Ethernet MRU 10240 bytes, BW 100000000 kbit
  Full-duplex, 100Gb/s, auto negotiation: off, uni-link: disabled
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Down 45 minutes, 18 seconds
  Loopback Mode : None
  1 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
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
  Up 46 minutes, 20 seconds
Management1 is up, line protocol is up (connected)
  Hardware is Ethernet, address is 606b.5b2e.fe10 (bia 606b.5b2e.fe10)
  Internet address is 192.168.20.161/23
  Broadcast address is 255.255.255.255
  IP MTU 1500 bytes (default), BW 1000000 kbit
  Full-duplex, 1Gb/s, auto negotiation: on, uni-link: n/a
  Up 46 minutes, 13 seconds
  Loopback Mode : None
  4 link status changes since last clear
  Last clearing of "show interface" counters 0:49:07 ago
  5 seconds input rate 43.6 kbps (0.0% with framing overhead), 39 packets/sec
  5 seconds output rate 113 kbps (0.0% with framing overhead), 27 packets/sec
     13382 packets input, 1818330 bytes
     Received 6837 broadcasts, 2483 multicast
     0 runts, 0 giants
     0 input errors, 0 CRC, 0 alignment, 0 symbol, 0 input discards
     0 PAUSE input
     3640 packets output, 1540347 bytes
     Sent 7 broadcasts, 95 multicast
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
  Up 44 minutes, 58 seconds
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
Et10                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et11                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et12                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et13                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et14                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et15                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et16                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et17                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et18                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et19                 0:05      0.0   0.0%        0      0.0   0.0%        0
Et20                 0:05      0.0   0.0%        0      0.0   0.0%        0
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

