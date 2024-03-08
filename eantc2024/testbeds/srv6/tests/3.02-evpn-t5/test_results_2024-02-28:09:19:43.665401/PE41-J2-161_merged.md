# Test results for PE41-J2-161

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

## show interfaces ethernet 11,10,20 | grep rate

```text
  5 seconds input rate 4.97 Mbps (0.1% with framing overhead), 602 packets/sec
  5 seconds output rate 4.14 Mbps (0.0% with framing overhead), 502 packets/sec
  5 seconds input rate 10.4 Mbps (0.1% with framing overhead), 1305 packets/sec
  5 seconds output rate 10.4 Mbps (0.1% with framing overhead), 1305 packets/sec
  5 seconds input rate 12.4 Mbps (0.1% with framing overhead), 1507 packets/sec
  5 seconds output rate 13.3 Mbps (0.1% with framing overhead), 1606 packets/sec
```

## show lldp neighbors

```text
Last table change time   : 1:47:54 ago
Number of table inserts  : 7
Number of table deletes  : 2
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
srv6      default  Cisco342-9902    L2   Ethernet10         P2P               UP    24          00                  
srv6      default  Nokia-59-IXRe2   L2   Ethernet20         P2P               UP    27          00                  
```

## show tunnel fib

```text

Type 'SRv6 Transport', index 361, endpoint fcbb:1:1000::/36, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 362, endpoint fcbb:0:1310::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 363, endpoint fcbb:0:36::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 364, endpoint fcbb:0:1000::/36, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 365, endpoint fcbb:0:20::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 366, endpoint fcbb:0:28::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 367, endpoint fcbb:0:336::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 368, endpoint fcbb:0:307::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 369, endpoint fcbb:0:1353::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 372, endpoint fcbb:0:59::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 377, endpoint fcbb:0:342::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 378, endpoint fcbb:0:352::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 379, endpoint fcbb:0:419::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161
```

## show bgp evpn route-type ip-prefix ipv4

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 1:336 ip-prefix 20.136.225.0/24
                                 2002::336             -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
 * >      RD: 1:338 ip-prefix 20.138.225.0/24
                                 2002::338             -       100     0       ? Or-ID: 10.0.1.38 C-LST: 100.0.0.53 
 * >      RD: 1:342 ip-prefix 20.142.225.0/24
                                 2002::342             0       100     0       ? Or-ID: 100.0.0.42 C-LST: 100.0.0.53 
 * >      RD: 1:344 ip-prefix 20.144.225.0/24
                                 2002::344             0       100     0       ? Or-ID: 100.0.0.44 C-LST: 100.0.0.53 
 * >      RD: 1:352 ip-prefix 20.152.225.0/24
                                 2002::352             0       100     0       ? Or-ID: 100.0.0.52 C-LST: 100.0.0.53 
 * >      RD: 1:353 ip-prefix 20.153.225.0/24
                                 2002::353             0       100     0       ?
          RD: 21:336 ip-prefix 21.136.225.0/24
                                 2002::336             -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
 * >      RD: 21:338 ip-prefix 21.138.225.0/24
                                 2002::338             -       100     0       ? Or-ID: 10.0.1.38 C-LST: 100.0.0.53 
          RD: 21:352 ip-prefix 21.142.225.0/24
                                 2002::342             0       100     0       ? Or-ID: 100.0.0.42 C-LST: 100.0.0.53 
 * >      RD: 21:352 ip-prefix 21.144.225.0/24
                                 2002::344             0       100     0       ? Or-ID: 100.0.0.44 C-LST: 100.0.0.53 
          RD: 21:352 ip-prefix 21.152.225.0/24
                                 2002::352             0       100     0       ? Or-ID: 100.0.0.52 C-LST: 100.0.0.53 
 * >      RD: 21:352 ip-prefix 21.153.225.0/24
                                 2002::353             0       100     0       ?
 * >      RD: 24:20 ip-prefix 24.20.225.0/24
                                 2002::20              0       100     0       ? Or-ID: 10.0.0.20 C-LST: 100.0.0.53 
 * >      RD: 24:20 ip-prefix 24.29.225.0/24
                                 2002::29              0       100     0       ? Or-ID: 10.0.0.29 C-LST: 100.0.0.53 
 * >      RD: 24:36 ip-prefix 24.36.225.0/24
                                 2002::36              0       100     0       ? Or-ID: 192.168.20.36 C-LST: 100.0.0.53 
 * >      RD: 10.0.0.58:24 ip-prefix 24.58.225.0/24
                                 2002::58              -       100     0       i Or-ID: 10.0.0.58 C-LST: 100.0.0.53 
 * >      RD: 10.0.0.59:24 ip-prefix 24.59.225.0/24
                                 2002::59              -       100     0       i Or-ID: 10.0.0.59 C-LST: 100.0.0.53 
 * >      RD: 24:302 ip-prefix 24.102.225.0/24
                                 2002::302             -       100     0       i Or-ID: 10.0.1.2 C-LST: 100.0.0.53 
 * >      RD: 24:307 ip-prefix 24.107.225.0/24
                                 2002::307             -       100     0       i Or-ID: 10.0.1.7 C-LST: 100.0.0.53 
 * >      RD: 24:310 ip-prefix 24.110.225.0/24
                                 2002::310             -       100     0       i Or-ID: 10.0.1.10 C-LST: 100.0.0.53 
 * >      RD: 24:336 ip-prefix 24.136.225.0/24
                                 2002::336             -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
 * >      RD: 24:338 ip-prefix 24.138.225.0/24
                                 2002::338             -       100     0       ? Or-ID: 10.0.1.38 C-LST: 100.0.0.53 
 * >      RD: 24:342 ip-prefix 24.142.225.0/24
                                 2002::342             0       100     0       ? Or-ID: 100.0.0.42 C-LST: 100.0.0.53 
 * >      RD: 24:344 ip-prefix 24.144.225.0/24
                                 2002::344             0       100     0       ? Or-ID: 100.0.0.44 C-LST: 100.0.0.53 
 * >      RD: 24:352 ip-prefix 24.152.225.0/24
                                 2002::352             0       100     0       ? Or-ID: 100.0.0.52 C-LST: 100.0.0.53 
 * >      RD: 24:353 ip-prefix 24.153.225.0/24
                                 2002::353             0       100     0       ?
 * >      RD: 24:161 ip-prefix 24.161.225.0/24
                                 -                     -       -       0       i
 * >      RD: 0.0.4.25:24 ip-prefix 24.219.225.0/24
                                 2002::419             -       0       0       i Or-ID: 192.0.0.1 C-LST: 100.0.0.53 
