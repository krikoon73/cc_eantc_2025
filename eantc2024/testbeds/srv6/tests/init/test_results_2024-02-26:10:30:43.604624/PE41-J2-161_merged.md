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

Uptime: 3 hours and 33 minutes
Total memory: 8099732 kB
Free memory: 5245556 kB

```

## show interfaces status

```text
Port       Name   Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1               notconnect   routed   full   25G    Not Present                    
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
Et39              notconnect   1        full   10G    10GBASE-SRL                    
Et40              notconnect   1        full   10G    10GBASE-SRL                    
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
Last table change time   : 3:09:59 ago
Number of table inserts  : 5
Number of table deletes  : 0
Number of table drops    : 0
Number of table age-outs : 0

Port          Neighbor Device ID               Neighbor Port ID    TTL
---------- -------------------------------- ---------------------- ---
Et5           Harness3-J-175.ns.eantc.de       Ethernet3           120
Et10          Cisco342-9902                    TenGigE0/0/0/12     120
Et11          JNPR-398-QFX5120                 546                 120
Et20          Nokia-59-IXRe2                   1610899777          121
Ma1           extreme-x460-1                   42                  120

```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
srv6      default  Cisco342-9902    L2   Ethernet10         P2P               UP    23          00                  
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
  2002::353 4 1                762       230    0    0 03:09:38 Estab   163    9
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
BGP routing table entry for ip-prefix 20.136.225.0/24, Route Distinguisher: 1:336
 Paths: 1 available
  Local
    2002::336 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.1.36, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      SRv6 SID: fcbb:0:336:e663::/64, End.DT4
BGP routing table entry for ip-prefix 20.138.225.0/24, Route Distinguisher: 1:338
 Paths: 1 available
  Local
    2002::338 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.1.38, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:20
      SRv6 SID: fcbb:0:1338:e663::/64, End.DT4 with NEXT-CSID
BGP routing table entry for ip-prefix 21.136.225.0/24, Route Distinguisher: 21:336
 Paths: 1 available
  Local
    2002::336 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, invalid, internal
      Originator: 10.0.1.36, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:21
      SRv6 SID: fcbb:1:336:e663::/64, End.DT4
BGP routing table entry for ip-prefix 21.138.225.0/24, Route Distinguisher: 21:338
 Paths: 1 available
  Local
    2002::338 from 2002::353 (100.0.0.53)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.1.38, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:21
      SRv6 SID: fcbb:1:1338:e666::/64, End.DT4 with NEXT-CSID
BGP routing table entry for ip-prefix 23.58.225.0/24, Route Distinguisher: 10.0.0.58:23
 Paths: 1 available
  Local
    2002::58 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, internal
      Originator: 10.0.0.58, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:23
BGP routing table entry for ip-prefix 23.59.225.0/24, Route Distinguisher: 10.0.0.59:23
 Paths: 1 available
  Local
    2002::59 from 2002::353 (100.0.0.53)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, invalid, internal
      Originator: 10.0.0.59, Cluster list: 100.0.0.53 
      Extended Community: Route-Target-AS:1:23
```

## show tunnel fib

