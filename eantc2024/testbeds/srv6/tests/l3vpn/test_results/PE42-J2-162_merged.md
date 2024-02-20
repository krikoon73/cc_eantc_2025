# Test results for PE42-J2-162

## show version

```text
Arista DCS-7280SR3-40YC6-F
Hardware version: 11.02
Serial number: JPA2339P1QH
Hardware MAC address: 606b.5b2e.f3fd
System MAC address: 606b.5b2e.f3fd

Software image version: 4.31.0F-34472350.binoshmonsrv6ImgCDD43101 (engineering build)
Architecture: x86_64
Internal build version: 4.31.0F-34472350.binoshmonsrv6ImgCDD43101
Internal build ID: 6aa1c3ff-36f3-4f04-af26-9fc35d05e1eb
Image format version: 3.0
Image optimization: Default

Uptime: 2 hours and 11 minutes
Total memory: 8099732 kB
Free memory: 5020816 kB

```

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
Last table change time   : 0:06:33 ago
Number of table inserts  : 8
Number of table deletes  : 2
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
srv6      default  JNPR-302-MX204   L1   Ethernet10         P2P               UP    25          01                  
srv6      default  Cisco344-N57B1   L1   Ethernet20         P2P               UP    27          00                  
```

## show segment-routing ipv6 locator

```text
SRv6 configuration for VRF default
Administrative status: enabled
Operational status: enabled
Encapsulation source address: 2002::162
Number of configured locators: 1

Locator uSID-LOC-162
State: active
Type: micro-SID
Micro-SID domain: SRv6-uSID-162
Prefix: fcbb:0:1162::/48
IGP algorithm: SPF
Block length: 32
Function length: 16
Function allocator: micro-SID::SRv6-uSID-162
SID function value pools: default
```

## show segment-routing ipv6 locator std

```text
SRv6 configuration for VRF default
Administrative status: enabled
Operational status: enabled
Encapsulation source address: 2002::162
Number of configured locators: 1
```

## show segment-routing ipv6 sid function allocators

```text
SRv6 SID function allocators for VRF default

Allocator micro-SID::SRv6-uSID-162
Function length: 16
Locator users: uSID-LOC-162
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

B3  fcbb:0:1162:400::/64, End.DT4 with NEXT-CSID, locator uSID-LOC-162
    via IPv4 lookup, VRF VPNv4-uSID
B3  fcbb:0:1162:401::/64, End.DT6 with NEXT-CSID, locator uSID-LOC-162
    via IPv6 lookup, VRF VPNv4-uSID
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.162, local AS number 1
Neighbor Status Codes: m - Under maintenance
  Neighbor  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  2002::353 4 1                248        80    0    0 00:58:50 Estab   0      0
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.162, local AS number 1
```

## show tunnel fib

```text

Type 'SRv6 Transport', index 5, endpoint fcbb:0:1353::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 9, endpoint fcbb:0:28::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 11, endpoint fcbb:0:1029::/48, forwarding None
   via fe80::eaf:31ff:feca:1104, 'Ethernet20' SRv6, source 2002::162

Type 'SRv6 Transport', index 15, endpoint fcbb:0:1344::/48, forwarding None
   via fe80::eaf:31ff:feca:1104, 'Ethernet20' SRv6, source 2002::162

Type 'SRv6 Transport', index 17, endpoint fcbb:0:342::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 18, endpoint fcbb:0:352::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 23, endpoint fcbb:0:1199::/48, forwarding None
   via fe80::eaf:31ff:feca:1104, 'Ethernet20' SRv6, source 2002::162

Type 'SRv6 Transport', index 35, endpoint fcbb:0:336::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162

Type 'SRv6 Transport', index 38, endpoint fcbb:0:1338::/48, forwarding None
   via fe80::eaf:31ff:feca:1104, 'Ethernet20' SRv6, source 2002::162

Type 'SRv6 Transport', index 41, endpoint fcbb:0:161::/48, forwarding None
   via fe80::f24b:3aff:fe21:9e0f, 'Ethernet10' SRv6, source 2002::162
```

## show bgp neighbors 2002::353 vpn-ipv4 advertised-routes detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.162, local AS number 1
BGP routing table entry for IPv4 prefix 20.162.225.0/24, Route Distinguisher: 1:1162
 Paths: 1 available
  Local
    2002::162 from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1:20
      Local SRv6 SID (VRF SID): fcbb:0:1162:400::/64, End.DT4 with NEXT-CSID
```