```

## show bgp evpn route-type ip-prefix ipv6

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 1:336 ip-prefix 2001:20:336:225::/64
                                 2002::336             -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
 * >      RD: 1:338 ip-prefix 2001:20:338:225::/64
                                 2002::338             -       100     0       ? Or-ID: 10.0.1.38 C-LST: 100.0.0.53 
 * >      RD: 10.0.0.59:24 ip-prefix 2001:24:59:425::/64
                                 2002::59              -       100     0       i Or-ID: 10.0.0.59 C-LST: 100.0.0.53 
 * >      RD: 24:302 ip-prefix 2001:24:102:225::/64
                                 2002::302             -       100     0       i Or-ID: 10.0.1.2 C-LST: 100.0.0.53 
 * >      RD: 24:307 ip-prefix 2001:24:107:225::/64
                                 2002::307             -       100     0       i Or-ID: 10.0.1.7 C-LST: 100.0.0.53 
 * >      RD: 24:310 ip-prefix 2001:24:110:225::/64
                                 2002::310             -       100     0       i Or-ID: 10.0.1.10 C-LST: 100.0.0.53 
 * >      RD: 24:161 ip-prefix 2001:24:161:225::/64
                                 -                     -       -       0       i
 * >      RD: 24:336 ip-prefix 2001:24:336:225::/64
                                 2002::336             -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
 * >      RD: 24:338 ip-prefix 2001:24:338:225::/64
                                 2002::338             -       100     0       ? Or-ID: 10.0.1.38 C-LST: 100.0.0.53 
```

## show ipv6 route vrf EVPN-T5-uSID

