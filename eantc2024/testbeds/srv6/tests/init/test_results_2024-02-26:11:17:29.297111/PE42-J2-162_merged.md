# Test results for PE42-J2-162

## show version

```text
Arista DCS-7280SR3-40YC6-F
Hardware version: 11.02
Serial number: JPA2339P1QH
Hardware MAC address: 606b.5b2e.f3fd
System MAC address: 606b.5b2e.f3fd

Software image version: 4.31.2F
Architecture: i686
Internal build version: 4.31.2F-35442146.4312F
Internal build ID: 635a071a-386e-447f-942c-bcc34d9ffd3c
Image format version: 3.0
Image optimization: Default

Uptime: 3 hours and 20 minutes
Total memory: 8099732 kB
Free memory: 5700460 kB

```

## show interfaces status

```text
Port       Name     Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1                 notconnect   1        full   25G    Not Present                    
Et2                 notconnect   1        full   25G    Not Present                    
Et3                 notconnect   1        full   25G    Not Present                    
Et4                 notconnect   1        full   25G    Not Present                    
Et5                 notconnect   1        full   10G    10GBASE-SRL                    
Et6                 notconnect   1        full   25G    Not Present                    
Et7                 notconnect   1        full   25G    Not Present                    
Et8                 notconnect   1        full   25G    Not Present                    
Et9                 notconnect   1        full   25G    Not Present                    
Et10                disabled     routed   full   10G    10GBASE-SRL                    
Et11                notconnect   1        full   25G    Not Present                    
Et12                disabled     trunk    full   10G    10GBASE-LR                     
Et13                notconnect   1        full   25G    Not Present                    
Et14                notconnect   1        full   25G    Not Present                    
Et15                notconnect   1        full   25G    Not Present                    
Et16                notconnect   1        full   25G    Not Present                    
Et17                notconnect   1        full   25G    Not Present                    
Et18                notconnect   1        full   25G    Not Present                    
Et19                notconnect   1        full   25G    Not Present                    
Et20                disabled     routed   full   10G    10GBASE-SR                     
Et21                notconnect   1        full   25G    Not Present                    
Et22                notconnect   1        full   25G    Not Present                    
Et23                notconnect   1        full   25G    Not Present                    
Et24                notconnect   1        full   25G    Not Present                    
Et25                notconnect   1        full   25G    Not Present                    
Et26                notconnect   1        full   25G    Not Present                    
Et27                notconnect   1        full   25G    Not Present                    
Et28                notconnect   1        full   25G    Not Present                    
Et29                notconnect   1        full   25G    Not Present                    
Et30                notconnect   1        full   25G    Not Present                    
Et31                notconnect   1        full   25G    Not Present                    
Et32                notconnect   1        full   25G    Not Present                    
Et33                notconnect   1        full   25G    Not Present                    
Et34                notconnect   1        full   25G    Not Present                    
Et35                notconnect   1        full   25G    Not Present                    
Et36                notconnect   1        full   25G    Not Present                    
Et37                errdisabled  1        full   25G    Not Present                    
Et38                errdisabled  1        full   25G    Not Present                    
Et39                disabled     1        full   10G    10GBASE-SRL                    
Et40                disabled     1        full   10G    10GBASE-SRL                    
Et41/1     Nokia_57 connected    routed   full   10G    40GBASE-SR4                    
Et41/2              notconnect   1        full   10G    40GBASE-SR4                    
Et41/3              notconnect   1        full   10G    40GBASE-SR4                    
Et41/4              notconnect   1        full   10G    40GBASE-SR4                    
Et43/1              notconnect   1        full   100G   Not Present                    
Et44/1              notconnect   1        full   100G   Not Present                    
Et45/1              notconnect   1        full   100G   Not Present                    
Et46/1              notconnect   1        full   100G   Not Present                    
Ma1                 connected    routed   a-full a-1G   10/100/1000                    

```

## show lldp neighbors

```text
Last table change time   : 2:53:24 ago
Number of table inserts  : 2
Number of table deletes  : 0
Number of table drops    : 0
Number of table age-outs : 0

Port            Neighbor Device ID       Neighbor Port ID    TTL
------------ ------------------------ ---------------------- ---
Et41/1          NOKIA-SR2-57             1610899526          121
Ma1             extreme-x460-1           22                  120

```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
IPV6      default  NOKIA-SR2-57     L2   Ethernet41/1       P2P               UP    27          00                  
```

## show segment-routing ipv6 locator

```text
```

## show segment-routing ipv6 locator std

```text
```

## show segment-routing ipv6 sid function allocators

```text
! Segment Routing over IPv6 is not enabled
SRv6 SID function allocators for VRF default