## show bgp neighbors 2002::353 vpn-ipv6 advertised-routes detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.162, local AS number 1
BGP routing table entry for IPv6 prefix 2001:20:162:225::/64, Route Distinguisher: 1:1162
 Paths: 1 available
  Local
    2002::162 from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:1:20
      Local SRv6 SID (VRF SID): fcbb:0:1162:401::/64, End.DT6 with NEXT-CSID
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
                                 2002::161             -       100     0       i Or-ID: 100.0.0.161 C-LST: 100.0.0.53 
 * >      RD: 1:1162 IPv4 prefix 20.162.225.0/24
                                 -                     -       -       0       i
   %      RD: 1:199 IPv4 prefix 20.199.225.0/24
                                 2002::199             0       100     0       ? Or-ID: 20.49.199.199 C-LST: 100.0.0.53 
   %      RD: 1:419 IPv4 prefix 20.225.225.0/24
                                 2002::419             -       0       0       i Or-ID: 192.0.0.1 C-LST: 100.0.0.53 
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
                                 2002::161             -       100     0       i Or-ID: 100.0.0.161 C-LST: 100.0.0.53 
 * >      RD: 1:1162 IPv6 prefix 2001:20:162:225::/64
                                 -                     -       -       0       i
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
Codes: C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 I L1     2001:0:11:310::/64 [115/40]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:11:353::/64 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:19:344::/64 [115/30]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2001:0:20:36::/64 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:28:316::/64 [115/90]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:28:336::/64 [115/100]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:29:58::/64 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2001:0:36:58::/64 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:49:199::/64 [115/30]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2001:0:58:310::/64 [115/50]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:58:419::/64 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:59:161::/64 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:59:352::/64 [115/50]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:161:342::/64 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 C        2001:0:162:302::/64 [0/0]
           via Ethernet10, directly connected
 C        2001:0:162:344::/64 [0/0]
           via Ethernet20, directly connected
 I L1     2001:0:199:344::/64 [115/20]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2001:0:302:353::/64 [115/20]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:307:352::/64 [115/40]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:307:353::/64 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:316:342::/64 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:1:20:36::/64 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:1:28:36::/64 [115/90]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:1:29:38::/64 [115/50]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2001:1:38:49::/64 [115/40]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2001:1:59:352::/64 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::11/128 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::20/128 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::28/128 [115/90]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::29/128 [115/50]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2002::36/128 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::49/128 [115/40]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2002::58/128 [115/50]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::59/128 [115/50]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::161/128 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 C        2002::162/128 [0/0]
           via Loopback0, directly connected
 I L1     2002::199/128 [115/20]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2002::302/128 [115/10]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::307/128 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::310/128 [115/40]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::316/128 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::336/128 [115/90]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::338/128 [115/50]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2002::342/128 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::344/128 [115/20]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2002::352/128 [115/50]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::353/128 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::419/128 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002:0:29:338::/64 [115/60]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     fcbb:0:20::/48 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:28::/48 [115/90]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:36::/48 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:161::/48 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:307::/48 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:316::/48 [115/10]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:336::/48 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:342::/48 [115/71]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:352::/48 [115/41]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:419::/48 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:48a::/48 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1011::/48 [115/40]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1029::/48 [115/50]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     fcbb:0:1049::/48 [115/30]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     fcbb:0:1199::/48 [115/20]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     fcbb:0:1302::/48 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1310::/48 [115/40]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1338::/48 [115/40]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     fcbb:0:1344::/48 [115/11]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     fcbb:0:1353::/48 [115/21]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     ::/0 [115/20]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10

```

## show ip route vrf all

```text

VRF: default
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

 C        100.0.0.162/32 is directly connected, Loopback0


VRF: EVPNv4-T5-uSID
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

 B I      20.28.225.0/24 [200/0]
           via fcbb:0:28::/48, SRv6 Transport tunnel index 9, SRv6 SID fcbb:0:28:e102::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.29.225.0/24 [200/0]
           via fcbb:0:1029::/48, SRv6 Transport tunnel index 11, SRv6 SID fcbb:0:1029:e102::
              via fe80::eaf:31ff:feca:1104, Ethernet20
 B I      20.136.225.0/24 [200/0]
           via fcbb:0:336::/48, SRv6 Transport tunnel index 35, SRv6 SID fcbb:0:336:afff::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.138.225.0/24 [200/0]
           via fcbb:0:1338::/48, SRv6 Transport tunnel index 38, SRv6 SID fcbb:0:1338:b332::
              via fe80::eaf:31ff:feca:1104, Ethernet20
 B I      20.142.225.0/24 [200/0]
           via fcbb:0:342::/48, SRv6 Transport tunnel index 17, SRv6 SID fcbb:0:342:e002::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.144.225.0/24 [200/0]
           via fcbb:0:1344::/48, SRv6 Transport tunnel index 15, SRv6 SID fcbb:0:1344:e001::
              via fe80::eaf:31ff:feca:1104, Ethernet20
 B I      20.152.225.0/24 [200/0]
           via fcbb:0:352::/48, SRv6 Transport tunnel index 18, SRv6 SID fcbb:0:352:e002::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.153.225.0/24 [200/0]
           via fcbb:0:1353::/48, SRv6 Transport tunnel index 5, SRv6 SID fcbb:0:1353:e003::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.161.225.0/24 [200/0]
           via fcbb:0:161::/48, SRv6 Transport tunnel index 41, SRv6 SID fcbb:0:161:400::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 C        20.162.225.0/24 [0/0]
           via Vlan20, directly connected


