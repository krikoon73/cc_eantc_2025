# Test results for PE41-J2-161

## show ipv6 route

```text

VRF: default
Displaying 54 of 59 IPv6 routing table entries
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
 I L2     2001:0:20:36::/64 [115/60]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:0:20:336::/64 [115/50]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:0:28:316::/64 [115/30]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:0:28:336::/64 [115/40]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:0:29:58::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:29:338::/64 [115/80]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:36:58::/64 [115/70]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:49:199::/64 [115/100]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:49:338::/64 [115/90]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:58:310::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:58:419::/64 [115/70]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2001:0:59:161::/64 [0/0]
           via Ethernet20, directly connected
 I L2     2001:0:59:352::/64 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2001:0:161:342::/64 [0/0]
           via Ethernet10, directly connected
 I L2     2001:0:162:302::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:162:344::/64 [115/1060]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:199:344::/64 [115/110]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:302:353::/64 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:307:352::/64 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:307:353::/64 [115/40]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:310:353::/64 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2001:0:316:342::/64 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:1:20:36::/64 [115/60]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2001:1:59:352::/64 [115/20]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::20/128 [115/50]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::28/128 [115/30]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::36/128 [115/60]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::58/128 [115/60]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::59/128 [115/10]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 C        2002::161/128 [0/0]
           via Loopback0, directly connected
 I L2     2002::307/128 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::310/128 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::316/128 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::336/128 [115/50]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::342/128 [115/20]
           via fe80::fa7a:41ff:fe18:8910, Ethernet10
 I L2     2002::352/128 [115/30]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::353/128 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::419/128 [115/80]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     2002::/72 [115/50]
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
 I L2     fcbb:0:1310::/48 [115/50]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1353::/48 [115/41]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1419::/48 [115/80]
           via fe80::8e7a:ff:fee7:f53d, Ethernet20
 I L2     fcbb:0:1000::/36 [115/50]
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
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 175, SRv6 SID fcbb:0:1011:e001::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.20.225.0/24 [200/0]
           via fcbb:0:20::/48, SRv6 Transport tunnel index 118, SRv6 SID fcbb:0:20:e100::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.28.225.0/24 [200/0]
           via fcbb:0:28::/48, SRv6 Transport tunnel index 129, SRv6 SID fcbb:0:28:e100::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.29.225.0/24 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 175, SRv6 SID fcbb:0:1029:e100::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.36.225.0/24 [200/0]
           via fcbb:0:36::/48, SRv6 Transport tunnel index 117, SRv6 SID fcbb:0:36:e13f::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.58.225.0/24 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 175, SRv6 SID fcbb:0:1058:e017::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.59.225.0/24 [200/0]
           via fcbb:0:59::/48, SRv6 Transport tunnel index 106, SRv6 SID fcbb:0:59:e017::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.102.225.0/24 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 175, SRv6 SID fcbb:0:1302:e000::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.107.225.0/24 [200/0]
           via fcbb:0:307::/48, SRv6 Transport tunnel index 145, SRv6 SID fcbb:0:307:e000::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.110.225.0/24 [200/0]
           via fcbb:0:1310::/48, SRv6 Transport tunnel index 165, SRv6 SID fcbb:0:1310:e000::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.116.225.0/24 [200/0]
           via fcbb:0:316::/48, SRv6 Transport tunnel index 152, SRv6 SID fcbb:0:316:e002::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.136.225.0/24 [200/0]
           via fcbb:0:336::/48, SRv6 Transport tunnel index 105, SRv6 SID fcbb:0:336:e664::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.138.225.0/24 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 175, SRv6 SID fcbb:0:1338:e666::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.142.225.0/24 [200/0]
           via fcbb:0:342::/48, SRv6 Transport tunnel index 112, SRv6 SID fcbb:0:342:e002::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      20.144.225.0/24 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 175, SRv6 SID fcbb:0:1344:e001::
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
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 175, SRv6 SID fcbb:0:1162:400::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20
 B I      20.199.225.0/24 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 175, SRv6 SID fcbb:0:1199:e1b7::
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
    h3c_20_CR16010E-F.00-00       599  17562   677    571 L2  0000.0000.0020.00-00  <>
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
        IPv6 Neighbor Address: 2001:0:20:336::336
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
    h3c_28_S12500R-2L.00-00       288  55792   701    428 L2  0000.0000.0028.00-00  <>
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
        IPv6 Neighbor Address: 2001:0:28:336::336
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
    huawei_36.00-00             440  17766   914    693 L2  0000.0000.0036.00-00  <>
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
    anet-161-R3.00-00           456  38618   638    250 L2  0000.0000.0161.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 338 s
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
    JNPR-307-ACX7024.00-00       178  19720   504    343 L2  0000.0000.0307.00-00  <>
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
    JNPR-310-ACX7100-48L.00-00       757  22478   918    300 L2  0000.0000.0310.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: JNPR-310-ACX7100-48L
      Area addresses: 49.0001
      Interface address: 10.0.1.10
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::58
        Global IPv6 Interface Address: 2001:0:58:310::310
      Reachability          : 2001:0:58:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:310:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::310/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:1310::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:1310::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
      Router Capabilities: Router Id: 10.0.1.10 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    JNPR-310-ACX7100-48L.00-01       448   6092   947     72 L2  0000.0000.0310.00-01  <>
      IS Neighbor          : Cisco353-8201-24H8FH.00 Metric: 10
        Global IPv6 Interface Address: 2001:0:310:353::353
    JNPR-316-MX304.00-00        266   8867   647    369 L2  0000.0000.0316.00-00  <>
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
    ZTE_336_ZXR10_M6000-8SE.00-00       498  17246   863    474 L2  0000.0000.0336.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: ZTE_336_ZXR10_M6000-8SE
      Area addresses: 49.0000
      Interface address: 10.0.1.36
      Interface address: 2002::336
      IS Neighbor          : h3c_20_CR16010E-F.00 Metric: 10
        IPv6 Neighbor Address: 2001:1:20:36::20
        Global IPv6 Interface Address: 2001:0:20:336::336
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
      Router Capabilities: Router Id: 10.0.1.36 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 4096
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  20
        SRv6 Capability: Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 900000 Range: 65536
        Algorithms:  0, 1
    Cisco342-9902.00-00         263   1430   698    417 L2  0000.0000.0342.00-00  <>
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
    Cisco352-N540.00-00         426  30852   635    435 L2  0000.0000.0352.00-00  <>
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
    Cisco353-8201-24H8FH.00-00       729  63953  1189    696 L2  0000.0000.0353.00-00  <>
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
      Reachability          : 2002::/72 Metric: 10 Type: 1 Up
      Reachability          : 2002::353/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1000::/36 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1353::/48 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:29:58::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:29:338::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 60 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:162:302::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:162:344::/64 Metric: 1020 Type: 1 Up
      Reachability          : 2001:0:199:344::/64 Metric: 70 Type: 1 Up
      Reachability          : 2001:0:11:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:49:338::/64 Metric: 50 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:310:353::/64 Metric: 20 Type: 1 Up
      SRv6 Locator: fcbb:0:1000::/36 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
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
    Nokia_58-SR1-3-SRv6.00-00       472  12709 65520    313 L2  0100.0000.0058.00-00  <>
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
      Reachability          : 2001:0:36:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::58/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.58 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0
    Nokia_58-SR1-3-SRv6.00-01       363  47379 65519    365 L2  0100.0000.0058.00-01  <>
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::310
        Global IPv6 Interface Address: 2001:0:58:310::58
      IS Neighbor          : Keys-Ixia-419.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:58:419::419
        Global IPv6 Interface Address: 2001:0:58:419::58
    Nokia-59-IXRe2.00-00        242  25862  1081    488 L2  0100.0000.0059.00-00  <>
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
    Keys-Ixia-419.00-00         168  60522  1192    351 L2  3800.0000.0419.00-00  <DefaultAtt>
      NLPID: 0xCC(IPv4) 0x8E(IPv6) 0x81(CLNP)
      Hostname: Keys-Ixia-419
      Area addresses: 49.0001
      Interface address: 2001:0:58:419::419
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:419::58
        Global IPv6 Interface Address: 2001:0:58:419::419
      Reachability          : 2002::419/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1419::/48 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:1419::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1419:11::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.1.119 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0
```

