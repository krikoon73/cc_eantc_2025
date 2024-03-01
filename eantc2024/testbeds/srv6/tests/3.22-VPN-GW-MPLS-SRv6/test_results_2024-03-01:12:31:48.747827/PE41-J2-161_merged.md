# Test results for PE41-J2-161

## show interfaces status

```text
Port       Name                                                Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1                                                            notconnect   routed   full   25G    Not Present                    
Et2                                                            notconnect   1        full   25G    Not Present                    
Et3                                                            notconnect   1        full   25G    Not Present                    
Et4                                                            notconnect   1        full   25G    Not Present                    
Et5                                                            connected    routed   full   10G    10GBASE-SR                     
Et6                                                            notconnect   1        full   25G    Not Present                    
Et7                                                            notconnect   1        full   25G    Not Present                    
Et8                                                            notconnect   1        full   25G    Not Present                    
Et9                                                            notconnect   1        full   25G    Not Present                    
Et10       "Link to Cisco .342 SNAKE TEST RIGHT ANTICLOCKWISE" connected    routed   full   10G    10GBASE-SR                     
Et11                                                           connected    trunk    full   10G    10GBASE-LR                     
Et12                                                           notconnect   1        full   25G    Not Present                    
Et13                                                           notconnect   1        full   25G    Not Present                    
Et14                                                           notconnect   1        full   25G    Not Present                    
Et15                                                           notconnect   1        full   25G    Not Present                    
Et16                                                           notconnect   1        full   25G    Not Present                    
Et17                                                           notconnect   1        full   25G    Not Present                    
Et18                                                           notconnect   1        full   25G    Not Present                    
Et19                                                           notconnect   1        full   25G    Not Present                    
Et20       "Link to Nokia .59 SNAKE TEST LEFT CLOCKWISE"       connected    routed   full   10G    10GBASE-SRL                    
Et21                                                           notconnect   1        full   25G    Not Present                    
Et22                                                           notconnect   1        full   25G    Not Present                    
Et23                                                           notconnect   1        full   25G    Not Present                    
Et24                                                           notconnect   1        full   25G    Not Present                    
Et25                                                           notconnect   1        full   25G    Not Present                    
Et26                                                           notconnect   1        full   25G    Not Present                    
Et27                                                           notconnect   1        full   25G    Not Present                    
Et28                                                           notconnect   1        full   25G    Not Present                    
Et29                                                           notconnect   1        full   25G    Not Present                    
Et30                                                           notconnect   1        full   25G    Not Present                    
Et31                                                           notconnect   1        full   25G    Not Present                    
Et32                                                           notconnect   1        full   25G    Not Present                    
Et33                                                           notconnect   1        full   25G    Not Present                    
Et34                                                           notconnect   1        full   25G    Not Present                    
Et35                                                           notconnect   1        full   25G    Not Present                    
Et36                                                           notconnect   1        full   25G    Not Present                    
Et37                                                           errdisabled  1        full   25G    Not Present                    
Et38                                                           errdisabled  1        full   25G    Not Present                    
Et39                                                           notconnect   1        full   10G    10GBASE-SRL                    
Et40                                                           notconnect   1        full   10G    10GBASE-SRL                    
Et41/1                                                         notconnect   1        full   100G   Not Present                    
Et42/1                                                         notconnect   1        full   100G   Not Present                    
Et43/1                                                         notconnect   1        full   100G   Not Present                    
Et44/1                                                         notconnect   1        full   100G   Not Present                    
Et45/1     Spine2-J-180                                        connected    routed   full   40G    40GBASE-SR4                    
Et46/1                                                         notconnect   1        full   40G    Not Present                    
Ma1                                                            connected    routed   a-full a-1G   10/100/1000                    

```

## show interfaces ethernet 45/1,20 | grep rate

```text
  5 seconds input rate 20.2 kbps (0.0% with framing overhead), 22 packets/sec
  5 seconds output rate 44.7 kbps (0.0% with framing overhead), 33 packets/sec
  5 seconds input rate 9.70 kbps (0.0% with framing overhead), 3 packets/sec
  5 seconds output rate 10.5 kbps (0.0% with framing overhead), 3 packets/sec
```

## show lldp neighbors

```text
Last table change time   : 21:02:15 ago
Number of table inserts  : 12
Number of table deletes  : 7
Number of table drops    : 0
Number of table age-outs : 0

Port            Neighbor Device ID             Neighbor Port ID    TTL
------------ ------------------------------ ---------------------- ---
Et10            Cisco342-9902                  TenGigE0/0/0/12     120
Et11            JNPR-398-QFX5120               546                 120
Et20            Nokia-59-IXRe2                 1610899777          121
Et45/1          Spine2-J-180.ns.eantc.de       Ethernet54/1        120
Ma1             extreme-x460-1                 42                  120

```

## show isis neighbors

```text
! IS-IS (sr_eantc) is shutdown
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
srv6      default  Cisco342-9902    L2   Ethernet10         P2P               UP    29          00                  
srv6      default  Spine2-J-180     L2   Ethernet45/1       P2P               UP    23          60                  
srv6      default  Nokia-59-IXRe2   L2   Ethernet20         P2P               UP    21          00                  
```

## show isis database detail

