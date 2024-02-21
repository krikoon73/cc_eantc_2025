# Test results for PE42-J2-162

## show ipv6 route

```text

VRF: default
Displaying 52 of 57 IPv6 routing table entries
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
 I L1     2001:0:20:36::/64 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:20:336::/64 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:28:316::/64 [115/90]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:28:336::/64 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:29:58::/64 [115/50]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:29:338::/64 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:36:58::/64 [115/50]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:49:199::/64 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:49:338::/64 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:58:310::/64 [115/40]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:58:419::/64 [115/50]
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
 I L1     2001:0:199:344::/64 [115/90]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:302:353::/64 [115/20]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:307:352::/64 [115/40]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:307:353::/64 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:310:353::/64 [115/40]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:0:316:342::/64 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:1:20:36::/64 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2001:1:59:352::/64 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::11/128 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::29/128 [115/50]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::49/128 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::58/128 [115/40]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 C        2002::162/128 [0/0]
           via Loopback0, directly connected
 I L1     2002::199/128 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::302/128 [115/10]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::310/128 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::338/128 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::344/128 [115/100]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::353/128 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::419/128 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     2002::/71 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb::/36 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1011::/48 [115/40]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1029::/48 [115/50]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1049::/48 [115/70]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1058::/48 [115/40]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1199::/48 [115/80]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1302::/48 [115/10]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1310::/48 [115/30]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1338::/48 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1344::/48 [115/91]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1353::/48 [115/21]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     fcbb:0:1419::/48 [115/60]
           via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 I L1     ::/0 [115/20]
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
           via fcbb::/36, SRv6 Transport tunnel index 213, SRv6 SID fcbb:0:20:e100::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.28.225.0/24 [200/0]
           via fcbb::/36, SRv6 Transport tunnel index 213, SRv6 SID fcbb:0:28:e100::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.29.225.0/24 [200/0]
           via fcbb:0:1029::/48, SRv6 Transport tunnel index 189, SRv6 SID fcbb:0:1029:e100::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.36.225.0/24 [200/0]
           via fcbb::/36, SRv6 Transport tunnel index 213, SRv6 SID fcbb:0:36:e13f::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.58.225.0/24 [200/0]
           via fcbb:0:1058::/48, SRv6 Transport tunnel index 199, SRv6 SID fcbb:0:1058:e017::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.59.225.0/24 [200/0]
           via fcbb::/36, SRv6 Transport tunnel index 213, SRv6 SID fcbb:0:59:e017::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.102.225.0/24 [200/0]
           via fcbb:0:1302::/48, SRv6 Transport tunnel index 212, SRv6 SID fcbb:0:1302:e000::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.107.225.0/24 [200/0]
           via fcbb::/36, SRv6 Transport tunnel index 213, SRv6 SID fcbb:0:307:e000::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.110.225.0/24 [200/0]
           via fcbb:0:1310::/48, SRv6 Transport tunnel index 215, SRv6 SID fcbb:0:1310:e000::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.116.225.0/24 [200/0]
           via fcbb::/36, SRv6 Transport tunnel index 213, SRv6 SID fcbb:0:316:e002::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.136.225.0/24 [200/0]
           via fcbb::/36, SRv6 Transport tunnel index 213, SRv6 SID fcbb:0:336:e664::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.138.225.0/24 [200/0]
           via fcbb:0:1338::/48, SRv6 Transport tunnel index 216, SRv6 SID fcbb:0:1338:e666::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.142.225.0/24 [200/0]
           via fcbb::/36, SRv6 Transport tunnel index 213, SRv6 SID fcbb:0:342:e002::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.144.225.0/24 [200/0]
           via fcbb:0:1344::/48, SRv6 Transport tunnel index 15, SRv6 SID fcbb:0:1344:e001::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.152.225.0/24 [200/0]
           via fcbb::/36, SRv6 Transport tunnel index 213, SRv6 SID fcbb:0:352:e002::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.153.225.0/24 [200/0]
           via fcbb:0:1353::/48, SRv6 Transport tunnel index 131, SRv6 SID fcbb:0:1353:e003::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.161.225.0/24 [200/0]
           via fcbb::/36, SRv6 Transport tunnel index 213, SRv6 SID fcbb:0:161:400::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 C        20.162.225.0/24 [0/0]
           via Vlan20, directly connected
 B I      20.199.225.0/24 [200/0]
           via fcbb:0:1199::/48, SRv6 Transport tunnel index 55, SRv6 SID fcbb:0:1199:e1b7::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10
 B I      20.219.225.0/24 [200/0]
           via fcbb::/36, SRv6 Transport tunnel index 213, SRv6 SID fcbb:0:419:e0b1::
              via fe80::f24b:3aff:fe21:9e0f, Ethernet10

```

## show isis database detail