```text

VRF: EVPN-T5-uSID
Displaying 7 of 11 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 B I      2001:24:59:425::/64 [200/0]
           via fcbb:0:59::/48, SRv6 Transport tunnel index 372, SRv6 SID fcbb:0:59:e031::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:24:102:225::/64 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 364, SRv6 SID fcbb:0:1302:e006::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:24:107:225::/64 [200/0]
           via fcbb:0:307::/48, SRv6 Transport tunnel index 368, SRv6 SID fcbb:0:307:e009::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      2001:24:110:225::/64 [200/0]
           via fcbb:0:1310::/48, SRv6 Transport tunnel index 362, SRv6 SID fcbb:0:1310:e013::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2001:24:161:225::/64 [0/0]
           via Vlan24, directly connected
 B I      2001:24:336:225::/64 [200/0]
           via fcbb:0:336::/48, SRv6 Transport tunnel index 367, SRv6 SID fcbb:0:336:e675::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:24:338:225::/64 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 364, SRv6 SID fcbb:0:1338:e674::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20

```

## show ip route vrf EVPN-T5-uSID

```text

VRF: EVPN-T5-uSID
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

 B I      24.20.225.0/24 [200/0]
           via fcbb:0:20::/48, SRv6 Transport tunnel index 365, SRv6 SID fcbb:0:20:e11f::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      24.29.225.0/24 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 364, SRv6 SID fcbb:0:1029:e114::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      24.36.225.0/24 [200/0]
           via fcbb:0:36::/48, SRv6 Transport tunnel index 363, SRv6 SID fcbb:0:36:e056::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      24.58.225.0/24 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 364, SRv6 SID fcbb:0:1058:e050::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      24.59.225.0/24 [200/0]
           via fcbb:0:59::/48, SRv6 Transport tunnel index 372, SRv6 SID fcbb:0:59:e030::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      24.102.225.0/24 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 364, SRv6 SID fcbb:0:1302:e005::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      24.107.225.0/24 [200/0]
           via fcbb:0:307::/48, SRv6 Transport tunnel index 368, SRv6 SID fcbb:0:307:e008::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      24.110.225.0/24 [200/0]
           via fcbb:0:1310::/48, SRv6 Transport tunnel index 362, SRv6 SID fcbb:0:1310:e012::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      24.136.225.0/24 [200/0]
           via fcbb:0:336::/48, SRv6 Transport tunnel index 367, SRv6 SID fcbb:0:336:e674::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      24.138.225.0/24 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 364, SRv6 SID fcbb:0:1338:e673::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      24.142.225.0/24 [200/0]
           via fcbb:0:342::/48, SRv6 Transport tunnel index 377, SRv6 SID fcbb:0:342:e014::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      24.144.225.0/24 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 364, SRv6 SID fcbb:0:1344:e010::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      24.152.225.0/24 [200/0]
           via fcbb:0:352::/48, SRv6 Transport tunnel index 378, SRv6 SID fcbb:0:352:e017::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      24.153.225.0/24 [200/0]
           via fcbb:0:1353::/48, SRv6 Transport tunnel index 369, SRv6 SID fcbb:0:1353:e007::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        24.161.225.0/24 [0/0]
           via Vlan24, directly connected

```