```

## show segment-routing ipv6 capabilities

```text
```

## show segment-routing ipv6 route

```text
! Segment Routing over IPv6 is not enabled
VRF default
Source Codes: B3 - BGP L3 VPN, S - Static
End Behaviors: End - Endpoint
               End.DT4 (6) - Endpoint with decapsulation and specific IPv4 (6) table lookup

```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.162, local AS number 65000
Neighbor Status Codes: m - Under maintenance
  Neighbor  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  2002::59  4 65000            438      8815    0    0 02:53:18 Estab   2      2
  2002::304 4 65000          29620     39436    0    0 00:00:00 Active
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.162, local AS number 65000
BGP routing table entry for ip-prefix 57.57.57.57/32, Route Distinguisher: 10.0.0.57:6002
 Paths: 1 available
  1
    2002::57 from 2002::59 (10.0.0.59)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.0.57, Cluster list: 0.231.244.180 
      Extended Community: Route-Target-AS:65000:6002 TunnelEncap:tunnelTypeMpls
      Rx path id: 0xf
      MPLS label: 524280
BGP routing table entry for ip-prefix 162.162.162.162/32, Route Distinguisher: 10.0.0.162:1
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:65000:6001 Route-Target-AS:65000:6002 TunnelEncap:tunnelTypeMpls
      MPLS label: 116384
```

## show tunnel fib

```text

Type 'IS-IS SR', index 1, endpoint 2002::59/128, forwarding None
   via fe80::1a5b:ff:fe89:bfcc, 'Ethernet41/1' label 20159

Type 'IS-IS SR', index 2, endpoint 2002::57/128, forwarding None
   via fe80::1a5b:ff:fe89:bfcc, 'Ethernet41/1' label 20157

Type 'IS-IS SR', index 3, endpoint 2002::303/128, forwarding None
   via fe80::1a5b:ff:fe89:bfcc, 'Ethernet41/1' label 20303

Type 'IS-IS SR', index 4, endpoint 2002::304/128, forwarding None
   via fe80::1a5b:ff:fe89:bfcc, 'Ethernet41/1' label 20304
```

## show bgp neighbors 2002::353 vpn-ipv4 advertised-routes detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.162, local AS number 65000
```

## show bgp neighbors 2002::353 vpn-ipv6 advertised-routes detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.162, local AS number 65000
```

## show bgp vpn-ipv4

```text
BGP routing table information for VRF default
Router identifier 100.0.0.162, local AS number 65000
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
          RD: 10.0.0.59:209 IPv4 prefix 20.59.111.0/24
                                 10.0.0.59             -       100     0       i
          RD: 10.0.0.59:6001 IPv4 prefix 57.1.0.0/24
                                 10.0.0.59             -       100     0       i
          RD: 10.0.0.59:6001 IPv4 prefix 57.1.0.57/32
                                 10.0.0.59             0       100     0       i
 * >      RD: 10.0.0.162:1 IPv4 prefix 57.57.57.57/32
                                 -                     -       100     0       1 i Or-ID: 10.0.0.57 C-LST: 0.231.244.180 
          RD: 10.0.0.59:5001 IPv4 prefix 59.59.59.59/32
                                 10.0.0.59             -       100     0       i
          RD: 10.0.0.59:6001 IPv4 prefix 59.59.59.59/32
                                 10.0.0.59             -       100     0       i
 * >      RD: 10.0.0.162:1 IPv4 prefix 162.162.162.162/32
                                 -                     -       -       0       i
```

## show bgp vpn-ipv6