```text
! IS-IS (sr_eantc) is shutdown
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: sr_eantc VRF: default
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: srv6 VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    CIEN-5169-3.00-00            49  58026 55647    203 L2  0000.0000.0003.00-00  <>
      NLPID: 0xCC(IPv4)
      Hostname: CIEN-5169-3
      Area addresses: 49.0001
      Interface address: 100.0.0.3
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 20.3.180.180
        IPv4 Interface Address: 20.3.180.3
        Adj-sid: 16000 flags: [L V] weight: 0x0
      Reachability         : 100.0.0.3/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 3 Flags: [N] Algorithm: 0
      Reachability         : 20.3.180.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 100.0.0.3 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    CIEN-11-5169.00-00          168  22878   646   1173 L2  0000.0000.0011.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: CIEN-11-5169
      Area addresses: 49.0001
      Interface address: 2001:0:11:310::11
      IS Neighbor          : Cisco353-8201-24H8FH.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:11:353::353
        Global IPv6 Interface Address: 2001:0:11:353::11
        Adj-sid: 24000 flags: [L V F] weight: 0x0
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:11:310::310
        Global IPv6 Interface Address: 2001:0:11:310::11
        Adj-sid: 24001 flags: [L V F] weight: 0x0
      Reachability         : 10.0.0.11/32 Metric: 0 Type: 1 Up
      Reachability          : 2002::11/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:11:353::/64 Metric: 10 Type: 1 Up
      Reachability          : fcbb:1:1011::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1011::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:2:1011::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:3:1011::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1000::/36 Metric: 20 Type: 1 Up
      Reachability          : 2002::29/128 Metric: 30 Type: 1 Up
      Reachability          : fcbb:0:1000::/48 Metric: 10 Type: 1 Up
      Reachability          : 2002::49/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::58/128 Metric: 20 Type: 1 Up
      Reachability          : 2002::199/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::302/128 Metric: 20 Type: 1 Up
      Reachability          : 2002::310/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::344/128 Metric: 50 Type: 1 Up
      Reachability          : 2002::353/128 Metric: 20 Type: 1 Up
      Reachability          : 2002::419/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::302/128 Metric: 20 Type: 1 Up
      SRv6 Locator: fcbb:1:1011::/48 Topology: 0
        Metric: 0 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:1011::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:0:1011::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1011::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:0:1000::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1000::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:2:1011::/48 Topology: 0
        Metric: 0 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:2:1011::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:3:1011::/48 Topology: 0
        Metric: 0 Algorithm: 130 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:3:1011::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      Router Capabilities: Router Id: 10.0.0.11 Flags: []
        SRv6 Capability: Flags: []
        SR Capability: Flags: [V]
          SRGB Base: 16000 Range: 8000
        Algorithms:  0, 128, 129, 130
    h3c_20_CR16010E-F.00-00      7331  51420  1105   1336 L2  0000.0000.0020.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: h3c_20_CR16010E-F
      Area addresses: 49.0000
      Interface address: 2001:0:20:36::20
      Interface address: 2001:0:20:316::20
      Interface address: 2001:0:20:336::20
      Interface address: 2002::20
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:20:36::36
        Global IPv6 Interface Address: 2001:0:20:36::20
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:20:36::36
        Global IPv6 Interface Address: 2001:0:20:36::20
      IS Neighbor          : JNPR-316-MX304.00   Metric: 10
        IPv6 Neighbor Address: 2001:0:20:316::316
        Global IPv6 Interface Address: 2001:0:20:316::20
      IS Neighbor          : ZTE_336_ZXR10_M6000-8SE.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:336::336
        Global IPv6 Interface Address: 2001:0:20:336::20
      IS Neighbor          : ZTE_336_ZXR10_M6000-8SE.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:336::336
        Global IPv6 Interface Address: 2001:0:20:336::20
      Reachability          : 2001:0:20:36::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:20:316::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:20:336::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::20/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:20::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:20::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:20::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 0
        SRv6 SID End
          SID : fcbb:0:20:e112::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP USP USD
          SID : fcbb:0:20:e113::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
    0000.0000.0021.00-00       2895  25398  1197    128 L2  0000.0000.0021.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 20.21.180.21
      Interface address: 100.0.0.21
      IS Neighbor          : Spine2-J-180.00     Metric: 10
      Reachability         : 20.21.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 100.0.0.21/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 21 Flags: [N] Algorithm: 0
      Reachability         : 192.168.20.0/23 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 100.0.0.21 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  13
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    h3c_26_S12500R-2L.00-00       538   8709  1071    139 L2  0000.0000.0026.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: h3c_26_S12500R-2L
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 20.26.180.26
      Interface address: 100.0.0.26
      IS Neighbor          : Spine2-J-180.00     Metric: 10
      Reachability         : 20.26.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 100.0.0.26/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 26 Flags: [N P] Algorithm: 0
      Router Capabilities: Router Id: 100.0.0.26 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    h3c_28_S12500R-2L.00-00      3159  56560  1160    833 L2  0000.0000.0028.00-00  <>
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
      IS Neighbor          : ZTE_336_ZXR10_M6000-8SE.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:28:336::336
        Global IPv6 Interface Address: 2001:0:28:336::28
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
        Algorithms:  0, 128, 129
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 100
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 100
          Flags: [M] 0x80
    Huawei-34.00-00           12312   2416  1192    139 L2  0000.0000.0034.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Huawei-34
      Area addresses: 49.0001
      Interface address: 100.0.0.34
      Interface address: 20.34.180.34
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 20.34.180.180
        IPv4 Interface Address: 20.34.180.34
        Adj-sid: 48000 flags: [L V] weight: 0x0
      Reachability         : 100.0.0.34/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 34 Flags: [N] Algorithm: 0
      Reachability         : 20.34.180.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 100.0.0.34 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    huawei_36.00-00           12446  49180  1192    783 L2  0000.0000.0036.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: huawei_36
      Area addresses: 49.0000
      Topology: 0 (IPv4)
      Interface address: 2002::36
      Interface address: 2001:0:36:310::36
      Interface address: 2001:0:36:58::36
      Interface address: 2001:0:20:36::36
      Reachability          : 2002::36/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:36::/48 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:36:310::/64 Metric: 10 Type: 1 Up
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
      SRv6 Locator: fcbb:3:36::/48 Topology: 0
        Metric: 0 Algorithm: 130 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:3:36::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
        SRv6 SID Un Supported
          SID : fcbb:3:36:e005::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 64
        SRv6 SID End
          SID : fcbb:3:36:e006::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP
          SID : fcbb:3:36:e007::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP USP USD
          SID : fcbb:3:36:e008::
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
    huawei_36.00-01            1121  40890  1033   1044 L2  0000.0000.0036.00-01  <>
      IS Neighbor          : h3c_20_CR16010E-F.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:36::20
        Global IPv6 Interface Address: 2001:0:20:36::36
      IS Neighbor          : h3c_20_CR16010E-F.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:36::20
        Global IPv6 Interface Address: 2001:0:20:36::36
      IS Neighbor          : h3c_20_CR16010E-F.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:36::20
        Global IPv6 Interface Address: 2001:0:20:36::36
      IS Neighbor          : h3c_20_CR16010E-F.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:36::20
        Global IPv6 Interface Address: 2001:0:20:36::36
      SRv6 Locator: fcbb:2:36::/48 Topology: 0
        Metric: 0 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:2:36::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
        SRv6 SID Un Supported
          SID : fcbb:2:36:e005::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 64
        SRv6 SID End
          SID : fcbb:2:36:e006::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP
          SID : fcbb:2:36:e007::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP USP USD
          SID : fcbb:2:36:e008::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
    huawei_36.00-02             119  13765  1033    883 L2  0000.0000.0036.00-02  <>
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:36:58::58
        Global IPv6 Interface Address: 2001:0:36:58::36
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:36:58::58
        Global IPv6 Interface Address: 2001:0:36:58::36
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:36:58::58
        Global IPv6 Interface Address: 2001:0:36:58::36
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:36:58::58
        Global IPv6 Interface Address: 2001:0:36:58::36
    huawei_36.00-03             116  40772  1033    883 L2  0000.0000.0036.00-03  <>
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:36:310::310
        Global IPv6 Interface Address: 2001:0:36:310::36
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:36:310::310
        Global IPv6 Interface Address: 2001:0:36:310::36
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:36:310::310
        Global IPv6 Interface Address: 2001:0:36:310::36
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:36:310::310
        Global IPv6 Interface Address: 2001:0:36:310::36
    anet-161-R3.00-00          1390  48997  1194    387 L2  0000.0000.0161.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 894 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: anet-161-R3
      Area addresses: 49.0000
      Interface address: 20.59.161.161
      Interface address: 20.161.180.161
      Interface address: 100.0.0.161
      Interface address: 2001:0:56:161::161
      Interface address: 2001:0:59:161::161
      Interface address: 2001:0:161:342::161
      Interface address: 2002::161
      IS Neighbor          : Nokia-59-IXRe2.00   Metric: 10
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 20.161.180.180
        IPv4 Interface Address: 20.161.180.161
        Adj-sid: 378544 flags: [L V] weight: 0x0
      IS Neighbor          : Cisco342-9902.00    Metric: 10
      Reachability         : 20.59.161.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.161.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 100.0.0.161/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 161 Flags: [N] Algorithm: 0
      Reachability          : fcbb:0:161::/48 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:56:161::/64 Metric: 10 Type: 1 Up
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
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SRv6 Capability: Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
    JNPR-307-ACX7024.00-00      3352   2764  1163    620 L2  0000.0000.0307.00-00  <>
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
      Reachability          : 2001:0:307:353::/64 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:307::/48 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:607::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:307::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:1:307::/48 Topology: 0
        Metric: 0 Algorithm: 128 Flags: []
      SRv6 Locator: fcbb:2:307::/48 Topology: 0
        Metric: 0 Algorithm: 129 Flags: []
      SRv6 Locator: fcbb:3:307::/48 Topology: 0
        Metric: 0 Algorithm: 130 Flags: []
      SRv6 Locator: fcbb:0:607::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:0:607::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.1.7 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1, 128, 129, 130
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 0
          Exclude admin groups: 1
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 0
      Unsupported TLV: Type: 14 Length: 2
    JNPR-310-ACX7100-48L.00-00     55740  59576  1195   1216 L2  0000.0000.0310.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: JNPR-310-ACX7100-48L
      Area addresses: 49.0001
      Interface address: 10.0.1.10
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:36:310::36
        Global IPv6 Interface Address: 2001:0:36:310::310
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::58
        Global IPv6 Interface Address: 2001:0:58:310::310
      IS Neighbor          : Cisco353-8201-24H8FH.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:310:353::353
        Global IPv6 Interface Address: 2001:0:310:353::353
      IS Neighbor          : CIEN-11-5169.00     Metric: 10
        IPv6 Neighbor Address: 2001:0:11:310::11
        Global IPv6 Interface Address: 2001:0:11:310::310
      Reachability          : 2002::310/128 Metric: 0 Type: 1 Up
      Reachability          : 2002::/72 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:310:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:25:110:225::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:36:310::/64 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1310::/48 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:1610::/48 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:1000::/36 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:310:338::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:2:1310::/48 Topology: 0
        Metric: 0 Algorithm: 129 Flags: []
      SRv6 Locator: fcbb:3:1310::/48 Topology: 0
        Metric: 0 Algorithm: 130 Flags: []
      SRv6 Locator: fcbb:0:1310::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:1:1310::/48 Topology: 0
        Metric: 0 Algorithm: 128 Flags: []
      SRv6 Locator: fcbb:0:1610::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:0:1610::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:0:1000::/36 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:1:1000::/36 Topology: 0
        Metric: 10 Algorithm: 128 Flags: []
      SRv6 Locator: fcbb:1:1000::/36 Topology: 0
        Metric: 10 Algorithm: 128 Flags: []
      SRv6 Locator: fcbb:1:1000::/36 Topology: 0
        Metric: 10 Algorithm: 128 Flags: []
      SRv6 Locator: fcbb:1:1000::/36 Topology: 0
        Metric: 10 Algorithm: 128 Flags: []
      SRv6 Locator: fcbb:1:1000::/36 Topology: 0
        Metric: 10 Algorithm: 128 Flags: []
      SRv6 Locator: fcbb:1:1000::/36 Topology: 0
        Metric: 10 Algorithm: 128 Flags: []
      SRv6 Locator: fcbb:1:1000::/36 Topology: 0
        Metric: 10 Algorithm: 128 Flags: []
      SRv6 Locator: fcbb:1:1000::/36 Topology: 0
        Metric: 10 Algorithm: 128 Flags: []
      SRv6 Locator: fcbb:1:1000::/36 Topology: 0
        Metric: 10 Algorithm: 128 Flags: []
      SRv6 Locator: fcbb:1:1000::/36 Topology: 0
        Metric: 10 Algorithm: 128 Flags: []
      Router Capabilities: Router Id: 10.0.1.10 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1, 128, 129, 130
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 0
          Exclude admin groups: 1
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 0
      Unsupported TLV: Type: 14 Length: 2
    JNPR-316-MX304.00-00       2198  62933  1006    838 L2  0000.0000.0316.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: JNPR-316-MX304
      Area addresses: 49.0000
      Interface address: 10.0.1.16
      IS Neighbor          : h3c_28_S12500R-2L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:28:316::28
        Global IPv6 Interface Address: 2001:0:28:316::316
      IS Neighbor          : h3c_20_CR16010E-F.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:316::20
        Global IPv6 Interface Address: 2001:0:20:316::316
      IS Neighbor          : Cisco342-9902.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:316:342::342
        Global IPv6 Interface Address: 2001:0:316:342::316
      Reachability          : 2002::316/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:316:342::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:28:316::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:20:316::/64 Metric: 10 Type: 1 Up
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
      Router Capabilities: Router Id: 10.0.1.16 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1, 128, 129, 130
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 0
          Exclude admin groups: 1
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 0
      Unsupported TLV: Type: 14 Length: 2
    ZTE_336_ZXR10_M6000-8SE.00-00      7269  16677  1175   1234 L2  0000.0000.0336.00-00  <>
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
    h41-9902.00-00            44933  56362   786    176 L2  0000.0000.0341.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: h41-9902
      Area addresses: 49.0001
      Interface address: 100.0.3.41
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 30.41.180.180
        IPv4 Interface Address: 30.41.180.41
        Adj-sid: 24004 flags: [L V] weight: 0x0
      Reachability         : 30.41.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 100.0.3.41/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 341 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 100.0.3.41 Flags: []
        SR Local Block:
          SRLB Base: 15000 Range: 1000
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Cisco342-9902.00-00         623  18473  1154    637 L2  0000.0000.0342.00-00  <>
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
      SRv6 Locator: fcbb:2:342::/48 Topology: 0
        Metric: 1 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:2:342::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0, 1, 128, 129
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 128
      Unsupported TLV: Type: 14 Length: 2
    h45-N57C1.00-00             474  49182   532    177 L2  0000.0000.0345.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: h45-N57C1
      Area addresses: 49.0001
      Interface address: 100.0.3.45
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 30.45.180.180
        IPv4 Interface Address: 30.45.180.45
        Adj-sid: 28103 flags: [L V] weight: 0x0
      Reachability         : 30.45.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 100.0.3.45/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 345 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 100.0.3.45 Flags: []
        SR Local Block:
          SRLB Base: 15000 Range: 1000
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    h48-N540-24Q8L2DD.00-00       478  26284   753    185 L2  0000.0000.0348.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: h48-N540-24Q8L2DD
      Area addresses: 49.0001
      Interface address: 100.0.3.48
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 30.48.180.180
        IPv4 Interface Address: 30.48.180.48
        Adj-sid: 25503 flags: [L V] weight: 0x0
      Reachability         : 30.48.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 100.0.3.48/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 348 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 100.0.3.48 Flags: []
        SR Local Block:
          SRLB Base: 15000 Range: 1000
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Cisco352-N540.00-00         574  33775   482    904 L2  0000.0000.0352.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: Cisco352-N540
      Area addresses: 49.0001
      Interface address: 2002::352
      IS Neighbor          : h3c_28_S12500R-2L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:28:352::28
        Global IPv6 Interface Address: 2001:0:28:352::352
      IS Neighbor          : JNPR-307-ACX7024.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:307:352::307
        Global IPv6 Interface Address: 2001:0:307:352::352
      IS Neighbor          : Nokia-59-IXRe2.00   Metric: 10
        IPv6 Neighbor Address: 2001:0:59:352::59
        Global IPv6 Interface Address: 2001:0:59:352::352
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
      SRv6 Locator: fcbb:2:352::/48 Topology: 0
        Metric: 1 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:2:352::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0, 1, 128, 129
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 128
      Unsupported TLV: Type: 14 Length: 2
    Cisco353-8201-24H8FH.00-00     17525  37169  1192   1241 L2  0000.0000.0353.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: Cisco353-8201-24H8FH
      Area addresses:
        49.0000
        49.0001
      Interface address: 2002::353
      IS Neighbor          : CIEN-11-5169.00     Metric: 10
        IPv6 Neighbor Address: 2001:0:11:353::11
        Global IPv6 Interface Address: 2001:0:11:353::353
      Reachability          : 2001:0:29:58::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:29:338::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:199:302::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:199:344::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:307:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:310:338::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:310:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::/72 Metric: 10 Type: 1 Up
      Reachability          : 2002::353/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1000::/36 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1353::/48 Metric: 1 Type: 1 Up
      Reachability          : fcbb:1:1000::/36 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:11:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:36:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:49:338::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:302:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:25:110:225::/64 Metric: 20 Type: 1 Up
      Reachability          : fcbb::/48 Metric: 20 Type: 1 Up
      Reachability          : 2001:1000:302:353::/64 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:419::/64 Metric: 40 Type: 1 Up
      SRv6 Locator: fcbb::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1000::/36 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:0:1353::/48 Topology: 0
        Metric: 1 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:1353::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:1:1000::/36 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:2:1058::/48 Topology: 0
        Metric: 22 Algorithm: 129 Flags: []
      SRv6 Locator: fcbb:2:1302::/48 Topology: 0
        Metric: 11 Algorithm: 129 Flags: []
      SRv6 Locator: fcbb:5:1302::/48 Topology: 0
        Metric: 10 Algorithm: 132 Flags: []
      SRv6 Locator: fcbb:5:1353::/48 Topology: 0
        Metric: 1 Algorithm: 132 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:5:1353::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:6:1302::/48 Topology: 0
        Metric: 10 Algorithm: 133 Flags: []
      SRv6 Locator: fcbb:6:1353::/48 Topology: 0
        Metric: 1 Algorithm: 133 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:6:1353::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:2:1310::/48 Topology: 0
        Metric: 11 Algorithm: 129 Flags: []
      SRv6 Locator: fcbb:2:1338::/48 Topology: 0
        Metric: 22 Algorithm: 129 Flags: []
      SRv6 Locator: fcbb:3:1011::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:7:1302::/48 Topology: 0
        Metric: 10 Algorithm: 134 Flags: []
      SRv6 Locator: fcbb:7:1353::/48 Topology: 0
        Metric: 1 Algorithm: 134 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:7:1353::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0, 1, 128, 129, 132, 133, 134
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 128
        Flex Algo: Algorithm: 132 Metric: IGP Metric (0) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 133 Metric: IGP Metric (0) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 134 Metric: IGP Metric (0) Calc: SPF (0) Prio: 128
      Unsupported TLV: Type: 14 Length: 2
    Cisco353-8201-24H8FH.00-01      3398  40636   434    568 L2  0000.0000.0353.00-01  <>
      IS Neighbor          : JNPR-307-ACX7024.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:307:353::307
        Global IPv6 Interface Address: 2001:0:307:353::353
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:310:353::353
        Global IPv6 Interface Address: 2001:0:310:353::353
      Reachability          : 2001:25:58:225::/64 Metric: 20 Type: 1 Up
      Reachability          : fcbb:2:1011::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:3:1011::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:3:1058::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:4:1058::/48 Metric: 20 Type: 1 Up
      SRv6 Locator: fcbb:2:1011::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
    evpn-rr-58.00-00            473  41000   811    178 L2  0000.0000.0358.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: evpn-rr-58
      Area addresses: 49.0001
      Interface address: 100.0.3.58
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 30.58.180.180
        IPv4 Interface Address: 30.58.180.58
        Adj-sid: 24001 flags: [L V] weight: 0x0
      Reachability         : 30.58.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 100.0.3.58/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 358 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 100.0.3.58 Flags: []
        SR Local Block:
          SRLB Base: 15000 Range: 1000
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 16000 Range: 8000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    evpn-rr2-60.00-00           469  50924   742    179 L2  0000.0000.0360.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: evpn-rr2-60
      Area addresses: 49.0001
      Interface address: 100.0.3.60
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 30.60.180.180
        IPv4 Interface Address: 30.60.180.60
        Adj-sid: 24001 flags: [L V] weight: 0x0
      Reachability         : 30.60.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 100.0.3.60/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 360 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 100.0.3.60 Flags: []
        SR Local Block:
          SRLB Base: 15000 Range: 1000
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 16000 Range: 8000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    h41-9902.00-00               11  27916   986    265 L2  0000.0000.3341.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: h41-9902
      Area addresses: 49.0002
      Interface address: 2001::41
      IS Neighbor          : SR1-EVPN.00         Metric: 10
      Reachability          : 2001::41/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:341::/48 Metric: 1 Type: 1 Up
      SRv6 Locator: fcbb:0:341::/48 Topology: 0
        Metric: 1 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:341::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Ribbon_31.00-00             462  32116   917     79 L2  0001.0000.0031.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Area addresses: 49.0001
      Router Capabilities: Router Id: 100.0.0.31 Flags: []
        SR Local Block:
          SRLB Base: 16 Range: 15344
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
      Unsupported TLV: Type: 14 Length: 2
    Ribbon_31.00-01             461  58975   493     38 L2  0001.0000.0031.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      Hostname: Ribbon_31
    Ribbon_31.00-02             464  47907   743    108 L2  0001.0000.0031.00-02  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      Interface address: 100.0.0.31
      Interface address: 20.31.180.31
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 20.31.180.180
        IPv4 Interface Address: 20.31.180.31
        Adj-sid: 756640 flags: [L V] weight: 0x0
        Adj-sid: 756641 flags: [L V B] weight: 0x0
      Reachability         : 100.0.0.31/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 31 Flags: [N] Algorithm: 0
      Reachability         : 20.31.180.0/24 Metric: 10 Type: 1 Up
    Spine2-J-180.00-00          895  20104  1182    872 L2  0001.0001.0180.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Spine2-J-180
      Area addresses: 49.0001
      Interface address: 30.41.180.180
      Interface address: 20.3.180.180
      Interface address: 20.31.180.180
      Interface address: 20.21.180.180
      Interface address: 30.14.180.180
      Interface address: 30.48.180.180
      Interface address: 20.180.182.180
      Interface address: 20.180.184.180
      Interface address: 20.180.183.180
      Interface address: 20.34.180.180
      Interface address: 20.161.180.180
      Interface address: 30.79.180.180
      Interface address: 20.180.181.180
      Interface address: 30.9.180.180
      Interface address: 20.56.180.180
      Interface address: 20.26.180.180
      Interface address: 30.45.180.180
      Interface address: 30.60.180.180
      Interface address: 30.58.180.180
      IS Neighbor          : SR1-EVPN.00         Metric: 10
        IPv4 Neighbor Address: 20.56.180.56
        IPv4 Interface Address: 20.56.180.180
        Adj-sid: 100016 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0021.00   Metric: 10
        IPv4 Neighbor Address: 20.21.180.21
        IPv4 Interface Address: 20.21.180.180
        Adj-sid: 100009 flags: [L V] weight: 0x0
      IS Neighbor          : Ribbon_31.00        Metric: 10
        IPv4 Neighbor Address: 20.31.180.31
        IPv4 Interface Address: 20.31.180.180
        Adj-sid: 100019 flags: [L V] weight: 0x0
      IS Neighbor          : juniper_379_MX304-evpn-mpls.00 Metric: 10
        IPv4 Neighbor Address: 30.79.180.79
        IPv4 Interface Address: 30.79.180.180
        Adj-sid: 100021 flags: [L V] weight: 0x0
      IS Neighbor          : PE42-J2-182.00      Metric: 10
        IPv4 Neighbor Address: 20.180.182.182
        IPv4 Interface Address: 20.180.182.180
        Adj-sid: 100004 flags: [L V] weight: 0x0
      IS Neighbor          : Huawei-34.00        Metric: 10
        IPv4 Neighbor Address: 20.34.180.34
        IPv4 Interface Address: 20.34.180.180
        Adj-sid: 100018 flags: [L V] weight: 0x0
      IS Neighbor          : PE21-J2-181.00      Metric: 10
        IPv4 Neighbor Address: 20.180.181.181
        IPv4 Interface Address: 20.180.181.180
        Adj-sid: 100000 flags: [L V] weight: 0x0
      IS Neighbor          : juniper-309-acx7332.00 Metric: 10
        IPv4 Neighbor Address: 30.9.180.9
        IPv4 Interface Address: 30.9.180.180
        Adj-sid: 100017 flags: [L V] weight: 0x0
      IS Neighbor          : h41-9902.00         Metric: 10
        IPv4 Neighbor Address: 30.41.180.41
        IPv4 Interface Address: 30.41.180.180
        Adj-sid: 100057 flags: [L V] weight: 0x0
      IS Neighbor          : CIEN-5169-3.00      Metric: 10
        IPv4 Neighbor Address: 20.3.180.3
        IPv4 Interface Address: 20.3.180.180
        Adj-sid: 100001 flags: [L V] weight: 0x0
      IS Neighbor          : evpn-rr-58.00       Metric: 10
        IPv4 Neighbor Address: 30.58.180.58
        IPv4 Interface Address: 30.58.180.180
        Adj-sid: 100014 flags: [L V] weight: 0x0
      IS Neighbor          : h48-N540-24Q8L2DD.00 Metric: 10
        IPv4 Neighbor Address: 30.48.180.48
        IPv4 Interface Address: 30.48.180.180
        Adj-sid: 100003 flags: [L V] weight: 0x0
      IS Neighbor          : PE24-J2-184.00      Metric: 10
        IPv4 Neighbor Address: 20.180.184.184
        IPv4 Interface Address: 20.180.184.180
        Adj-sid: 100006 flags: [L V] weight: 0x0
      IS Neighbor          : PE23-J2-183.00      Metric: 10
        IPv4 Neighbor Address: 20.180.183.183
        IPv4 Interface Address: 20.180.183.180
        Adj-sid: 100005 flags: [L V] weight: 0x0
      IS Neighbor          : evpn-rr2-60.00      Metric: 10
        IPv4 Neighbor Address: 30.60.180.60
        IPv4 Interface Address: 30.60.180.180
        Adj-sid: 100015 flags: [L V] weight: 0x0
      IS Neighbor          : h3c_26_S12500R-2L.00 Metric: 10
        IPv4 Neighbor Address: 20.26.180.26
        IPv4 Interface Address: 20.26.180.180
        Adj-sid: 100010 flags: [L V] weight: 0x0
      IS Neighbor          : anet-161-R3.00      Metric: 10
        IPv4 Neighbor Address: 20.161.180.161
        IPv4 Interface Address: 20.161.180.180
        Adj-sid: 100020 flags: [L V] weight: 0x0
      IS Neighbor          : h45-N57C1.00        Metric: 10
        IPv4 Neighbor Address: 30.45.180.45
        IPv4 Interface Address: 30.45.180.180
        Adj-sid: 100002 flags: [L V] weight: 0x0
      Reachability         : 100.0.0.180/32 Metric: 0 Type: 1 Up
      Reachability         : 30.41.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.3.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.31.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.21.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 30.14.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 30.48.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.180.182.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.180.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.180.183.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.34.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.161.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 30.79.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.180.181.0/24 Metric: 10 Type: 1 Up
      Reachability         : 30.9.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.56.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.26.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 30.45.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 30.60.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 30.58.180.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 100.0.0.180 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        SR Capability: Flags: [I]
          SRGB Base: 900000 Range: 65536
    PE21-J2-181.00-00           468  47563  1128    156 L2  0001.0001.0181.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: PE21-J2-181
      Area addresses: 49.0001
      Interface address: 20.180.181.181
      Interface address: 100.0.0.181
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 20.180.181.180
        IPv4 Interface Address: 20.180.181.181
        Adj-sid: 100000 flags: [L V] weight: 0x0
      Reachability         : 20.180.181.0/24 Metric: 10 Type: 1 Up
      Reachability         : 100.0.0.181/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 181 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 100.0.0.201 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  6
        SR Capability: Flags: [I]
          SRGB Base: 900000 Range: 65536
    PE42-J2-182.00-00           489   4480  1156    182 L2  0001.0001.0182.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: PE42-J2-182
      Area addresses: 49.0001
      Interface address: 20.180.182.182
      Interface address: 100.0.0.182
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 20.180.182.180
        IPv4 Interface Address: 20.180.182.182
        Adj-sid: 394912 flags: [L V] weight: 0x0
      Reachability         : 20.30.2.0/24 Metric: 0 Type: 1 Up
      Reachability         : 20.30.3.0/24 Metric: 0 Type: 1 Up
      Reachability         : 20.30.4.0/24 Metric: 0 Type: 1 Up
      Reachability         : 100.0.0.182/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 182 Flags: [N] Algorithm: 0
      Reachability         : 20.180.182.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 100.0.0.182 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    PE23-J2-183.00-00           491  45498   416    156 L2  0001.0001.0183.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: PE23-J2-183
      Area addresses: 49.0001
      Interface address: 20.180.183.183
      Interface address: 100.0.0.183
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 20.180.183.180
        IPv4 Interface Address: 20.180.183.183
        Adj-sid: 100000 flags: [L V] weight: 0x0
      Reachability         : 20.180.183.0/24 Metric: 10 Type: 1 Up
      Reachability         : 100.0.0.183/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 183 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 100.0.0.183 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I]
          SRGB Base: 900000 Range: 65536
    PE24-J2-184.00-00           475  65136  1085    156 L2  0001.0001.0184.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: PE24-J2-184
      Area addresses: 49.0001
      Interface address: 20.180.184.184
      Interface address: 100.0.0.184
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 20.180.184.180
        IPv4 Interface Address: 20.180.184.184
        Adj-sid: 100000 flags: [L V] weight: 0x0
      Reachability         : 20.180.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 100.0.0.184/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 184 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 100.0.0.184 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I]
          SRGB Base: 900000 Range: 65536
    Nokia-59-IXRe2.00-00       6341   1801  1199    632 L2  0002.3124.4180.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-59-IXRe2
      Area addresses: 49.0000.0000.0059.00
      Interface address: 2001:0:59:352::59
      Interface address: 2002::59
      IS Neighbor          : Cisco352-N540.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:59:352::352
        Global IPv6 Interface Address: 2001:0:59:352::59
        Adj-sid: 1048573 flags: [L V B F] weight: 0x0
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
      Router Capabilities: Router Id: 0.231.244.180 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  9
        SRv6 Capability: Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 130, 131
    Nokia_58-SR1-3-SRv6.00-00      1629  13220 57224    274 L2  0100.0000.0058.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia_58-SR1-3-SRv6
      Area addresses:
        49.0000
        49.0001
      Interface address: 10.0.0.58
      Interface address: 2001:0:36:58::58
      Interface address: 2001:0:58:310::58
      Interface address: 2001:0:58:419::58
      Reachability         : 10.0.0.58/32 Metric: 0 Type: 1 Up
      Reachability         : 20.55.2.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.58.225.0/24 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1000::/36 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:1000::/36 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
      Router Capabilities: Router Id: 10.0.0.58 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 128, 129, 130, 131
    Nokia_58-SR1-3-SRv6.00-01      5065  17875 57358    503 L2  0100.0000.0058.00-01  <>
      Interface address: 2002::58
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::310
        Global IPv6 Interface Address: 2001:0:58:310::58
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::310
        Global IPv6 Interface Address: 2001:0:58:310::58
      Reachability          : 2001:0:36:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:199:302::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:0:302:353::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:310:353::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:25:110:225::/64 Metric: 20 Type: 1 Up
      Reachability          : fcbb:1:1058::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:2:1058::/48 Topology: 0
        Metric: 0 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:2:1058::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:3:1310::/48 Topology: 0
        Metric: 10 Algorithm: 130 Flags: []
    Nokia_58-SR1-3-SRv6.00-02      3280  24431 65520    245 L2  0100.0000.0058.00-02  <>
      Reachability         : 10.0.0.57/32 Metric: 10 Type: 1 Down
        SR Prefix-SID: 1957 Flags: [R N P] Algorithm: 0
      Reachability         : 12.0.0.219/32 Metric: 20 Type: 1 Down
      Reachability         : 20.57.10.0/24 Metric: 0 Type: 1 Up
      Reachability         : 20.57.15.0/24 Metric: 20 Type: 1 Down
      Reachability         : 25.36.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.107.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.110.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.152.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.153.225.0/24 Metric: 0 Type: 1 Up
      Reachability          : 2001:25:58:225::/64 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:419::/64 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:419::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:3:1058::/48 Metric: 0 Type: 1 Up
      Reachability          : fcbb:4:1058::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:419::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
        SRv6 SID End with PSP USP
          SID : fcbb:0:419:11::
    Nokia_58-SR1-3-SRv6.00-03     20059  56267 65520   1249 L2  0100.0000.0058.00-03  <>
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:36:58::36
        Global IPv6 Interface Address: 2001:0:36:58::58
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:36:58::36
        Global IPv6 Interface Address: 2001:0:36:58::58
      IS Neighbor          : 6401.0001.0000.00   Metric: 10
        Global IPv6 Interface Address: 2001:0:58:419::58
      IS Neighbor          : 6401.0001.0000.00   Metric: 10
        Global IPv6 Interface Address: 2001:0:58:419::58
      Reachability         : 10.0.0.233/32 Metric: 10 Type: 1 Down
        SR Prefix-SID: 333 Flags: [R N P] Algorithm: 0
      Reachability         : 20.56.2.0/24 Metric: 20 Type: 1 Down
      Reachability         : 20.57.11.0/24 Metric: 0 Type: 1 Up
      Reachability         : 20.57.13.0/24 Metric: 20 Type: 1 Down
      Reachability         : 20.57.14.0/24 Metric: 20 Type: 1 Down
      Reachability         : 25.20.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.102.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.116.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.136.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.138.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.142.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.144.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 100.0.0.0/24 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:11:353::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:29:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:29:338::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:0:49:338::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:199:344::/64 Metric: 50 Type: 1 Up
      Reachability          : 2001:0:310:338::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:1000:302:353::/64 Metric: 30 Type: 1 Up
      Reachability          : 2002::/72 Metric: 10 Type: 1 Up
        Route Tag: 58
      Reachability          : fcbb::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:1:1011::/48 Metric: 30 Type: 1 Up
      SRv6 Locator: fcbb::/48 Topology: 0
        Metric: 20 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:1:1000::/36 Topology: 0
        Metric: 0 Algorithm: 128 Flags: []
      SRv6 Locator: fcbb:2:1011::/48 Topology: 0
        Metric: 22 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:2:1011::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:2:1302::/48 Topology: 0
        Metric: 33 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:2:1302::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:2:1310::/48 Topology: 0
        Metric: 11 Algorithm: 129 Flags: []
      SRv6 Locator: fcbb:2:1338::/48 Topology: 0
        Metric: 22 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:2:1338::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:3:1011::/48 Topology: 0
        Metric: 20 Algorithm: 130 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:3:1011::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:3:1338::/48 Topology: 0
        Metric: 20 Algorithm: 130 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:3:1338::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
    SR1-EVPN.00-00              627  61137   896    502 L2  1000.0000.0056.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: SR1-EVPN
      Area addresses: 49.0002
      Interface address: 20.56.180.56
      Interface address: 100.0.0.56
      Interface address: 2001::56
      Interface address: 2001:0:41:56::56
      Interface address: 2001:0:56:59::56
      IS Neighbor (Narrow metrics, unsupported): Nokia-59-IXRe2.00   Metric: 10
      IS Neighbor (Narrow metrics, unsupported): Spine2-J-180.00     Metric: 10
      IS Neighbor (Narrow metrics, unsupported): h41-9902.00         Metric: 10
      IS Neighbor          : Nokia-59-IXRe2.00   Metric: 10
        Adj-sid: 524258 flags: [L V B F] weight: 0x0
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 20.56.180.180
        IPv4 Interface Address: 20.56.180.56
        Adj-sid: 524257 flags: [L V B] weight: 0x0
      IS Neighbor          : h41-9902.00         Metric: 10
        Adj-sid: 524259 flags: [L V B F] weight: 0x0
      Reachability (Narrow metrics, unsupported): 20.56.180.0/24 Metric: 10 Type: 1
      Reachability (Narrow metrics, unsupported): 100.0.0.56/32 Metric: 0 Type: 1
      Reachability         : 20.56.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 100.0.0.56/32 Metric: 0 Type: 1 Up
      Reachability          : 2001::56/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:41:56::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:56:59::/64 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:56::/48 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 100.0.0.56 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SRv6 Capability: Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    juniper-309-acx7332.00-00       474  41461   631    180 L2  1000.0003.0009.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: juniper-309-acx7332
      Area addresses: 49.0001.0000.0000
      Interface address: 100.0.30.9
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 30.9.180.180
        IPv4 Interface Address: 30.9.180.9
        Adj-sid: 33 flags: [L V] weight: 0x0
      Reachability         : 100.0.30.9/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 309 Flags: [N] Algorithm: 0
      Reachability         : 30.9.180.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 100.0.30.9 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  3
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    juniper_379_MX304-evpn-mpls.00-00       499  13355   882    188 L2  1000.0003.7009.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: juniper_379_MX304-evpn-mpls
      Area addresses: 49.0001.0000.0000
      Interface address: 100.0.37.9
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 30.79.180.180
        IPv4 Interface Address: 30.79.180.79
        Adj-sid: 204 flags: [L V] weight: 0x0
      Reachability         : 30.79.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 100.0.37.9/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 379 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 100.0.37.9 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    6401.0001.0000.00-00         13   5904   657    187 L2  6401.0001.0000.00-00  <DefaultAtt>
      NLPID: 0xCC(IPv4) 0x8E(IPv6) 0x81(CLNP)
      Area addresses: 49.0001
      Interface address: 2001:0:58:419::419
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
      Reachability          : 2002::419/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:419::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:419::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
        SRv6 SID End with PSP USP
          SID : fcbb:0:419:11::
      Router Capabilities: Router Id: 10.0.1.119 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0
```