## show isis database detail

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: srv6 VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    h3c_20_CR16010E-F.00-00      3991  12298  1092   1237 L2  0000.0000.0020.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: h3c_20_CR16010E-F
      Area addresses: 49.0000
      Interface address: 2001:0:20:36::20
      Interface address: 2001:0:20:336::20
      Interface address: 2001:0:20:352::20
      Interface address: 2002::20
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:20:36::36
        Global IPv6 Interface Address: 2001:0:20:36::20
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:20:36::36
        Global IPv6 Interface Address: 2001:0:20:36::20
      IS Neighbor          : ZTE_336_ZXR10_M6000-8SE.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:336::336
        Global IPv6 Interface Address: 2001:0:20:336::20
      IS Neighbor          : Cisco352-N540.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:20:352::352
        Global IPv6 Interface Address: 2001:0:20:352::20
      IS Neighbor          : Cisco352-N540.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:20:352::352
        Global IPv6 Interface Address: 2001:0:20:352::20
      Reachability          : 2001:0:20:36::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:20:336::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:20:352::/64 Metric: 10 Type: 1 Up
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
      SRv6 Locator: fcbb:1:20::/48 Topology: 0
        Metric: 0 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:20::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 0
        SRv6 SID End
          SID : fcbb:1:20:e102::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP USP USD
          SID : fcbb:1:20:e103::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0, 128, 129, 130, 131
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 100
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 100
          Flags: [M] 0x80
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 100
          Flags: [M] 0x80
        Flex Algo: Algorithm: 131 Metric: IGP Metric (0) Calc: SPF (0) Prio: 100
          Flags: [M] 0x80
    h3c_20_CR16010E-F.00-01      1590  27535  1092    276 L2  0000.0000.0020.00-01  <>
      IS Neighbor          : ZTE_336_ZXR10_M6000-8SE.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:336::336
        Global IPv6 Interface Address: 2001:0:20:336::20
    h3c_28_S12500R-2L.00-00      1579   9698  1168    964 L2  0000.0000.0028.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: h3c_28_S12500R-2L
      Area addresses: 49
      Interface address: 2001:0:28:316::28
      Interface address: 2001:0:28:336::28
      Interface address: 2001:0:28:352::28
      Interface address: 2002::28
      IS Neighbor          : JNPR-316-MX304.00   Metric: 10
        IPv6 Neighbor Address: 2001:0:28:316::316
        Global IPv6 Interface Address: 2001:0:28:316::28
      IS Neighbor          : JNPR-316-MX304.00   Metric: 10
        IPv6 Neighbor Address: 2001:0:28:316::316
        Global IPv6 Interface Address: 2001:0:28:316::28
      IS Neighbor          : ZTE_336_ZXR10_M6000-8SE.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:28:336::336
        Global IPv6 Interface Address: 2001:0:28:336::28
      IS Neighbor          : ZTE_336_ZXR10_M6000-8SE.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:28:336::336
        Global IPv6 Interface Address: 2001:0:28:336::28
      IS Neighbor          : Cisco352-N540.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:28:352::352
        Global IPv6 Interface Address: 2001:0:28:352::28
      IS Neighbor          : Cisco352-N540.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:28:352::352
        Global IPv6 Interface Address: 2001:0:28:352::28
      Reachability          : 2001:0:28:316::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:28:336::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:28:352::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::28/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:28::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:28::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:28::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 0
      SRv6 Locator: fcbb:1:28::/48 Topology: 0
        Metric: 0 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:28::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 0
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0, 128
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 100
          Flags: [] 0x1
    huawei_36.00-00             221  13465   856   1030 L2  0000.0000.0036.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: huawei_36
      Area addresses: 49.0000
      Topology: 0 (IPv4)
      Interface address: 2002::36
      Interface address: 2001:0:36:58::36
      Interface address: 2001:0:20:36::36
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:36:58::58
        Global IPv6 Interface Address: 2001:0:36:58::36
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:36:58::58
        Global IPv6 Interface Address: 2001:0:36:58::36
      Reachability          : 2002::36/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:36::/48 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:20:36::/64 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:1:36::/48 Topology: 0
        Metric: 0 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:36::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
        SRv6 SID Un Supported
          SID : fcbb:1:36:e004::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 64
        SRv6 SID End
          SID : fcbb:1:36:e005::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP
          SID : fcbb:1:36:e006::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP USP USD
          SID : fcbb:1:36:e007::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:0:36::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:36::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
        SRv6 SID Un Supported
          SID : fcbb:0:36:e004::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 64
        SRv6 SID End
          SID : fcbb:0:36:e005::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP
          SID : fcbb:0:36:e006::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP USP USD
          SID : fcbb:0:36:e007::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0, 128, 129, 130
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 128
          Exclude admin groups: 1
          Flags: [M] 0x80
    huawei_36.00-01             899  30894   856    465 L2  0000.0000.0036.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      IS Neighbor          : h3c_20_CR16010E-F.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:36::20
        Global IPv6 Interface Address: 2001:0:20:36::36
      IS Neighbor          : h3c_20_CR16010E-F.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:36::20
        Global IPv6 Interface Address: 2001:0:20:36::36
    anet-161-R3.00-00           237  37307   512    250 L2  0000.0000.0161.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 212 s
      NLPID: 0x8E(IPv6)
      Hostname: anet-161-R3
      Area addresses: 49.0000
      Interface address: 2001:0:161:342::161
      Interface address: 2001:0:59:161::161
      Interface address: 2002::161
      IS Neighbor          : Cisco342-9902.00    Metric: 10
      IS Neighbor          : Nokia-59-IXRe2.00   Metric: 10
      Reachability          : fcbb:0:161::/48 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:161:342::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:59:161::/64 Metric: 10 Type: 1 Up
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
    JNPR-307-ACX7024.00-00      1532  35038  1150    675 L2  0000.0000.0307.00-00  <>
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
      Reachability          : fcbb:0:307::/48 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:9307::/48 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:307:352::/64 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:307::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:1:307::/48 Topology: 0
        Metric: 0 Algorithm: 128 Flags: []
      SRv6 Locator: fcbb:0:9307::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:0:9307::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:2:307::/48 Topology: 0
        Metric: 0 Algorithm: 129 Flags: []
      SRv6 Locator: fcbb:3:307::/48 Topology: 0
        Metric: 0 Algorithm: 130 Flags: []
      SRv6 Locator: fcbb:5:307::/48 Topology: 0
        Metric: 0 Algorithm: 132 Flags: []
      SRv6 Locator: fcbb:6:307::/48 Topology: 0
        Metric: 0 Algorithm: 133 Flags: []
      SRv6 Locator: fcbb:7:307::/48 Topology: 0
        Metric: 0 Algorithm: 134 Flags: []
      Router Capabilities: Router Id: 10.0.1.7 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1, 128, 129, 130, 132, 133, 134
        Flex Algo: Algorithm: 134 Metric: IGP Metric (0) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 133 Metric: IGP Metric (0) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 132 Metric: IGP Metric (0) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 0
          Exclude admin groups: 1
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 0
      Unsupported TLV: Type: 14 Length: 2
    JNPR-310-ACX7100-48L.00-00     12162  35022  1182    797 L2  0000.0000.0310.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: JNPR-310-ACX7100-48L
      Area addresses: 49.0001
      Interface address: 10.0.1.10
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::58
        Global IPv6 Interface Address: 2001:0:58:310::310
      IS Neighbor          : Cisco353-8201-24H8FH.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:310:353::353
        Global IPv6 Interface Address: 2001:0:310:353::353
      Reachability          : 2001:0:58:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:310:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:310:338::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::310/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:25:110:225::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::/72 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:9310::/48 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:1310::/48 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:1000::/36 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:9310::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:0:9310::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:2:1310::/48 Topology: 0
        Metric: 0 Algorithm: 129 Flags: []
      SRv6 Locator: fcbb:3:1310::/48 Topology: 0
        Metric: 0 Algorithm: 130 Flags: []
      SRv6 Locator: fcbb:0:1310::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:1:1310::/48 Topology: 0
        Metric: 0 Algorithm: 128 Flags: []
      SRv6 Locator: fcbb:5:1310::/48 Topology: 0
        Metric: 0 Algorithm: 132 Flags: []
      SRv6 Locator: fcbb:6:1310::/48 Topology: 0
        Metric: 0 Algorithm: 133 Flags: []
      SRv6 Locator: fcbb:7:1310::/48 Topology: 0
        Metric: 0 Algorithm: 134 Flags: []
      SRv6 Locator: fcbb:0:1000::/36 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:1:1000::/36 Topology: 0
        Metric: 10 Algorithm: 128 Flags: []
      Router Capabilities: Router Id: 10.0.1.10 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1, 128, 129, 130, 132, 133, 134
        Flex Algo: Algorithm: 134 Metric: IGP Metric (0) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 133 Metric: IGP Metric (0) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 132 Metric: IGP Metric (0) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 0
          Exclude admin groups: 1
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 0
      Unsupported TLV: Type: 14 Length: 2
    JNPR-316-MX304.00-00       1236  13165  1152    795 L2  0000.0000.0316.00-00  <>
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
      Reachability          : 2002::316/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:316:342::/64 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:316::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:316::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:0:316::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:1:316::/48 Topology: 0
        Metric: 0 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:1:316::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:2:316::/48 Topology: 0
        Metric: 0 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:2:316::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:3:316::/48 Topology: 0
        Metric: 0 Algorithm: 130 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:3:316::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:5:316::/48 Topology: 0
        Metric: 0 Algorithm: 132 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:5:316::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:6:316::/48 Topology: 0
        Metric: 0 Algorithm: 133 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:6:316::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:7:316::/48 Topology: 0
        Metric: 0 Algorithm: 134 Flags: []
      Router Capabilities: Router Id: 10.0.1.16 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1, 128, 129, 130, 132, 133, 134
        Flex Algo: Algorithm: 134 Metric: IGP Metric (0) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 133 Metric: IGP Metric (0) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 132 Metric: IGP Metric (0) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 0
          Exclude admin groups: 1
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 0
      Unsupported TLV: Type: 14 Length: 2
    ZTE_336_ZXR10_M6000-8SE.00-00      3026  62919  1178   1198 L2  0000.0000.0336.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: ZTE_336_ZXR10_M6000-8SE
      Area addresses: 49.0000
      Interface address: 10.0.1.36
      Interface address: 2002::336
      IS Neighbor          : h3c_20_CR16010E-F.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:336::20
        Global IPv6 Interface Address: 2001:0:20:336::336
      IS Neighbor          : h3c_20_CR16010E-F.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:336::20
        Global IPv6 Interface Address: 2001:0:20:336::336
      IS Neighbor          : h3c_28_S12500R-2L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:28:336::28
        Global IPv6 Interface Address: 2001:0:28:336::336
      IS Neighbor          : h3c_28_S12500R-2L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:28:336::28
        Global IPv6 Interface Address: 2001:0:28:336::336
      Reachability         : 10.0.1.36/32 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:20:336::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:28:336::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::336/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:336::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:336::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:0:336::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:1:336::/48 Topology: 0
        Metric: 0 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:1:336::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:2:336::/48 Topology: 0
        Metric: 0 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:2:336::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:3:336::/48 Topology: 0
        Metric: 0 Algorithm: 130 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:3:336::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:4:336::/48 Topology: 0
        Metric: 0 Algorithm: 131 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:4:336::
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
        Algorithms:  0, 1, 128, 129, 130, 131
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 100
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 128
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 128
          Exclude admin groups: 1
        Flex Algo: Algorithm: 131 Metric: IGP Metric (0) Calc: SPF (0) Prio: 128
          Exclude admin groups: 1,231
    Cisco342-9902.00-00         302  61020   473    563 L2  0000.0000.0342.00-00  <>
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
      SRv6 Locator: fcbb:1:342::/48 Topology: 0
        Metric: 1 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:342::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0, 1, 128
      Unsupported TLV: Type: 14 Length: 2
    Cisco352-N540.00-00         288  45713   478    943 L2  0000.0000.0352.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: Cisco352-N540
      Area addresses: 49.0001
      Interface address: 2002::352
      IS Neighbor          : h3c_20_CR16010E-F.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:352::20
        Global IPv6 Interface Address: 2001:0:20:352::352
      IS Neighbor          : h3c_28_S12500R-2L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:28:352::28
        Global IPv6 Interface Address: 2001:0:28:352::352
      IS Neighbor          : JNPR-307-ACX7024.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:307:352::307
        Global IPv6 Interface Address: 2001:0:307:352::352
      IS Neighbor          : Nokia-59-IXRe2.00   Metric: 10
        IPv6 Neighbor Address: 2001:0:59:352::59
        Global IPv6 Interface Address: 2001:0:59:352::352
      Reachability          : 2001:0:20:352::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:28:352::/64 Metric: 10 Type: 1 Up
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
      SRv6 Locator: fcbb:1:352::/48 Topology: 0
        Metric: 1 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:352::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0, 1, 128
      Unsupported TLV: Type: 14 Length: 2
    Cisco353-8201-24H8FH.00-00      2382  47384   562    999 L2  0000.0000.0353.00-00  <>
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
        IPv6 Neighbor Address: 2001:0:310:353::353
        Global IPv6 Interface Address: 2001:0:310:353::353
      Reachability          : 2001:0:11:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:11:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:29:338::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:49:338::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:307:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:310:338::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:310:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::/72 Metric: 10 Type: 1 Up
      Reachability          : 2002::353/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:419::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1000::/36 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1353::/48 Metric: 1 Type: 1 Up
      Reachability          : fcbb:1:1000::/36 Metric: 5 Type: 1 Up
      Reachability          : 2001:0:29:58::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:199:302::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:199:344::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:302:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:25:110:225::/64 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:9310::/48 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:419::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1000::/36 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1353::/48 Topology: 0
        Metric: 1 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1353::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:0:9310::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:1:1000::/36 Topology: 0
        Metric: 5 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:1:1353::/48 Topology: 0
        Metric: 1 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:1353::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0, 1, 128
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
      Unsupported TLV: Type: 14 Length: 2
    Nokia_58-SR1-3-SRv6.00-00      1420  52243 65443    707 L2  0100.0000.0058.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia_58-SR1-3-SRv6
      Area addresses:
        49.0000
        49.0001
      Interface address: 10.0.0.58
      Interface address: 2001:0:36:58::58
      Interface address: 2001:0:58:310::58
      Interface address: 2001:0:58:419::58
      Interface address: 2002::58
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:36:58::36
        Global IPv6 Interface Address: 2001:0:36:58::58
      Reachability         : 10.0.0.58/32 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:29:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:199:344::/64 Metric: 50 Type: 1 Up
      Reachability          : 2002::58/128 Metric: 0 Type: 1 Up
      Reachability          : 2002::199/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::338/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::344/128 Metric: 60 Type: 1 Up
      Reachability          : fcbb:0:1000::/36 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:1000::/36 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:1:1302::/48 Topology: 0
        Metric: 802 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:1:1302::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:1:1344::/48 Topology: 0
        Metric: 20801 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:1344::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:1:1353::/48 Topology: 0
        Metric: 753 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:1353::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.0.58 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 128
    Nokia_58-SR1-3-SRv6.00-01      4182  46608 65444   1180 L2  0100.0000.0058.00-01  <>
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::310
        Global IPv6 Interface Address: 2001:0:58:310::58
      IS Neighbor          : Keys-Ixia-419.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:58:419::419
        Global IPv6 Interface Address: 2001:0:58:419::58
      Reachability          : 2001:0:11:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:11:353::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:29:338::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:0:49:338::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:199:302::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:0:302:353::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:310:338::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:310:353::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:25:110:225::/64 Metric: 20 Type: 1 Up
      Reachability          : 2002::/71 Metric: 20 Type: 1 Up
      Reachability          : 2002::11/128 Metric: 20 Type: 1 Up
      Reachability          : 2002::29/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::49/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::302/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::310/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::353/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::419/128 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:419::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:9310::/48 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:419::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:419:11::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:0:9310::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:0:9310::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:1:1011::/48 Topology: 0
        Metric: 71 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:1011::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:1:1029::/48 Topology: 0
        Metric: 100 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:1029::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 0
      SRv6 Locator: fcbb:1:1058::/48 Topology: 0
        Metric: 0 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:1058::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:1:1199::/48 Topology: 0
        Metric: 10801 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:1199::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
        SRv6 SID Un Supported
          SID : fcbb:1:1199:e001::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 64
        SRv6 SID End
          SID : fcbb:1:1199:e002::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP
          SID : fcbb:1:1199:e003::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP USP USD
          SID : fcbb:1:1199:e004::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:1:1310::/48 Topology: 0
        Metric: 50 Algorithm: 128 Flags: []
      SRv6 Locator: fcbb:1:1338::/48 Topology: 0
        Metric: 79 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:1:1338::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
    Nokia-59-IXRe2.00-00        394  10244   979    883 L2  0100.0000.0059.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-59-IXRe2
      Area addresses: 49.0000.0000.0059.00
      Interface address: 10.0.0.59
      Interface address: 2001:0:59:161::59
      Interface address: 2001:0:59:352::59
      Interface address: 2002::59
      IS Neighbor          : anet-161-R3.00      Metric: 10
        Global IPv6 Interface Address: 2001:0:59:161::59
        Adj-sid: 1048572 flags: [L V B F] weight: 0x0
      IS Neighbor          : Cisco352-N540.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:59:352::352
        Global IPv6 Interface Address: 2001:0:59:352::59
        Adj-sid: 1048573 flags: [L V B F] weight: 0x0
      Reachability         : 10.0.0.59/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 59 Flags: [N P] Algorithm: 0
      Reachability          : 2001:0:59:161::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:59:352::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::59/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 159 Flags: [N P] Algorithm: 0
      Reachability          : fcbb:0:59::/48 Metric: 0 Type: 1 Up
      Reachability          : fcbb:3:59::/48 Metric: 0 Type: 1 Up
      Reachability          : fcbb:4:59::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:59::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:59::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:1:59::/48 Topology: 0
        Metric: 0 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:59::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:3:59::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:3:59::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:4:59::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:4:59::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.0.59 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  9
        SRv6 Capability: Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130, 131
    Keys-Ixia-419.00-00         462  20512   567    351 L2  3800.0000.0419.00-00  <DefaultAtt>
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
Locator: fcbb:0:20::/48
System ID: h3c_20_CR16010E-F
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:2:336::/48
System ID: ZTE_336_ZXR10_M6000-8SE
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:3:316::/48
System ID: JNPR-316-MX304
Flags: Down: unset
Level: 2
Algorithm: 130, Topology: 0