```text

IS-IS Instance: srv6 VRF: default
  IS-IS Level 1 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS Flags
    CIEN-11-5169.00-00          618   6647   381    529 L1 <>
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
    h3c_29_S12500R-2L.00-00       282   8128  1005    430 L1 <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: h3c_29_S12500R-2L
      Area addresses: 49.0001
      Interface address: 2001:0:29:58::29
      Interface address: 2001:0:29:338::29
      Interface address: 2002::29
      IS Neighbor          : ZTE_338_ZXR10_M6000-4SE.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:29:338::338
        Global IPv6 Interface Address: 2001:0:29:338::29
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:29:58::58
        Global IPv6 Interface Address: 2001:0:29:58::29
      Reachability          : 2001:0:29:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:29:338::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::29/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:1029::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:1029::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1029::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 0
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
    Ericsson_6676_49.00-00       302  49921   382    486 L1 <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Ericsson_6676_49
      Area addresses: 49.0001
      Interface address: 10.0.0.49
      Interface address: 2002::49
      IS Neighbor          : huawei_199.00       Metric: 10
        IPv4 Interface Address: 20.49.199.49
        IPv6 Neighbor Address: 2001:0:49:199::199
        Global IPv6 Interface Address: 2001:0:49:199::49
      IS Neighbor          : ZTE_338_ZXR10_M6000-4SE.00 Metric: 10
        IPv4 Interface Address: 21.38.49.49
        IPv6 Neighbor Address: 2001:0:49:338::338
        Global IPv6 Interface Address: 2001:0:49:338::49
      Reachability         : 10.0.0.49/32 Metric: 10 Type: 1 Up
      Reachability         : 20.49.199.0/24 Metric: 10 Type: 1 Up
      Reachability         : 21.38.49.0/24 Metric: 10 Type: 1 Up
      Reachability          : 2002::49/128 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:49:338::/64 Metric: 10 Type: 1 Up
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
    anet-162-R3.00-00           237   4403   476    250 L1 <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 176 s
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
    huawei_199.00-00            281  54689  1015    694 L1 <>
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
    JNPR-302-MX204.00-00        245  52850  1189    351 L1 <>
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
    JNPR-310-ACX7100-48L.00-00       812  61710   985    404 L2 <DefaultAtt>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0x8E(IPv6)
      Hostname: JNPR-310-ACX7100-48L
      Area addresses: 49.0001
      Interface address: 10.0.1.10
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::58
        Global IPv6 Interface Address: 2001:0:58:310::310
      IS Neighbor          : CIEN-11-5169.00     Metric: 10
        IPv6 Neighbor Address: 2001:0:11:310::11
        Global IPv6 Interface Address: 2001:0:11:310::310
      IS Neighbor          : Cisco353-8201-24H8FH.00 Metric: 10
        Global IPv6 Interface Address: 2001:0:310:353::353
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
    ZTE_338_ZXR10_M6000-4SE.00-00       341  55803   370    499 L2 <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: ZTE_338_ZXR10_M6000-4SE
      Area addresses: 49.0001
      Interface address: 10.0.1.38
      Interface address: 2002::338
      IS Neighbor          : h3c_29_S12500R-2L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:29:338::29
        Global IPv6 Interface Address: 2001:0:29:338::338
      IS Neighbor          : Ericsson_6676_49.00 Metric: 10
        IPv4 Neighbor Address: 21.38.49.49
        IPv4 Interface Address: 21.38.49.38
        IPv6 Neighbor Address: 2001:0:49:338::49
        Global IPv6 Interface Address: 2001:0:49:338::338
        Adj-sid: 965536 flags: [L V] weight: 0x0
      Reachability         : 10.0.1.38/32 Metric: 10 Type: 1 Up
      Reachability         : 21.38.49.0/24 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:29:338::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:49:338::/64 Metric: 10 Type: 1 Up
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
    Cisco344-N57B1.00-00        232  64087   531    418 L1 <>
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
    Cisco353-8201-24H8FH.00-00       893   9376   334    767 L2 <DefaultAtt>
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
      Reachability          : 2001:0:28:336::/64 Metric: 60 Type: 1 Down
      Reachability          : 2001:0:59:352::/64 Metric: 30 Type: 1 Down
      Reachability          : 2001:0:302:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:307:352::/64 Metric: 20 Type: 1 Down
      Reachability          : 2001:0:307:353::/64 Metric: 10 Type: 1 Down
      Reachability          : 2002::/71 Metric: 10 Type: 1 Down
      Reachability          : 2002::353/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb::/36 Metric: 10 Type: 1 Down
      Reachability          : fcbb:0:1353::/48 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:20:36::/64 Metric: 40 Type: 1 Down
      Reachability          : 2001:0:59:161::/64 Metric: 40 Type: 1 Down
      Reachability          : 2001:1:20:36::/64 Metric: 50 Type: 1 Down
      Reachability          : 2001:1:59:352::/64 Metric: 40 Type: 1 Down
      Reachability          : 2001:0:11:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:20:336::/64 Metric: 60 Type: 1 Down
      Reachability          : 2001:0:28:316::/64 Metric: 70 Type: 1 Down
      Reachability          : 2001:0:161:342::/64 Metric: 50 Type: 1 Down
      Reachability          : 2001:0:316:342::/64 Metric: 60 Type: 1 Down
      SRv6 Locator: fcbb::/36 Topology: 0
        Metric: 10 Algorithm: 0 Flags: [D]
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
    Nokia_58-SR1-3-SRv6.00-00       367  32411 65519    463 L2 <DefaultAtt>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia_58-SR1-3-SRv6
      Area addresses:
        49.0000
        49.0001
      Interface address: 10.0.0.58
      Interface address: 2001:0:29:58::58
      Interface address: 2001:0:36:58::58
      Interface address: 2001:0:58:310::58
      Interface address: 2001:0:58:419::58
      Interface address: 2002::58
      IS Neighbor          : h3c_29_S12500R-2L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:29:58::29
        Global IPv6 Interface Address: 2001:0:29:58::58
      Reachability         : 10.0.0.58/32 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:29:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::58/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.58 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0
    Nokia_58-SR1-3-SRv6.00-02        43  12491 65519    467 L2 <>
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::310
        Global IPv6 Interface Address: 2001:0:58:310::58
      IS Neighbor          : Keys-Ixia-419.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:58:419::419
        Global IPv6 Interface Address: 2001:0:58:419::58
      Reachability          : fcbb:0:1058::/48 Metric: 0 Type: 1 Up
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
    Keys-Ixia-419.00-00         168  60522  1196    351 L2 <DefaultAtt>
      Remaining lifetime received: 1198 s Modified to: 1200 s
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