## show tunnel fib

```text

Type 'IS-IS SR', index 2, endpoint 100.0.0.3/32, forwarding None
   via 20.161.180.180, 'Ethernet45/1' label 900003

Type 'IS-IS SR', index 3, endpoint 100.0.0.181/32, forwarding None
   via 20.161.180.180, 'Ethernet45/1' label 900181

Type 'IS-IS SR', index 4, endpoint 100.0.3.45/32, forwarding None
   via 20.161.180.180, 'Ethernet45/1' label 900345

Type 'IS-IS SR', index 5, endpoint 100.0.37.9/32, forwarding None
   via 20.161.180.180, 'Ethernet45/1' label 900379

Type 'IS-IS SR', index 6, endpoint 100.0.3.60/32, forwarding None
   via 20.161.180.180, 'Ethernet45/1' label 900360

Type 'IS-IS SR', index 7, endpoint 100.0.0.183/32, forwarding None
   via 20.161.180.180, 'Ethernet45/1' label 900183

Type 'IS-IS SR', index 8, endpoint 100.0.0.26/32, forwarding None
   via 20.161.180.180, 'Ethernet45/1' label 900026

Type 'IS-IS SR', index 9, endpoint 100.0.0.34/32, forwarding None
   via 20.161.180.180, 'Ethernet45/1' label 900034

Type 'IS-IS SR', index 11, endpoint 100.0.3.41/32, forwarding None
   via 20.161.180.180, 'Ethernet45/1' label 900341

Type 'IS-IS SR', index 12, endpoint 100.0.30.9/32, forwarding None
   via 20.161.180.180, 'Ethernet45/1' label 900309

Type 'IS-IS SR', index 13, endpoint 100.0.0.31/32, forwarding None
   via 20.161.180.180, 'Ethernet45/1' label 900031

Type 'IS-IS SR', index 14, endpoint 100.0.3.58/32, forwarding None
   via 20.161.180.180, 'Ethernet45/1' label 900358

Type 'IS-IS SR', index 15, endpoint 100.0.0.21/32, forwarding None
   via 20.161.180.180, 'Ethernet45/1' label 900021

Type 'IS-IS SR', index 16, endpoint 100.0.0.184/32, forwarding None
   via 20.161.180.180, 'Ethernet45/1' label 900184

Type 'IS-IS SR', index 17, endpoint 100.0.0.182/32, forwarding None
   via 20.161.180.180, 'Ethernet45/1' label 900182

Type 'IS-IS SR', index 19, endpoint 100.0.3.48/32, forwarding None
   via 20.161.180.180, 'Ethernet45/1' label 900348

Type 'SRv6 Transport', index 1420, endpoint fcbb:0:59::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161

Type 'SRv6 Transport', index 1556, endpoint fcbb:0:341::/48, forwarding None
   via fe80::8e7a:ff:fee7:f53d, 'Ethernet20' SRv6, source 2002::161
```