Locator: fcbb:1:336::/48
System ID: ZTE_336_ZXR10_M6000-8SE
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:1:1000::/36
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:336::/48
System ID: ZTE_336_ZXR10_M6000-8SE
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:1:28::/48
System ID: h3c_28_S12500R-2L
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:1:352::/48
System ID: Cisco352-N540
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:1:1302::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:0:36::/48
System ID: huawei_36
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:3:336::/48
System ID: ZTE_336_ZXR10_M6000-8SE
Flags: Down: unset
Level: 2
Algorithm: 130, Topology: 0

Locator: fcbb:7:307::/48
System ID: JNPR-307-ACX7024
Flags: Down: unset
Level: 2
Algorithm: 134, Topology: 0

Locator: fcbb:1:1199::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:0:9307::/48
System ID: JNPR-307-ACX7024
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:6:316::/48
System ID: JNPR-316-MX304
Flags: Down: unset
Level: 2
Algorithm: 133, Topology: 0

Locator: fcbb:1:1000::/36
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:6:307::/48
System ID: JNPR-307-ACX7024
Flags: Down: unset
Level: 2
Algorithm: 133, Topology: 0

Locator: fcbb:5:307::/48
System ID: JNPR-307-ACX7024
Flags: Down: unset
Level: 2
Algorithm: 132, Topology: 0