VRF: mgmt
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

Gateway of last resort:
 S        0.0.0.0/0 [1/0] via 192.168.20.1, Management1

 C        192.168.20.0/23 is directly connected, Management1

```

## show ipv6 route vrf all

```text

VRF: default
Displaying 70 of 75 IPv6 routing table entries
Codes: C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 I L1     2001:0:11:310::/64 [115/40]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:11:353::/64 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:19:344::/64 [115/30]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2001:0:20:36::/64 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:28:316::/64 [115/90]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:28:336::/64 [115/100]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:29:58::/64 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2001:0:36:58::/64 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:49:199::/64 [115/30]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2001:0:58:310::/64 [115/50]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:58:419::/64 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:59:161::/64 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:59:352::/64 [115/50]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:161:342::/64 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 C        2001:0:162:302::/64 [0/0]
           via Ethernet10, directly connected
 C        2001:0:162:344::/64 [0/0]
           via Ethernet20, directly connected
 I L1     2001:0:199:344::/64 [115/20]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2001:0:302:353::/64 [115/20]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:307:352::/64 [115/40]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:307:353::/64 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:316:342::/64 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:1:20:36::/64 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:1:28:36::/64 [115/90]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:1:29:38::/64 [115/50]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2001:1:38:49::/64 [115/40]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2001:1:59:352::/64 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::11/128 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::20/128 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::28/128 [115/90]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::29/128 [115/50]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2002::36/128 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::49/128 [115/40]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2002::58/128 [115/50]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::59/128 [115/50]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::161/128 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 C        2002::162/128 [0/0]
           via Loopback0, directly connected
 I L1     2002::199/128 [115/20]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2002::302/128 [115/10]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::307/128 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::310/128 [115/40]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::316/128 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::336/128 [115/90]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::338/128 [115/50]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2002::342/128 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::344/128 [115/20]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     2002::352/128 [115/50]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::353/128 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::419/128 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002:0:29:338::/64 [115/60]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     fcbb:0:20::/48 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:28::/48 [115/90]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:36::/48 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:161::/48 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:307::/48 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:316::/48 [115/10]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:336::/48 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:342::/48 [115/71]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:352::/48 [115/41]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:419::/48 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:48a::/48 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1011::/48 [115/40]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1029::/48 [115/50]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     fcbb:0:1049::/48 [115/30]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     fcbb:0:1199::/48 [115/20]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     fcbb:0:1302::/48 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1310::/48 [115/40]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1338::/48 [115/40]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     fcbb:0:1344::/48 [115/11]
           via fe80::eaf:31ff:feca:1104, Ethernet20
 I L1     fcbb:0:1353::/48 [115/21]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     ::/0 [115/20]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10


VRF: EVPNv4-T5-uSID
Displaying 0 of 3 IPv6 routing table entries
Codes: C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route



VRF: VPNv4-uSID
Displaying 7 of 11 IPv6 routing table entries
Codes: C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 B I      2001:20:28:225::/64 [200/0]
           via fcbb:0:28::/48, SRv6 Transport tunnel index 9, SRv6 SID fcbb:0:28:e103::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:29:225::/64 [200/0]
           via fcbb:0:1029::/48, SRv6 Transport tunnel index 11, SRv6 SID fcbb:0:1029:e103::
              via fe80::eaf:31ff:feca:1104, Ethernet20
 B I      2001:20:161:225::/64 [200/0]
           via fcbb:0:161::/48, SRv6 Transport tunnel index 41, SRv6 SID fcbb:0:161:401::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 C        2001:20:162:225::/64 [0/0]
           via Vlan20, directly connected
 B I      2001:20:199:225::/64 [200/0]
           via fcbb:0:1199::/48, SRv6 Transport tunnel index 23, SRv6 SID fcbb:0:1199:e000:0:1:0:22
              via fe80::eaf:31ff:feca:1104, Ethernet20
 B I      2001:20:336:225::/64 [200/0]
           via fcbb:0:336::/48, SRv6 Transport tunnel index 35, SRv6 SID fcbb:0:336:b000::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      2001:20:338:225::/64 [200/0]
           via fcbb:0:1338::/48, SRv6 Transport tunnel index 38, SRv6 SID fcbb:0:1338:b333::
              via fe80::eaf:31ff:feca:1104, Ethernet20


VRF: mgmt
Displaying 0 of 3 IPv6 routing table entries
Codes: C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route


! IPv6 routing not enabled
```