## show isis segment-routing ipv6 locators

```text
! IS-IS (sr_eantc) is shutdown
Locator: fcbb:0:20::/48
System ID: h3c_20_CR16010E-F
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:2:1011::/48
System ID: CIEN-11-5169
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:2:1011::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

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

Locator: fcbb:6:1302::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: 133, Topology: 0

Locator: fcbb:3:1011::/48
System ID: CIEN-11-5169
Flags: Down: unset
Level: 2
Algorithm: 130, Topology: 0

Locator: fcbb:3:1011::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 130, Topology: 0

Locator: fcbb:0:607::/48
System ID: JNPR-307-ACX7024
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:1:352::/48
System ID: Cisco352-N540
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:2:352::/48
System ID: Cisco352-N540
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:2:36::/48
System ID: huawei_36
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

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

Locator: fcbb:1:1000::/36
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:1:1000::/36
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:0:1011::/48
System ID: CIEN-11-5169
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:7:1353::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: 134, Topology: 0

Locator: fcbb:2:1302::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:2:1302::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:5:1353::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: 132, Topology: 0

Locator: fcbb:0:1310::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:1:316::/48
System ID: JNPR-316-MX304
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:7:1302::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: 134, Topology: 0

Locator: fcbb:2:316::/48
System ID: JNPR-316-MX304
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:3:1011::/48
System ID: Cisco353-8201-24H8FH
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

Locator: fcbb:3:1310::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 130, Topology: 0

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
System ID: 6401.0001.0000
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:419::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:6:1353::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: 133, Topology: 0

Locator: fcbb:3:36::/48
System ID: huawei_36
Flags: Down: unset
Level: 2
Algorithm: 130, Topology: 0

Locator: fcbb:0:307::/48
System ID: JNPR-307-ACX7024
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:2:1058::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:2:1058::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:0:1610::/48
System ID: JNPR-310-ACX7100-48L
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

Locator: fcbb:1:1011::/48
System ID: CIEN-11-5169
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:3:1338::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 130, Topology: 0

Locator: fcbb:0:341::/48
System ID: h41-9902
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:4:336::/48
System ID: ZTE_336_ZXR10_M6000-8SE
Flags: Down: unset
Level: 2
Algorithm: 131, Topology: 0

Locator: fcbb:2:1310::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:2:1310::/48
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:2:1310::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

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

Locator: fcbb:0:1000::/48
System ID: CIEN-11-5169
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

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

Locator: fcbb:2:1011::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:352::/48
System ID: Cisco352-N540
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:5:1302::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: 132, Topology: 0

Locator: fcbb:2:1338::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:2:1338::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:2:342::/48
System ID: Cisco342-9902
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

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

## show bgp evpn route-type ip-prefix ipv4

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
          RD: 100.0.0.56:2000 ip-prefix 20.10.56.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2000 ip-prefix 20.30.1.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2000 ip-prefix 20.30.1.0/24
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2000 ip-prefix 20.30.2.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2000 ip-prefix 20.30.3.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2000 ip-prefix 20.30.4.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:4444 ip-prefix 20.111.182.0/24
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 * >      RD: 24:161 ip-prefix 24.161.225.0/24
                                 -                     -       -       0       i
   %      RD: 100.0.0.181:1023 ip-prefix 30.30.1.0/24
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
   %      RD: 100.0.0.181:1023 ip-prefix 30.30.2.0/24
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.161:6666 ip-prefix 44.59.225.0/24
                                 -                     -       100     0       i Or-ID: 0.231.244.180 C-LST: 100.0.3.41 
          RD: 100.0.3.41:0 ip-prefix 44.59.225.0/24
                                 PolicyReject          -       -       0       i Or-ID: 0.231.244.180 C-LST: 100.0.0.180 100.0.3.41 
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
 * >      RD: 100.0.0.182:4444 ip-prefix 2001:20:162:225::/64
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 * >      RD: 24:161 ip-prefix 2001:24:161:225::/64
                                 -                     -       -       0       i
 * >      RD: 100.0.0.182:4444 ip-prefix 2001:44:111:182::/64
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
```