```text

Type 'SRv6 Transport', index 1, endpoint fcbb:0:336::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 2, endpoint fcbb:1:1000::/36, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 3, endpoint fcbb:0:1000::/36, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 4, endpoint fcbb:0:1310::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 7, endpoint fcbb:0:59::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 8, endpoint fcbb:0:307::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 9, endpoint fcbb:0:28::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 10, endpoint fcbb:0:1353::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 11, endpoint fcbb:0:36::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 13, endpoint fcbb:0:316::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 21, endpoint fcbb:0:352::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 22, endpoint fcbb:0:342::/48, forwarding None
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
 * >      RD: 1011:1 IPv4 prefix 20.11.225.0/24
                                 2002::11              -       100     0       ? Or-ID: 10.0.0.11 C-LST: 100.0.0.53 
 * >      RD: 1:28 IPv4 prefix 20.28.225.0/24
                                 2002::28              0       100     0       ? Or-ID: 10.0.0.28 C-LST: 100.0.0.53 
 * >      RD: 1:29 IPv4 prefix 20.29.225.0/24
                                 2002::29              0       100     0       ? Or-ID: 10.0.0.29 C-LST: 100.0.0.53 
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
 * >      RD: 1:199 IPv4 prefix 20.199.225.0/24
                                 2002::199             0       100     0       ? Or-ID: 20.49.199.199 C-LST: 100.0.0.53 
 * >      RD: 21:1011 IPv4 prefix 21.11.225.0/24
                                 2002::11              -       100     0       ? Or-ID: 10.0.0.11 C-LST: 100.0.0.53 
          RD: 1:21 IPv4 prefix 21.28.225.0/24
                                 2002::28              0       100     0       ? Or-ID: 10.0.0.28 C-LST: 100.0.0.53 
 * >      RD: 1:21 IPv4 prefix 21.29.225.0/24
                                 2002::29              0       100     0       ? Or-ID: 10.0.0.29 C-LST: 100.0.0.53 
          RD: 1:21 IPv4 prefix 21.36.225.0/24
                                 2002::36              0       100     0       ? Or-ID: 192.168.20.36 C-LST: 100.0.0.53 
 * >      RD: 21:58 IPv4 prefix 21.58.225.0/24
                                 2002::58              -       100     0       i Or-ID: 10.0.0.58 C-LST: 100.0.0.53 
   %      RD: 21:59 IPv4 prefix 21.59.225.0/24
                                 2002::59              -       100     0       i Or-ID: 10.0.0.59 C-LST: 100.0.0.53 
 * >      RD: 21:302 IPv4 prefix 21.102.225.0/24
                                 2002::302             -       100     0       i Or-ID: 10.0.1.2 C-LST: 100.0.0.53 
          RD: 21:307 IPv4 prefix 21.107.225.0/24
                                 2002::307             -       100     0       i Or-ID: 10.0.1.7 C-LST: 100.0.0.53 
 * >      RD: 21:310 IPv4 prefix 21.110.225.0/24
                                 2002::310             -       100     0       i Or-ID: 10.0.1.10 C-LST: 100.0.0.53 
          RD: 21:316 IPv4 prefix 21.116.225.0/24
                                 2002::316             -       100     0       i Or-ID: 10.0.1.16 C-LST: 100.0.0.53 
          RD: 21:352 IPv4 prefix 21.142.225.0/24
                                 2002::342             0       100     0       ? Or-ID: 100.0.0.42 C-LST: 100.0.0.53 
 * >      RD: 21:352 IPv4 prefix 21.144.225.0/24
                                 2002::344             0       100     0       ? Or-ID: 100.0.0.44 C-LST: 100.0.0.53 
          RD: 21:352 IPv4 prefix 21.152.225.0/24
                                 2002::352             0       100     0       ? Or-ID: 100.0.0.52 C-LST: 100.0.0.53 
 * >      RD: 21:352 IPv4 prefix 21.153.225.0/24
                                 2002::353             0       100     0       ?
 * >      RD: 2:199 IPv4 prefix 21.199.225.0/24
                                 2002::199             0       100     0       ? Or-ID: 20.49.199.199 C-LST: 100.0.0.53 
          RD: 100:1 IPv4 prefix 192.168.11.0/24
                                 2002::199             0       100     0       ? Or-ID: 20.49.199.199 C-LST: 100.0.0.53 
          RD: 100:2 IPv4 prefix 192.168.21.0/24
                                 2002::36              0       100     0       ? Or-ID: 192.168.20.36 C-LST: 100.0.0.53 
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
 * >      RD: 1:28 IPv6 prefix 2001:20:28:225::/64
                                 2002::28              0       100     0       ? Or-ID: 10.0.0.28 C-LST: 100.0.0.53 
 * >      RD: 1:29 IPv6 prefix 2001:20:29:225::/64
                                 2002::29              0       100     0       ? Or-ID: 10.0.0.29 C-LST: 100.0.0.53 
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
 * >      RD: 1:199 IPv6 prefix 2001:20:199:225::/64
                                 2002::199             0       100     0       ? Or-ID: 20.49.199.199 C-LST: 100.0.0.53 
 * >      RD: 1:336 IPv6 prefix 2001:20:336:225::/64
                                 2002::336             -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
 * >      RD: 21:302 IPv6 prefix 2001:21:102:225::/64
                                 2002::302             -       100     0       i Or-ID: 10.0.1.2 C-LST: 100.0.0.53 
          RD: 21:307 IPv6 prefix 2001:21:107:225::/64
                                 2002::307             -       100     0       i Or-ID: 10.0.1.7 C-LST: 100.0.0.53 
 * >      RD: 21:310 IPv6 prefix 2001:21:110:225::/64
                                 2002::310             -       100     0       i Or-ID: 10.0.1.10 C-LST: 100.0.0.53 
          RD: 21:316 IPv6 prefix 2001:21:116:225::/64
                                 2002::316             -       100     0       i Or-ID: 10.0.1.16 C-LST: 100.0.0.53 
```