Locator: fcbb:5:1310::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: 132, Topology: 0

Locator: fcbb:1:1344::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:4:59::/48
System ID: Nokia-59-IXRe2
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1310::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:7:1310::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: 134, Topology: 0

Locator: fcbb:5:316::/48
System ID: JNPR-316-MX304
Flags: Down: unset
Level: 2
Algorithm: 132, Topology: 0

Locator: fcbb:1:316::/48
System ID: JNPR-316-MX304
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:1:1058::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:2:316::/48
System ID: JNPR-316-MX304
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:1:1338::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

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

Locator: fcbb:3:1310::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: 130, Topology: 0

Locator: fcbb:0:161::/48
System ID: anet-161-R3
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:1:307::/48
System ID: JNPR-307-ACX7024
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:0:419::/48
System ID: Nokia_58-SR1-3-SRv6
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

Locator: fcbb:1:59::/48
System ID: Nokia-59-IXRe2
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:7:316::/48
System ID: JNPR-316-MX304
Flags: Down: unset
Level: 2
Algorithm: 134, Topology: 0

Locator: fcbb:0:307::/48
System ID: JNPR-307-ACX7024
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1000::/36
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1000::/36
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:1000::/36
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:1:20::/48
System ID: h3c_20_CR16010E-F
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:1:1011::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:3:59::/48
System ID: Nokia-59-IXRe2
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:4:336::/48
System ID: ZTE_336_ZXR10_M6000-8SE
Flags: Down: unset
Level: 2
Algorithm: 131, Topology: 0