## show bgp vpn-ipv4 summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.161, local AS number 1
Neighbor Status Codes: m - Under maintenance
  Neighbor V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  2001::41 4 64512            128       118    0   19 00:13:01 Estab   6      5
```

## show bgp vpn-ipv6 summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.161, local AS number 1
Neighbor Status Codes: m - Under maintenance
  Neighbor V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  2001::41 4 64512            128       118    0   19 00:13:01 Estab(NotNegotiated)
```

## show bgp neighbors 100.0.0.180 evpn advertised-routes

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
                    q - Queued for advertisement
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 24:161 ip-prefix 24.161.225.0/24
                                 100.0.0.161           -       100     0       i
 * >      RD: 100.0.0.161:6666 ip-prefix 44.59.225.0/24
                                 100.0.0.161           -       100     0       i Or-ID: 0.231.244.180 C-LST: 100.0.3.41 
 * >      RD: 24:161 ip-prefix 2001:24:161:225::/64
                                 100.0.0.161           -       100     0       i
```

## show bgp neighbors 100.0.0.180 evpn received-routes

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
          RD: 100.0.0.56:4556 auto-discovery 56 0000:0000:0000:0000:0000
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.26:2310 auto-discovery 2311 0000:0000:0000:0000:0000
                                 100.0.0.26            0       100     0       i Or-ID: 100.0.0.26 C-LST: 100.0.0.180 
   %      RD: 100.0.0.183:3301 auto-discovery 0 0000:00d2:0000:0000:00d2
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
   %      RD: 100.0.0.183:3302 auto-discovery 0 0000:00d2:0000:0000:00d2
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
   %      RD: 100.0.0.184:3301 auto-discovery 0 0000:00d2:0000:0000:00d2
                                 100.0.0.184           -       100     0       i Or-ID: 100.0.0.184 C-LST: 100.0.0.180 
   %      RD: 100.0.0.184:3302 auto-discovery 0 0000:00d2:0000:0000:00d2
                                 100.0.0.184           -       100     0       i Or-ID: 100.0.0.184 C-LST: 100.0.0.180 
   %      RD: 100.0.0.183:1 auto-discovery 0000:00d2:0000:0000:00d2
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
   %      RD: 100.0.0.184:1 auto-discovery 0000:00d2:0000:0000:00d2
                                 100.0.0.184           -       100     0       i Or-ID: 100.0.0.184 C-LST: 100.0.0.180 
 * >      RD: 100.0.3.41:3311 auto-discovery 0 0011:1111:2222:2211:1111
                                 100.0.3.41            -       100     0       i Or-ID: 100.0.3.41 C-LST: 100.0.0.180 
 * >      RD: 100.0.3.41:1 auto-discovery 0011:1111:2222:2211:1111
                                 100.0.3.41            -       100     0       i Or-ID: 100.0.3.41 C-LST: 100.0.0.180 
          RD: 100.0.0.56:4558 auto-discovery 0 0048:5648:5648:5648:5648
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:4558 auto-discovery 0048:5648:5648:5648:5648
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
   %      RD: 100.0.0.181:3301 mac-ip 0000.0181.0181
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2301 mac-ip 0002.ffff.fe0a
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.31:3 mac-ip 0012.0100.0002
                                 100.0.0.31            -       100     0       ? Or-ID: 100.0.0.31 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2301 mac-ip 0014.0100.0001
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 * >      RD: 100.0.37.9:2301 mac-ip 0015.0100.0002
                                 100.0.37.9            -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.26:2301 mac-ip 0019.0100.0002
                                 100.0.0.26            0       100     0       i Or-ID: 100.0.0.26 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.21:2301 mac-ip 001a.0100.0002
                                 100.0.0.21            0       100     0       i Or-ID: 100.0.0.21 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.3:1 mac-ip 001b.0100.0002
                                 100.0.0.3             -       100     0       i Or-ID: 100.0.0.3 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2301 mac-ip 001b.0100.0002
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2056 mac-ip 0056.5656.5656 20.10.56.253
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2301 mac-ip 0056.5656.5656 20.30.1.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2302 mac-ip 0056.5656.5656 20.30.2.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2056 mac-ip 00aa.aaaa.aaaa 20.10.56.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2301 mac-ip 00aa.aaaa.aaaa 20.30.1.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2302 mac-ip 00aa.aaaa.aaaa 20.30.2.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2303 mac-ip 2303 0056.5656.5656 20.30.3.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2303 mac-ip 2303 00aa.aaaa.aaaa 20.30.3.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2304 mac-ip 2304 0056.5656.5656 20.30.4.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2304 mac-ip 2304 00aa.aaaa.aaaa 20.30.4.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.3:1 imet 100.0.0.3
                                 100.0.0.3             -       100     0       i Or-ID: 100.0.0.3 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.21:2301 imet 100.0.0.21
                                 100.0.0.21            0       100     0       i Or-ID: 100.0.0.21 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.26:2301 imet 100.0.0.26
                                 100.0.0.26            0       100     0       i Or-ID: 100.0.0.26 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.31:3 imet 100.0.0.31
                                 100.0.0.31            -       100     0       ? Or-ID: 100.0.0.31 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2056 imet 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2301 imet 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2302 imet 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:4557 imet 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:4558 imet 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
   %      RD: 100.0.0.181:3301 imet 100.0.0.181
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
   %      RD: 100.0.0.181:3302 imet 100.0.0.181
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2301 imet 100.0.0.182
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2302 imet 100.0.0.182
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
   %      RD: 100.0.0.183:3301 imet 100.0.0.183
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
   %      RD: 100.0.0.183:3302 imet 100.0.0.183
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
   %      RD: 100.0.0.184:3301 imet 100.0.0.184
                                 100.0.0.184           -       100     0       i Or-ID: 100.0.0.184 C-LST: 100.0.0.180 
   %      RD: 100.0.0.184:3302 imet 100.0.0.184
                                 100.0.0.184           -       100     0       i Or-ID: 100.0.0.184 C-LST: 100.0.0.180 
 * >      RD: 100.0.3.41:3311 imet 100.0.3.41
                                 100.0.3.41            -       100     0       i Or-ID: 100.0.3.41 C-LST: 100.0.0.180 
 * >      RD: 100.0.30.9:2301 imet 100.0.30.9
                                 100.0.30.9            -       100     0       i Or-ID: 100.0.30.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.37.9:2301 imet 100.0.37.9
                                 100.0.37.9            -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2303 imet 2303 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2303 imet 2303 100.0.0.182
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2304 imet 2304 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2303 imet 2304 100.0.0.182
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
   %      RD: 100.0.0.183:1 ethernet-segment 0000:00d2:0000:0000:00d2 100.0.0.183
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
   %      RD: 100.0.0.184:1 ethernet-segment 0000:00d2:0000:0000:00d2 100.0.0.184
                                 100.0.0.184           -       100     0       i Or-ID: 100.0.0.184 C-LST: 100.0.0.180 
 * >      RD: 100.0.3.41:0 ethernet-segment 0011:1111:2222:2211:1111 100.0.3.41
                                 100.0.3.41            -       100     0       i Or-ID: 100.0.3.41 C-LST: 100.0.0.180 
          RD: 100.0.0.56:0 ethernet-segment 0048:5648:5648:5648:5648 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2000 ip-prefix 20.10.56.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2000 ip-prefix 20.30.1.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2000 ip-prefix 20.30.1.0/24
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2000 ip-prefix 20.30.2.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2000 ip-prefix 20.30.3.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
          RD: 100.0.0.56:2000 ip-prefix 20.30.4.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:4444 ip-prefix 20.111.182.0/24
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
   %      RD: 100.0.0.181:1023 ip-prefix 30.30.1.0/24
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
   %      RD: 100.0.0.181:1023 ip-prefix 30.30.2.0/24
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
          RD: 100.0.3.41:0 ip-prefix 44.59.225.0/24
                                 100.0.3.41            -       100     0       i Or-ID: 0.231.244.180 C-LST: 100.0.0.180 100.0.3.41 
 * >      RD: 100.0.0.182:4444 ip-prefix 2001:20:162:225::/64
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:4444 ip-prefix 2001:44:111:182::/64
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
```