## show ipv6 route

```text

VRF: default
Displaying 71 of 76 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 I L2     10:10:10::20/128 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:11:310::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:11:353::/64 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:20:36::/64 [115/40]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:20:336::/64 [115/40]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:20:352::/64 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:28:316::/64 [115/30]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:0:28:336::/64 [115/40]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:28:352::/64 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:29:58::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:29:338::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:36:58::/64 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:36:310::/64 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:49:199::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:49:338::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:58:310::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:58:419::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2001:0:59:161::/64 [0/0]
           via Ethernet20, directly connected
 I L2     2001:0:59:352::/64 [115/20]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2001:0:161:342::/64 [0/0]
           via Ethernet10, directly connected
 I L2     2001:0:199:302::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:199:344::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:302:353::/64 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:307:352::/64 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:307:353::/64 [115/40]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:310:338::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:310:353::/64 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:316:342::/64 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:1:20:36::/64 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:1:20:336::/64 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::11/128 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::20/128 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::28/128 [115/30]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::29/128 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::36/128 [115/40]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::49/128 [115/90]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::58/128 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::59/128 [115/10]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2002::161/128 [0/0]
           via Loopback0, directly connected
 I L2     2002::199/128 [115/90]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::302/128 [115/80]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::307/128 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::310/128 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::316/128 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::336/128 [115/50]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::338/128 [115/80]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::342/128 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::344/128 [115/110]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::352/128 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::353/128 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::419/128 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::/72 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::/71 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     3001:0:29:338::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     3001:0:49:338::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:20::/48 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:28::/48 [115/30]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:36::/48 [115/40]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:59::/48 [115/10]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:307::/48 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:316::/48 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:336::/48 [115/40]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:342::/48 [115/11]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:352::/48 [115/21]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1310::/48 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1353::/48 [115/41]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1419::/48 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1000::/36 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:9307::/48 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:9310::/48 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:1:1000::/36 [115/80]
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
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 3, SRv6 SID fcbb:0:1011:e000::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.28.225.0/24 [200/0]
           via fcbb:0:28::/48, SRv6 Transport tunnel index 9, SRv6 SID fcbb:0:28:e100::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.29.225.0/24 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 3, SRv6 SID fcbb:0:1029:e100::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.36.225.0/24 [200/0]
           via fcbb:0:36::/48, SRv6 Transport tunnel index 11, SRv6 SID fcbb:0:36:e026::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.58.225.0/24 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 3, SRv6 SID fcbb:0:1058:e028::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.59.225.0/24 [200/0]
           via fcbb:0:59::/48, SRv6 Transport tunnel index 7, SRv6 SID fcbb:0:59:e017::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.102.225.0/24 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 3, SRv6 SID fcbb:0:1302:e002::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.107.225.0/24 [200/0]
           via fcbb:0:307::/48, SRv6 Transport tunnel index 8, SRv6 SID fcbb:0:307:e002::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.110.225.0/24 [200/0]
           via fcbb:0:1310::/48, SRv6 Transport tunnel index 4, SRv6 SID fcbb:0:1310:e000::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.116.225.0/24 [200/0]
           via fcbb:0:316::/48, SRv6 Transport tunnel index 13, SRv6 SID fcbb:0:316:e000::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.142.225.0/24 [200/0]
           via fcbb:0:342::/48, SRv6 Transport tunnel index 22, SRv6 SID fcbb:0:342:e010::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.144.225.0/24 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 3, SRv6 SID fcbb:0:1344:e00e::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.152.225.0/24 [200/0]
           via fcbb:0:352::/48, SRv6 Transport tunnel index 21, SRv6 SID fcbb:0:352:e010::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.153.225.0/24 [200/0]
           via fcbb:0:1353::/48, SRv6 Transport tunnel index 10, SRv6 SID fcbb:0:1353:e003::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        20.161.225.0/24 [0/0]
           via Vlan20, directly connected
 B I      20.199.225.0/24 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 3, SRv6 SID fcbb:0:1199:e027::
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
Displaying 71 of 76 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 I L2     10:10:10::20/128 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:11:310::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:11:353::/64 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:20:36::/64 [115/40]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:20:336::/64 [115/40]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:20:352::/64 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:28:316::/64 [115/30]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:0:28:336::/64 [115/40]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:28:352::/64 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:29:58::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:29:338::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:36:58::/64 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:36:310::/64 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:49:199::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:49:338::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:58:310::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:58:419::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2001:0:59:161::/64 [0/0]
           via Ethernet20, directly connected
 I L2     2001:0:59:352::/64 [115/20]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2001:0:161:342::/64 [0/0]
           via Ethernet10, directly connected
 I L2     2001:0:199:302::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:199:344::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:302:353::/64 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:307:352::/64 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:307:353::/64 [115/40]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:310:338::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:310:353::/64 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:316:342::/64 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:1:20:36::/64 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:1:20:336::/64 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::11/128 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::20/128 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::28/128 [115/30]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::29/128 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::36/128 [115/40]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::49/128 [115/90]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::58/128 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::59/128 [115/10]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2002::161/128 [0/0]
           via Loopback0, directly connected
 I L2     2002::199/128 [115/90]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::302/128 [115/80]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::307/128 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::310/128 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::316/128 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::336/128 [115/50]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::338/128 [115/80]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::342/128 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::344/128 [115/110]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::352/128 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::353/128 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::419/128 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::/72 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::/71 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     3001:0:29:338::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     3001:0:49:338::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:20::/48 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:28::/48 [115/30]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:36::/48 [115/40]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:59::/48 [115/10]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:307::/48 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:316::/48 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:336::/48 [115/40]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:342::/48 [115/11]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     fcbb:0:352::/48 [115/21]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1310::/48 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1353::/48 [115/41]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1419::/48 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1000::/36 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:9307::/48 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:9310::/48 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:1:1000::/36 [115/80]
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

 B I      2001:20:11:225::/64 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 3, SRv6 SID fcbb:0:1011:e001::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:28:225::/64 [200/0]
           via fcbb:0:28::/48, SRv6 Transport tunnel index 9, SRv6 SID fcbb:0:28:e101::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:29:225::/64 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 3, SRv6 SID fcbb:0:1029:e101::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:36:225::/64 [200/0]
           via fcbb:0:36::/48, SRv6 Transport tunnel index 11, SRv6 SID fcbb:0:36:e027::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:58:225::/64 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 3, SRv6 SID fcbb:0:1058:e029::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:59:225::/64 [200/0]
           via fcbb:0:59::/48, SRv6 Transport tunnel index 7, SRv6 SID fcbb:0:59:e018::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:102:225::/64 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 3, SRv6 SID fcbb:0:1302:e003::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:107:225::/64 [200/0]
           via fcbb:0:307::/48, SRv6 Transport tunnel index 8, SRv6 SID fcbb:0:307:e003::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:110:225::/64 [200/0]
           via fcbb:0:1310::/48, SRv6 Transport tunnel index 4, SRv6 SID fcbb:0:1310:e001::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:116:225::/64 [200/0]
           via fcbb:0:316::/48, SRv6 Transport tunnel index 13, SRv6 SID fcbb:0:316:e001::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:142:225::/64 [200/0]
           via fcbb:0:342::/48, SRv6 Transport tunnel index 22, SRv6 SID fcbb:0:342:e011::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:144:225::/64 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 3, SRv6 SID fcbb:0:1344:e00f::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:152:225::/64 [200/0]
           via fcbb:0:352::/48, SRv6 Transport tunnel index 21, SRv6 SID fcbb:0:352:e00f::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:153:225::/64 [200/0]
           via fcbb:0:1353::/48, SRv6 Transport tunnel index 10, SRv6 SID fcbb:0:1353:e004::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2001:20:161:225::/64 [0/0]
           via Vlan20, directly connected
 B I      2001:20:199:225::/64 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 3, SRv6 SID fcbb:0:1199:e026::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:20:336:225::/64 [200/0]
           via fcbb:0:336::/48, SRv6 Transport tunnel index 1, SRv6 SID fcbb:0:336:e664::
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