Locator: fcbb:2:1310::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:1:1310::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:1:1310::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:0:1353::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:1:1029::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:1:342::/48
System ID: Cisco342-9902
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:0:316::/48
System ID: JNPR-316-MX304
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:3:307::/48
System ID: JNPR-307-ACX7024
Flags: Down: unset
Level: 2
Algorithm: 130, Topology: 0

Locator: fcbb:0:342::/48
System ID: Cisco342-9902
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:9310::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:9310::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:9310::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:352::/48
System ID: Cisco352-N540
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:6:1310::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: 133, Topology: 0

Locator: fcbb:1:1353::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:1:1353::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:1:36::/48
System ID: huawei_36
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:2:307::/48
System ID: JNPR-307-ACX7024
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

```

## show arp vrf EVPN-T5-uSID

```text
Address         Age (sec)  Hardware Addr   Interface
24.161.225.225    1:11:24  0020.0100.0001  Vlan24, Ethernet11
```

## show mac address-table vlan 24

```text
          Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports      Moves   Last Move
----    -----------       ----        -----      -----   ---------
  24    0020.0100.0001    DYNAMIC     Et11       1       0:18:35 ago
  24    00aa.aaaa.aaaa    STATIC      Router
  24    606b.5b2e.fe11    STATIC      Router
Total Mac Addresses for this criterion: 3

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