## show bgp neighbors 2001::41 vpn-ipv4 advertised-routes

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast, q - Queued for advertisement
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 100.0.0.161:6666 IPv4 prefix 20.111.182.0/24
                                 2002::161             -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
```

## show bgp neighbors 2001::41 vpn-ipv4 received-routes

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
          RD: 100.0.3.41:0 IPv4 prefix 20.111.182.0/24
                                 2001::41              -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.3.41 100.0.0.180 
   %      RD: 21:59 IPv4 prefix 21.59.225.0/24
                                 2002::59              -       100     0       i Or-ID: 0.231.244.180 C-LST: 100.0.3.41 
 * >      RD: 10.0.0.59:6666 IPv4 prefix 44.59.225.0/24
                                 2002::59              -       100     0       i Or-ID: 0.231.244.180 C-LST: 100.0.3.41 
          RD: 1:130 IPv4 prefix 130.59.225.0/24
                                 2002::59              -       100     0       i Or-ID: 0.231.244.180 C-LST: 100.0.3.41 
          RD: 1:131 IPv4 prefix 131.59.225.0/24
                                 2002::59              -       100     0       i Or-ID: 0.231.244.180 C-LST: 100.0.3.41 
 * >      RD: 200:59 IPv4 prefix 200.59.225.0/24
                                 2002::59              -       100     0       i Or-ID: 0.231.244.180 C-LST: 100.0.3.41 
```