```text
BGP routing table information for VRF default
Router identifier 100.0.0.162, local AS number 65000
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 10.0.0.59:6001 IPv6 prefix 59::59/128
                                 2002::59              -       100     0       i
 * >      RD: 10.0.0.103:8 IPv6 prefix 2001:0:83:111::/64
                                 2002::303             -       100     0       i Or-ID: 192.168.21.3 C-LST: 10.0.0.103 
 *        RD: 10.0.0.103:8 IPv6 prefix 2001:0:83:111::/64
                                 2002::303             -       100     0       1 i Or-ID: 192.168.21.3 C-LST: 0.231.244.180 
 * >      RD: 10.0.0.162:1 IPv6 prefix 2002:162::162/128
                                 -                     -       -       0       i
 * >      RD: 10.0.0.57:1 IPv6 prefix 2600:50:10:57::/64
                                 2002::57              -       100     0       i Or-ID: 10.0.0.57 C-LST: 10.0.0.103 
 *        RD: 10.0.0.57:1 IPv6 prefix 2600:50:10:57::/64
                                 2002::57              -       100     0       1 i Or-ID: 10.0.0.57 C-LST: 0.231.244.180 
 * >      RD: 10.0.0.162:1 IPv6 prefix 5757::/64
                                 -                     -       100     0       1 i Or-ID: 10.0.0.57 C-LST: 0.231.244.180 
 * >      RD: 10.0.0.57:6001 IPv6 prefix 5757:1::/64
                                 2002::57              -       100     0       i Or-ID: 10.0.0.57 C-LST: 10.0.0.103 
 *        RD: 10.0.0.57:6001 IPv6 prefix 5757:1::/64
                                 2002::57              -       100     0       1 i Or-ID: 10.0.0.57 C-LST: 0.231.244.180 
 * >      RD: 10.0.0.59:6001 IPv6 prefix 5757:1::/64
                                 2002::59              -       100     0       i
 * >      RD: 10.0.0.59:6001 IPv6 prefix 5757:1::57/128
                                 2002::59              0       100     0       i
```

## show ipv6 route

```text

VRF: default
Displaying 12 of 16 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 I L2     2001:0:5:57::/64 [115/20]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 I L2     2001:0:57:59::/64 [115/20]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 C        2001:0:57:162::/64 [0/0]
           via Ethernet41/1, directly connected
 I L2     2001:0:57:303::/64 [115/20]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 I L2     2001:0:57:304::/64 [115/20]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 I L2     2001:0:59:304::/64 [115/30]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 I L2     2001:0:303:304::/64 [115/30]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 I L2     2002::57/128 [115/10]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 I L2     2002::59/128 [115/20]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 C        2002::162/128 [0/0]
           via Loopback0, directly connected
 I L2     2002::303/128 [115/20]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 I L2     2002::304/128 [115/20]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1

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

 C        100.0.0.162/32
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



VRF: IPV6
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

 B I      57.57.57.57/32 [200/0]
           via 2002::57/128, IS-IS SR tunnel index 2, label 524280
              via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1, label 20157
 C        162.162.162.162/32 [0/0]
           via Loopback100, directly connected


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
Displaying 12 of 16 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 I L2     2001:0:5:57::/64 [115/20]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 I L2     2001:0:57:59::/64 [115/20]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 C        2001:0:57:162::/64 [0/0]
           via Ethernet41/1, directly connected
 I L2     2001:0:57:303::/64 [115/20]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 I L2     2001:0:57:304::/64 [115/20]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 I L2     2001:0:59:304::/64 [115/30]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 I L2     2001:0:303:304::/64 [115/30]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 I L2     2002::57/128 [115/10]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 I L2     2002::59/128 [115/20]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 C        2002::162/128 [0/0]
           via Loopback0, directly connected
 I L2     2002::303/128 [115/20]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1
 I L2     2002::304/128 [115/20]
           via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1


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



VRF: IPV6
Displaying 6 of 9 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 B I      59::59/128 [200/0]
           via 2002::59/128, IS-IS SR tunnel index 1, label 1048574
              via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1, label 20159
 B I      2001:0:83:111::/64 [200/0]
           via 2002::303/128, IS-IS SR tunnel index 3, label 16
              via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1, label 20303
 C        2002:162::162/128 [0/0]
           via Loopback100, directly connected
 B I      5757::/64 [200/0]
           via 2002::57/128, IS-IS SR tunnel index 2, label 524280
              via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1, label 20157
 B I      5757:1::57/128 [200/0]
           via 2002::59/128, IS-IS SR tunnel index 1, label 1048574
              via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1, label 20159
 B I      5757:1::/64 [200/0]
           via 2002::59/128, IS-IS SR tunnel index 1, label 1048574
              via fe80::1a5b:ff:fe89:bfcc, Ethernet41/1, label 20159


VRF: VPNv4-uSID
Displaying 0 of 3 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route



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