## show bgp  neighbors 2001::41 vpn-ipv4 received-routes rd 10.0.0.59:6666  detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
BGP routing table entry for IPv4 prefix 44.59.225.0/24, Route Distinguisher: 10.0.0.59:6666
 Paths: 1 available
  Local
    2002::59 from 2001::41 (100.0.3.41)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 0.231.244.180, Cluster list: 100.0.3.41 
      Community: 6666:6666
      Extended Community: Route-Target-AS:6666:6666
      Remote SRv6 SID: fcbb:0:59:e057::/64, End.DT4 with NEXT-CSID
```

## show bgp neighbors 100.0.0.180 evpn received-routes route-type ip-prefix ipv4 rd 100.0.0.182:4444 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
BGP routing table entry for ip-prefix 20.111.182.0/24, Route Distinguisher: 100.0.0.182:4444
 Paths: 1 available
  Local
    100.0.0.182 from 100.0.0.180 (100.0.0.180)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 100.0.0.182, Cluster list: 100.0.0.180 
      Extended Community: Route-Target-AS:4444:4444 TunnelEncap:tunnelTypeMpls
      Rx path id: 0x1
      MPLS label: 362148
```

## show ip route vrf T5-SR-IPVPN-SRv6-GW

```text

VRF: T5-SR-IPVPN-SRv6-GW
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

 B I      20.111.182.0/24 [200/0]
           via 100.0.0.182/32, IS-IS SR tunnel index 17, label 362148
              via 20.161.180.180, Ethernet45/1, label 900182
 B I      44.59.225.0/24 [200/0]
           via fcbb:0:59::/48, SRv6 Transport tunnel index 1420, SRv6 SID fcbb:0:59:e057::
              via fe80::8e7a:ff:fee7:f53d, Ethernet20

```

