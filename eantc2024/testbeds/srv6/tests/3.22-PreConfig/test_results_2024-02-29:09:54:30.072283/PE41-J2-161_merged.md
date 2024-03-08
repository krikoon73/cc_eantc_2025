# Test results for PE41-J2-161

## show interfaces status

```text
Port       Name         Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1                     notconnect   routed   full   25G    Not Present                    
Et2                     notconnect   1        full   25G    Not Present                    
Et3                     notconnect   1        full   25G    Not Present                    
Et4                     notconnect   1        full   25G    Not Present                    
Et5                     connected    1        full   10G    10GBASE-SRL                    
Et6                     notconnect   1        full   25G    Not Present                    
Et7                     notconnect   1        full   25G    Not Present                    
Et8                     notconnect   1        full   25G    Not Present                    
Et9                     notconnect   1        full   25G    Not Present                    
Et10                    connected    routed   full   10G    10GBASE-SR                     
Et11                    connected    trunk    full   10G    10GBASE-LR                     
Et12                    notconnect   1        full   25G    Not Present                    
Et13                    notconnect   1        full   25G    Not Present                    
Et14                    notconnect   1        full   25G    Not Present                    
Et15                    notconnect   1        full   25G    Not Present                    
Et16                    notconnect   1        full   25G    Not Present                    
Et17                    notconnect   1        full   25G    Not Present                    
Et18                    notconnect   1        full   25G    Not Present                    
Et19                    notconnect   1        full   25G    Not Present                    
Et20                    connected    routed   full   10G    10GBASE-SRL                    
Et21                    notconnect   1        full   25G    Not Present                    
Et22                    notconnect   1        full   25G    Not Present                    
Et23                    notconnect   1        full   25G    Not Present                    
Et24                    notconnect   1        full   25G    Not Present                    
Et25                    notconnect   1        full   25G    Not Present                    
Et26                    notconnect   1        full   25G    Not Present                    
Et27                    notconnect   1        full   25G    Not Present                    
Et28                    notconnect   1        full   25G    Not Present                    
Et29                    notconnect   1        full   25G    Not Present                    
Et30                    notconnect   1        full   25G    Not Present                    
Et31                    notconnect   1        full   25G    Not Present                    
Et32                    notconnect   1        full   25G    Not Present                    
Et33                    notconnect   1        full   25G    Not Present                    
Et34                    notconnect   1        full   25G    Not Present                    
Et35                    notconnect   1        full   25G    Not Present                    
Et36                    notconnect   1        full   25G    Not Present                    
Et37                    errdisabled  1        full   25G    Not Present                    
Et38                    errdisabled  1        full   25G    Not Present                    
Et39                    notconnect   1        full   10G    10GBASE-SRL                    
Et40                    notconnect   1        full   10G    10GBASE-SRL                    
Et41/1                  notconnect   1        full   100G   Not Present                    
Et42/1                  notconnect   1        full   100G   Not Present                    
Et43/1                  notconnect   1        full   100G   Not Present                    
Et44/1                  notconnect   1        full   100G   Not Present                    
Et45/1     Spine2-J-180 connected    routed   full   40G    40GBASE-SR4                    
Et46/1                  notconnect   1        full   40G    Not Present                    
Ma1                     connected    routed   a-full a-1G   10/100/1000                    

```

## show interfaces ethernet 11,10,20 | grep rate

```text
  5 seconds input rate 12.2 kbps (0.0% with framing overhead), 3 packets/sec
  5 seconds output rate 2.44 kbps (0.0% with framing overhead), 2 packets/sec
  5 seconds input rate 26 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds output rate 487 bps (0.0% with framing overhead), 0 packets/sec
  5 seconds input rate 1.14 kbps (0.0% with framing overhead), 1 packets/sec
  5 seconds output rate 69 bps (0.0% with framing overhead), 0 packets/sec
```

## show lldp neighbors

```text
Last table change time   : 13:52:00 ago
Number of table inserts  : 10
Number of table deletes  : 4
Number of table drops    : 0
Number of table age-outs : 0

Port            Neighbor Device ID               Neighbor Port ID    TTL
------------ -------------------------------- ---------------------- ---
Et5             Harness3-J-175.ns.eantc.de       Ethernet3           120
Et10            Cisco342-9902                    TenGigE0/0/0/12     120
Et11            JNPR-398-QFX5120                 546                 120
Et20            Nokia-59-IXRe2                   1610899777          121
Et45/1          Spine2-J-180.ns.eantc.de         Ethernet54/1        120
Ma1             extreme-x460-1                   42                  120

```

## show isis neighbors

```text
! IS-IS (sr_eantc) is shutdown
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
srv6      default  Cisco342-9902    L2   Ethernet10         P2P               UP    22          00                  
srv6      default  Spine2-J-180     L2   Ethernet45/1       P2P               UP    27          60                  
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
    CIEN-5169-3.00-00            35  65180 65129    203 L2  0000.0000.0003.00-00  <>
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
    h3c_20_CR16010E-F.00-00      6381  43691  1167    980 L2  0000.0000.0020.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: h3c_20_CR16010E-F
      Area addresses: 49.0000
      Interface address: 2001:0:20:36::20
      Interface address: 2001:0:20:336::20
      Interface address: 2002::20
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:20:36::36
        Global IPv6 Interface Address: 2001:0:20:36::20
      IS Neighbor          : ZTE_336_ZXR10_M6000-8SE.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:336::336
        Global IPv6 Interface Address: 2001:0:20:336::20
      Reachability          : 2001:0:20:36::/64 Metric: 10 Type: 1 Up
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
      SRv6 Locator: fcbb:3:20::/48 Topology: 0
        Metric: 0 Algorithm: 130 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:3:20::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 0
        SRv6 SID End
          SID : fcbb:3:20:e100::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP USP USD
          SID : fcbb:3:20:e101::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
    h3c_20_CR16010E-F.00-01      2855   1483  1168   1164 L2  0000.0000.0020.00-01  <>
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:20:36::36
        Global IPv6 Interface Address: 2001:0:20:36::20
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:20:36::36
        Global IPv6 Interface Address: 2001:0:20:36::20
      IS Neighbor          : ZTE_336_ZXR10_M6000-8SE.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:336::336
        Global IPv6 Interface Address: 2001:0:20:336::20
      IS Neighbor          : ZTE_336_ZXR10_M6000-8SE.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:336::336
        Global IPv6 Interface Address: 2001:0:20:336::20
      SRv6 Locator: fcbb:2:20::/48 Topology: 0
        Metric: 0 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:2:20::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 0
        SRv6 SID End
          SID : fcbb:2:20:e102::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP USP USD
          SID : fcbb:2:20:e103::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:4:20::/48 Topology: 0
        Metric: 0 Algorithm: 131 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:4:20::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 0
        SRv6 SID End
          SID : fcbb:4:20:e102::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
        SRv6 SID End with PSP USP USD
          SID : fcbb:4:20:e103::
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
          Exclude admin groups: 1
          Flags: [M] 0x80
        Flex Algo: Algorithm: 131 Metric: IGP Metric (0) Calc: SPF (0) Prio: 100
          Exclude admin groups: 255
          Flags: [M] 0x80
    h3c_20_CR16010E-F.00-02        51  51237  1168    484 L2  0000.0000.0020.00-02  <>
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:20:36::36
        Global IPv6 Interface Address: 2001:0:20:36::20
      IS Neighbor          : ZTE_336_ZXR10_M6000-8SE.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:20:336::336
        Global IPv6 Interface Address: 2001:0:20:336::20
    0000.0000.0021.00-00        663  60780   833    128 L2  0000.0000.0021.00-00  <>
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
    h3c_26_S12500R-2L.00-00       398  15479   644    139 L2  0000.0000.0026.00-00  <>
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
    h3c_28_S12500R-2L.00-00      2346  36061  1125    974 L2  0000.0000.0028.00-00  <>
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
        Algorithms:  0, 128, 129
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 100
          Flags: [] 0x1
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 100
          Flags: [] 0x1
    Huawei-34.00-00             705  16573   987    139 L2  0000.0000.0034.00-00  <>
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
    huawei_36.00-00             755  64186   987    783 L2  0000.0000.0036.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: huawei_36
      Area addresses: 49.0000
      Topology: 0 (IPv4)
      Interface address: 2002::36
      Interface address: 2001:0:36:58::36
      Interface address: 2001:0:20:36::36
      Interface address: 2001:0:36:310::36
      Reachability          : 2002::36/128 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:36::/48 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:20:36::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:36:310::/64 Metric: 10 Type: 1 Up
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
    huawei_36.00-01            1002  36674   573   1044 L2  0000.0000.0036.00-01  <>
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
    huawei_36.00-02               8   5206   572    883 L2  0000.0000.0036.00-02  <>
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
    huawei_36.00-03               7  31446   572    883 L2  0000.0000.0036.00-03  <>
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
    anet-161-R3.00-00           403  13660   500    334 L2  0000.0000.0161.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: anet-161-R3
      Area addresses: 49.0000
      Interface address: 20.161.180.161
      Interface address: 100.0.0.161
      Interface address: 2001:0:161:342::161
      Interface address: 2001:0:59:161::161
      Interface address: 2002::161
      IS Neighbor          : Cisco342-9902.00    Metric: 10
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 20.161.180.180
        IPv4 Interface Address: 20.161.180.161
        Adj-sid: 100001 flags: [L V] weight: 0x0
      Reachability         : 20.161.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 100.0.0.161/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 161 Flags: [N] Algorithm: 0
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
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SRv6 Capability: Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 900000 Range: 65536
    JNPR-307-ACX7024.00-00      2306  52301  1125    676 L2  0000.0000.0307.00-00  <>
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
      Reachability          : 2001:0:307:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:307:352::/64 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:307::/48 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:607::/48 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:7:307::/48 Topology: 0
        Metric: 0 Algorithm: 134 Flags: []
      SRv6 Locator: fcbb:5:307::/48 Topology: 0
        Metric: 0 Algorithm: 132 Flags: []
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
        Algorithms:  0, 1, 128, 129, 130, 132, 134
        Flex Algo: Algorithm: 134 Metric: IGP Metric (0) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 133 Metric: IGP Metric (0) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 132 Metric: IGP Metric (0) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 0
          Exclude admin groups: 1
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 0
      Unsupported TLV: Type: 14 Length: 2
    JNPR-310-ACX7100-48L.00-00     22616  25440  1196    952 L2  0000.0000.0310.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: JNPR-310-ACX7100-48L
      Area addresses: 49.0001
      Interface address: 10.0.1.10
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::58
        Global IPv6 Interface Address: 2001:0:58:310::310
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:36:310::36
        Global IPv6 Interface Address: 2001:0:36:310::310
      IS Neighbor          : Cisco353-8201-24H8FH.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:310:353::353
        Global IPv6 Interface Address: 2001:0:310:353::353
      Reachability          : 2002::310/128 Metric: 0 Type: 1 Up
      Reachability          : 2002::/72 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:310:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:25:110:225::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:310:338::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:36:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1310::/48 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:1610::/48 Metric: 0 Type: 1 Up
      Reachability          : fcbb:0:1000::/36 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:7:1310::/48 Topology: 0
        Metric: 0 Algorithm: 134 Flags: []
      SRv6 Locator: fcbb:5:1310::/48 Topology: 0
        Metric: 0 Algorithm: 132 Flags: []
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
      SRv6 Locator: fcbb:1:1000::/36 Topology: 0
        Metric: 10 Algorithm: 128 Flags: []
      SRv6 Locator: fcbb:0:1000::/36 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
      Router Capabilities: Router Id: 10.0.1.10 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 1, 128, 129, 130, 132, 134
        Flex Algo: Algorithm: 134 Metric: IGP Metric (0) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 133 Metric: IGP Metric (0) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 132 Metric: IGP Metric (0) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 0
          Exclude admin groups: 1
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 0
      Unsupported TLV: Type: 14 Length: 2
    JNPR-316-MX304.00-00       1725  64624   987    849 L2  0000.0000.0316.00-00  <>
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
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:7:316::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
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
    ZTE_336_ZXR10_M6000-8SE.00-00      6229  13607  1194   1278 L2  0000.0000.0336.00-00  <>
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
    h41-9902.00-00              353  32355  1078    176 L2  0000.0000.0341.00-00  <>
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
    Cisco342-9902.00-00         499  17067  1057    637 L2  0000.0000.0342.00-00  <>
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
    h45-N57C1.00-00             352  46499   582    177 L2  0000.0000.0345.00-00  <>
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
    Cisco352-N540.00-00         449  32625   662    904 L2  0000.0000.0352.00-00  <>
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
    Cisco353-8201-24H8FH.00-00      2630  58349   600   1431 L2  0000.0000.0353.00-00  <>
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
      Reachability          : 2001:0:11:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:29:338::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:49:338::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:307:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:310:338::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:310:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::/72 Metric: 10 Type: 1 Up
      Reachability          : 2002::353/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:419::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1000::/36 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:1353::/48 Metric: 1 Type: 1 Up
      Reachability          : fcbb:1:1000::/36 Metric: 50 Type: 1 Up
      Reachability          : 2001:0:29:58::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:36:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:199:302::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:199:344::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:302:353::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:25:110:225::/64 Metric: 20 Type: 1 Up
      Reachability          : fcbb:3:419::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:4:419::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:5:419::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:6:419::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:7:419::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:1:419::/48 Metric: 40 Type: 1 Up
      Reachability          : fcbb:2:419::/48 Metric: 40 Type: 1 Up
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
      SRv6 Locator: fcbb:1:1000::/36 Topology: 0
        Metric: 50 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:1:1353::/48 Topology: 0
        Metric: 1 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:1353::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:2:353::/48 Topology: 0
        Metric: 1 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:2:353::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:2:1058::/48 Topology: 0
        Metric: 22 Algorithm: 129 Flags: []
      SRv6 Locator: fcbb:2:1302::/48 Topology: 0
        Metric: 11 Algorithm: 129 Flags: []
      SRv6 Locator: fcbb:2:1310::/48 Topology: 0
        Metric: 11 Algorithm: 129 Flags: []
      SRv6 Locator: fcbb:2:1338::/48 Topology: 0
        Metric: 22 Algorithm: 129 Flags: []
      SRv6 Locator: fcbb:1:419::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:2:419::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:2:1011::/48 Topology: 0
        Metric: 11 Algorithm: 129 Flags: []
      SRv6 Locator: fcbb:2:1029::/48 Topology: 0
        Metric: 33 Algorithm: 129 Flags: []
      SRv6 Locator: fcbb:3:419::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:4:419::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:5:419::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:6:419::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:7:419::/48 Topology: 0
        Metric: 40 Algorithm: 0 Flags: []
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0, 1, 128, 129
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 128
      Unsupported TLV: Type: 14 Length: 2
    Cisco353-8201-24H8FH.00-01       205  24307  1199    117 L2  0000.0000.0353.00-01  <>
      Reachability          : 2001:0:11:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:25:102:225::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:25:58:225::/64 Metric: 20 Type: 1 Up
      Reachability          : fcbb:3:1058::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:4:1058::/48 Metric: 20 Type: 1 Up
    evpn-rr-58.00-00            348  39850  1188    178 L2  0000.0000.0358.00-00  <>
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
    evpn-rr2-60.00-00           348  47475   989    179 L2  0000.0000.0360.00-00  <>
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
    Ribbon_31.00-00             341  28922   989     79 L2  0001.0000.0031.00-00  <>
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
    Ribbon_31.00-01             340  55781   623     38 L2  0001.0000.0031.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      Hostname: Ribbon_31
    Ribbon_31.00-02             344  49043  1184    108 L2  0001.0000.0031.00-02  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      Interface address: 100.0.0.31
      Interface address: 20.31.180.31
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 20.31.180.180
        IPv4 Interface Address: 20.31.180.31
        Adj-sid: 756642 flags: [L V] weight: 0x0
        Adj-sid: 756643 flags: [L V B] weight: 0x0
      Reachability         : 100.0.0.31/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 31 Flags: [N] Algorithm: 0
      Reachability         : 20.31.180.0/24 Metric: 10 Type: 1 Up
    Spine2-J-180.00-00          628  19647   823    830 L2  0001.0001.0180.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Spine2-J-180
      Area addresses: 49.0001
      Interface address: 20.3.180.180
      Interface address: 20.21.180.180
      Interface address: 30.14.180.180
      Interface address: 20.180.182.180
      Interface address: 20.180.184.180
      Interface address: 30.41.180.180
      Interface address: 20.180.183.180
      Interface address: 20.34.180.180
      Interface address: 20.161.180.180
      Interface address: 30.79.180.180
      Interface address: 20.180.181.180
      Interface address: 20.31.180.180
      Interface address: 30.9.180.180
      Interface address: 20.56.180.180
      Interface address: 20.26.180.180
      Interface address: 30.45.180.180
      Interface address: 30.60.180.180
      Interface address: 30.58.180.180
      IS Neighbor          : CIEN-5169-3.00      Metric: 10
        IPv4 Neighbor Address: 20.3.180.3
        IPv4 Interface Address: 20.3.180.180
        Adj-sid: 100001 flags: [L V] weight: 0x0
      IS Neighbor          : PE42-J2-182.00      Metric: 10
        IPv4 Neighbor Address: 20.180.182.182
        IPv4 Interface Address: 20.180.182.180
        Adj-sid: 100004 flags: [L V] weight: 0x0
      IS Neighbor          : Huawei-34.00        Metric: 10
        IPv4 Neighbor Address: 20.34.180.34
        IPv4 Interface Address: 20.34.180.180
        Adj-sid: 100018 flags: [L V] weight: 0x0
      IS Neighbor          : juniper_379_MX304-evpn-mpls.00 Metric: 10
        IPv4 Neighbor Address: 30.79.180.79
        IPv4 Interface Address: 30.79.180.180
        Adj-sid: 100008 flags: [L V] weight: 0x0
      IS Neighbor          : PE21-J2-181.00      Metric: 10
        IPv4 Neighbor Address: 20.180.181.181
        IPv4 Interface Address: 20.180.181.180
        Adj-sid: 100000 flags: [L V] weight: 0x0
      IS Neighbor          : Ribbon_31.00        Metric: 10
        IPv4 Neighbor Address: 20.31.180.31
        IPv4 Interface Address: 20.31.180.180
        Adj-sid: 100019 flags: [L V] weight: 0x0
      IS Neighbor          : juniper-309-acx7332.00 Metric: 10
        IPv4 Neighbor Address: 30.9.180.9
        IPv4 Interface Address: 30.9.180.180
        Adj-sid: 100017 flags: [L V] weight: 0x0
      IS Neighbor          : SR1-EVPN.00         Metric: 10
        IPv4 Neighbor Address: 20.56.180.56
        IPv4 Interface Address: 20.56.180.180
        Adj-sid: 100016 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0021.00   Metric: 10
        IPv4 Neighbor Address: 20.21.180.21
        IPv4 Interface Address: 20.21.180.180
        Adj-sid: 100009 flags: [L V] weight: 0x0
      IS Neighbor          : PE24-J2-184.00      Metric: 10
        IPv4 Neighbor Address: 20.180.184.184
        IPv4 Interface Address: 20.180.184.180
        Adj-sid: 100006 flags: [L V] weight: 0x0
      IS Neighbor          : h41-9902.00         Metric: 10
        IPv4 Neighbor Address: 30.41.180.41
        IPv4 Interface Address: 30.41.180.180
        Adj-sid: 100013 flags: [L V] weight: 0x0
      IS Neighbor          : PE23-J2-183.00      Metric: 10
        IPv4 Neighbor Address: 20.180.183.183
        IPv4 Interface Address: 20.180.183.180
        Adj-sid: 100005 flags: [L V] weight: 0x0
      IS Neighbor          : anet-161-R3.00      Metric: 10
        IPv4 Neighbor Address: 20.161.180.161
        IPv4 Interface Address: 20.161.180.180
        Adj-sid: 100020 flags: [L V] weight: 0x0
      IS Neighbor          : evpn-rr2-60.00      Metric: 10
        IPv4 Neighbor Address: 30.60.180.60
        IPv4 Interface Address: 30.60.180.180
        Adj-sid: 100015 flags: [L V] weight: 0x0
      IS Neighbor          : evpn-rr-58.00       Metric: 10
        IPv4 Neighbor Address: 30.58.180.58
        IPv4 Interface Address: 30.58.180.180
        Adj-sid: 100014 flags: [L V] weight: 0x0
      IS Neighbor          : h3c_26_S12500R-2L.00 Metric: 10
        IPv4 Neighbor Address: 20.26.180.26
        IPv4 Interface Address: 20.26.180.180
        Adj-sid: 100010 flags: [L V] weight: 0x0
      IS Neighbor          : h45-N57C1.00        Metric: 10
        IPv4 Neighbor Address: 30.45.180.45
        IPv4 Interface Address: 30.45.180.180
        Adj-sid: 100002 flags: [L V] weight: 0x0
      Reachability         : 100.0.0.180/32 Metric: 0 Type: 1 Up
      Reachability         : 20.3.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.21.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 30.14.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.180.182.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.180.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 30.41.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.180.183.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.34.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.161.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 30.79.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.180.181.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.31.180.0/24 Metric: 10 Type: 1 Up
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
    PE21-J2-181.00-00           345  45136   672    156 L2  0001.0001.0181.00-00  <>
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
    PE42-J2-182.00-00           361   4863   880    182 L2  0001.0001.0182.00-00  <>
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
    PE23-J2-183.00-00           368  43071   641    156 L2  0001.0001.0183.00-00  <>
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
    PE24-J2-184.00-00           352  62964  1095    156 L2  0001.0001.0184.00-00  <>
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
    Nokia-59-IXRe2.00-00        143  55812   994    662 L2  0002.3124.4180.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-59-IXRe2
      Area addresses: 49.0000.0000.0059.00
      Interface address: 2001:0:59:161::59
      Interface address: 2001:0:59:352::59
      Interface address: 2002::59
      IS Neighbor          : Cisco352-N540.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:59:352::352
        Global IPv6 Interface Address: 2001:0:59:352::59
        Adj-sid: 1048573 flags: [L V B F] weight: 0x0
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
      Router Capabilities: Router Id: 0.231.244.180 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  9
        SRv6 Capability: Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 130, 131
    Nokia_58-SR1-3-SRv6.00-00      1592   5410 65526    922 L2  0100.0000.0058.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia_58-SR1-3-SRv6
      Area addresses:
        49.0000
        49.0001
      Interface address: 10.0.0.58
      Interface address: 2001:0:36:58::58
      Interface address: 2001:0:58:310::58
      Interface address: 2001:0:58:419::58
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:36:58::36
        Global IPv6 Interface Address: 2001:0:36:58::58
      IS Neighbor          : huawei_36.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:36:58::36
        Global IPv6 Interface Address: 2001:0:36:58::58
      Reachability         : 10.0.0.58/32 Metric: 0 Type: 1 Up
      Reachability         : 20.55.2.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.58.225.0/24 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:29:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:36:58::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:310::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::199/128 Metric: 40 Type: 1 Up
      Reachability          : fcbb:0:1000::/36 Metric: 0 Type: 1 Up
      SRv6 Locator: fcbb:0:1000::/36 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
      SRv6 Locator: fcbb:1:1338::/48 Topology: 0
        Metric: 70 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:1:1338::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
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
      SRv6 Locator: fcbb:2:1338::/48 Topology: 0
        Metric: 22 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:2:1338::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:3:1029::/48 Topology: 0
        Metric: 10 Algorithm: 130 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:3:1029:e102::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:4:1029::/48 Topology: 0
        Metric: 10 Algorithm: 131 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:4:1029:e102::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:4:1338::/48 Topology: 0
        Metric: 20 Algorithm: 131 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:4:1338::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.0.58 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SRv6 Capability: Flags: []
        Algorithms:  0, 128, 129, 130, 131
    Nokia_58-SR1-3-SRv6.00-01      5012  35369 65526   1344 L2  0100.0000.0058.00-01  <>
      Interface address: 2002::58
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::310
        Global IPv6 Interface Address: 2001:0:58:310::58
      IS Neighbor          : JNPR-310-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:310::310
        Global IPv6 Interface Address: 2001:0:58:310::58
      Reachability         : 20.57.11.0/24 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:11:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:11:353::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:29:338::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:36:310::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:49:199::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:0:49:338::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:199:302::/64 Metric: 40 Type: 1 Up
      Reachability          : 2001:0:199:344::/64 Metric: 50 Type: 1 Up
      Reachability          : 2001:0:302:353::/64 Metric: 30 Type: 1 Up
      Reachability          : 2001:0:310:338::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:0:310:353::/64 Metric: 20 Type: 1 Up
      Reachability          : 2001:25:110:225::/64 Metric: 20 Type: 1 Up
      Reachability          : 2002::/71 Metric: 20 Type: 1 Up
      Reachability          : 2002::11/128 Metric: 20 Type: 1 Up
      Reachability          : 2002::29/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::49/128 Metric: 40 Type: 1 Up
      Reachability          : 2002::58/128 Metric: 0 Type: 1 Up
      Reachability          : 2002::302/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::310/128 Metric: 10 Type: 1 Up
      Reachability          : 2002::338/128 Metric: 30 Type: 1 Up
      Reachability          : 2002::344/128 Metric: 60 Type: 1 Up
      Reachability          : 2002::353/128 Metric: 30 Type: 1 Up
      SRv6 Locator: fcbb:1:1029::/48 Topology: 0
        Metric: 89 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:1029:e101::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:1:1058::/48 Topology: 0
        Metric: 0 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:1058::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:1:1199::/48 Topology: 0
        Metric: 10907 Algorithm: 128 Flags: []
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
      SRv6 Locator: fcbb:1:1302::/48 Topology: 0
        Metric: 908 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USP USD
          SID : fcbb:1:1302::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:1:1310::/48 Topology: 0
        Metric: 43 Algorithm: 128 Flags: []
      SRv6 Locator: fcbb:1:1344::/48 Topology: 0
        Metric: 20907 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:1344::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:1:1353::/48 Topology: 0
        Metric: 859 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:1353::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:2:353::/48 Topology: 0
        Metric: 23 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:2:353::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:2:1029::/48 Topology: 0
        Metric: 11 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:2:1029:e102::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:2:1058::/48 Topology: 0
        Metric: 0 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:2:1058::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:2:1310::/48 Topology: 0
        Metric: 11 Algorithm: 129 Flags: []
      SRv6 Locator: fcbb:3:1310::/48 Topology: 0
        Metric: 10 Algorithm: 130 Flags: []
      SRv6 Locator: fcbb:3:1338::/48 Topology: 0
        Metric: 20 Algorithm: 130 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : fcbb:3:1338::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
    Nokia_58-SR1-3-SRv6.00-02         6   7464 65173    416 L2  0100.0000.0058.00-02  <>
      Reachability         : 10.0.0.57/32 Metric: 10 Type: 1 Down
        SR Prefix-SID: 1957 Flags: [R N P] Algorithm: 0
      Reachability         : 10.0.0.233/32 Metric: 10 Type: 1 Down
        SR Prefix-SID: 333 Flags: [R N P] Algorithm: 0
      Reachability         : 10.0.0.254/32 Metric: 20 Type: 1 Down
        SR Prefix-SID: 254 Flags: [R N P] Algorithm: 0
      Reachability         : 12.0.0.219/32 Metric: 20 Type: 1 Down
      Reachability         : 12.0.0.221/32 Metric: 40 Type: 1 Down
      Reachability         : 12.0.0.225/32 Metric: 30 Type: 1 Down
      Reachability         : 12.0.0.227/32 Metric: 30 Type: 1 Down
      Reachability         : 20.52.1.0/24 Metric: 30 Type: 1 Down
      Reachability         : 20.54.2.0/24 Metric: 20 Type: 1 Down
      Reachability         : 20.56.2.0/24 Metric: 20 Type: 1 Down
      Reachability         : 20.57.10.0/24 Metric: 0 Type: 1 Up
      Reachability         : 20.57.12.0/24 Metric: 20 Type: 1 Down
      Reachability         : 20.57.13.0/24 Metric: 20 Type: 1 Down
      Reachability         : 20.57.15.0/24 Metric: 20 Type: 1 Down
      Reachability         : 25.20.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.29.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.36.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.59.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.107.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.110.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.116.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.136.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.138.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.142.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.144.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.152.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.153.225.0/24 Metric: 0 Type: 1 Up
      Reachability          : 2001:25:58:225::/64 Metric: 0 Type: 1 Up
      Reachability          : fcbb:3:1058::/48 Metric: 0 Type: 1 Up
      Reachability          : fcbb:4:1058::/48 Metric: 0 Type: 1 Up
    Nokia_58-SR1-3-SRv6.00-03       174  47402 65527    949 L2  0100.0000.0058.00-03  <>
      IS Neighbor          : Keys-Ixia-419.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:58:419::419
        Global IPv6 Interface Address: 2001:0:58:419::58
      IS Neighbor          : Keys-Ixia-419.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:58:419::419
        Global IPv6 Interface Address: 2001:0:58:419::58
      Reachability         : 25.102.225.0/24 Metric: 0 Type: 1 Up
      Reachability         : 25.219.225.0/24 Metric: 0 Type: 1 Up
      Reachability          : 2001:21:219:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:25:20:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:25:29:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:25:36:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:25:59:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:25:107:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:25:116:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:25:142:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:25:144:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:25:152:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:25:153:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:25:219:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:25:336:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:25:338:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:129:219:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:130:219:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:131:219:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:132:219:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:133:219:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:134:219:225::/64 Metric: 0 Type: 1 Up
      Reachability          : 2002::419/128 Metric: 20 Type: 1 Up
      Reachability          : fcbb:0:419::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:1:419::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:3:419::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:5:419::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:6:419::/48 Metric: 20 Type: 1 Up
      Reachability          : fcbb:7:419::/48 Metric: 20 Type: 1 Up
      SRv6 Locator: fcbb:0:419::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:419:11::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:2:419::/48 Topology: 0
        Metric: 11 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:2:419:11::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:3:1011::/48 Topology: 0
        Metric: 20 Algorithm: 130 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:3:1011::
          SID structure: Block length: 32 Node length: 16
                         Function length: 16 Argument length: 0
      SRv6 Locator: fcbb:4:419::/48 Topology: 0
        Metric: 10 Algorithm: 131 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:4:419:11::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
    SR1-EVPN.00-00              452  38972  1195    198 L2  1000.0000.0056.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: SR1-EVPN
      Area addresses: 49.0001
      Interface address: 20.56.180.56
      Interface address: 100.0.0.56
      Interface address: 2001::56
      IS Neighbor          : Spine2-J-180.00     Metric: 10
        IPv4 Neighbor Address: 20.56.180.180
        IPv4 Interface Address: 20.56.180.56
        Adj-sid: 524271 flags: [L V B] weight: 0x0
      Reachability         : 20.56.180.0/24 Metric: 10 Type: 1 Up
      Reachability         : 100.0.0.56/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 56 Flags: [N P] Algorithm: 0
      Reachability          : 2001::56/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 100.0.0.56 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    juniper-309-acx7332.00-00       350  39545   675    180 L2  1000.0003.0009.00-00  <>
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
    juniper_379_MX304-evpn-mpls.00-00       375  11694   750    188 L2  1000.0003.7009.00-00  <>
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
    Keys-Ixia-419.00-00         599  21068   842   1043 L2  3800.0000.0419.00-00  <DefaultAtt>
      NLPID: 0xCC(IPv4) 0x8E(IPv6) 0x81(CLNP)
      Hostname: Keys-Ixia-419
      Area addresses: 49.0001
      Interface address: 2001:0:58:419::419
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:419::58
        Global IPv6 Interface Address: 2001:0:58:419::419
      IS Neighbor          : Nokia_58-SR1-3-SRv6.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:58:419::58
        Global IPv6 Interface Address: 2001:0:58:419::419
      Reachability          : 2002::419/128 Metric: 10 Type: 1 Up
      Reachability          : fcbb:0:419::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:1:419::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:2:419::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:3:419::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:4:419::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:5:419::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:6:419::/48 Metric: 10 Type: 1 Up
      Reachability          : fcbb:7:419::/48 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:58:419::/64 Metric: 10 Type: 1 Up
      SRv6 Locator: fcbb:0:419::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:0:419:11::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:1:419::/48 Topology: 0
        Metric: 0 Algorithm: 128 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:1:419:11::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:2:419::/48 Topology: 0
        Metric: 0 Algorithm: 129 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:2:419:11::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:3:419::/48 Topology: 0
        Metric: 0 Algorithm: 130 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:3:419:11::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:4:419::/48 Topology: 0
        Metric: 0 Algorithm: 131 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:4:419:11::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:5:419::/48 Topology: 0
        Metric: 0 Algorithm: 132 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:5:419:11::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:6:419::/48 Topology: 0
        Metric: 0 Algorithm: 133 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:6:419:11::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      SRv6 Locator: fcbb:7:419::/48 Topology: 0
        Metric: 0 Algorithm: 134 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : fcbb:7:419:11::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.1.119 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0, 128, 129, 130, 131, 132, 133, 134
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

Type 'IS-IS SR', index 10, endpoint 100.0.0.56/32, forwarding None
   via 20.161.180.180, 'Ethernet45/1' label 900056

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

Type 'SRv6 Transport', index 593, endpoint fcbb:0:28::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 594, endpoint fcbb:0:36::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 595, endpoint fcbb:0:1000::/36, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 596, endpoint fcbb:3:59::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 597, endpoint fcbb:0:307::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 598, endpoint fcbb:0:352::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 599, endpoint fcbb:0:336::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 600, endpoint fcbb:0:1310::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 601, endpoint fcbb:1:1000::/36, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 602, endpoint fcbb:0:59::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 603, endpoint fcbb:0:20::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 604, endpoint fcbb:4:59::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 605, endpoint fcbb:0:1353::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 609, endpoint fcbb:0:342::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 610, endpoint fcbb:4:1058::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161

Type 'SRv6 Transport', index 611, endpoint fcbb:3:1058::/48, forwarding None
   via fe80::fa7a:41ff:fe18:8910, 'Ethernet10' SRv6, source 2002::161
```

## show isis segment-routing ipv6 locators

```text
! IS-IS (sr_eantc) is shutdown
Locator: fcbb:3:1029::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 130, Topology: 0

Locator: fcbb:0:20::/48
System ID: h3c_20_CR16010E-F
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:2:1011::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:2:1011::/48
System ID: Cisco353-8201-24H8FH
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

Locator: fcbb:3:20::/48
System ID: h3c_20_CR16010E-F
Flags: Down: unset
Level: 2
Algorithm: 130, Topology: 0

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

Locator: fcbb:6:419::/48
System ID: Keys-Ixia-419
Flags: Down: unset
Level: 2
Algorithm: 133, Topology: 0

Locator: fcbb:2:419::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:2:419::/48
System ID: Keys-Ixia-419
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:1:28::/48
System ID: h3c_28_S12500R-2L
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

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

Locator: fcbb:1:1302::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:2:36::/48
System ID: huawei_36
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:2:419::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:36::/48
System ID: huawei_36
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:4:1338::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 131, Topology: 0

Locator: fcbb:5:419::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:3:336::/48
System ID: ZTE_336_ZXR10_M6000-8SE
Flags: Down: unset
Level: 2
Algorithm: 130, Topology: 0

Locator: fcbb:2:20::/48
System ID: h3c_20_CR16010E-F
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

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

Locator: fcbb:6:316::/48
System ID: JNPR-316-MX304
Flags: Down: unset
Level: 2
Algorithm: 133, Topology: 0

Locator: fcbb:4:20::/48
System ID: h3c_20_CR16010E-F
Flags: Down: unset
Level: 2
Algorithm: 131, Topology: 0

Locator: fcbb:1:1000::/36
System ID: JNPR-310-ACX7100-48L
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:6:419::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

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

Locator: fcbb:4:1029::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 131, Topology: 0

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

Locator: fcbb:1:419::/48
System ID: Keys-Ixia-419
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

Locator: fcbb:3:419::/48
System ID: Cisco353-8201-24H8FH
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

Locator: fcbb:2:1029::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:2:1029::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

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

Locator: fcbb:3:419::/48
System ID: Keys-Ixia-419
Flags: Down: unset
Level: 2
Algorithm: 130, Topology: 0

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

Locator: fcbb:3:36::/48
System ID: huawei_36
Flags: Down: unset
Level: 2
Algorithm: 130, Topology: 0

Locator: fcbb:4:419::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

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

Locator: fcbb:7:419::/48
System ID: Keys-Ixia-419
Flags: Down: unset
Level: 2
Algorithm: 134, Topology: 0

Locator: fcbb:1:20::/48
System ID: h3c_20_CR16010E-F
Flags: Down: unset
Level: 2
Algorithm: 128, Topology: 0

Locator: fcbb:3:1338::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 130, Topology: 0

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

Locator: fcbb:7:419::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:4:419::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 131, Topology: 0

Locator: fcbb:4:419::/48
System ID: Keys-Ixia-419
Flags: Down: unset
Level: 2
Algorithm: 131, Topology: 0

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

Locator: fcbb:2:353::/48
System ID: Nokia_58-SR1-3-SRv6
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

Locator: fcbb:2:353::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: 129, Topology: 0

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

Locator: fcbb:1:419::/48
System ID: Cisco353-8201-24H8FH
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

Locator: fcbb:0:352::/48
System ID: Cisco352-N540
Flags: Down: unset
Level: 2
Algorithm: SPF (0), Topology: 0

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

Locator: fcbb:5:419::/48
System ID: Keys-Ixia-419
Flags: Down: unset
Level: 2
Algorithm: 132, Topology: 0

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
 * >      RD: 100.0.0.31:2000 ip-prefix 20.10.31.0/24
                                 100.0.0.31            -       100     0       i Or-ID: 100.0.0.31 C-LST: 100.0.0.180 
 * >      RD: 100.0.37.9:2000 ip-prefix 20.10.32.0/24
                                 100.0.37.9            -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.37.9:2000 ip-prefix 20.10.32.32/32
                                 100.0.37.9            -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.37.9:2000 ip-prefix 20.10.32.201/32
                                 100.0.37.9            -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2000 ip-prefix 20.10.56.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.4:2000 ip-prefix 20.30.1.0/24
                                 100.0.0.34            0       100     0       ? Or-ID: 100.0.0.34 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2000 ip-prefix 20.30.1.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2000 ip-prefix 20.30.1.0/24
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2000 ip-prefix 20.30.2.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2000 ip-prefix 20.30.3.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2000 ip-prefix 20.30.4.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 24:161 ip-prefix 24.161.225.0/24
                                 -                     -       -       0       i
   %      RD: 100.0.0.181:1023 ip-prefix 30.30.1.0/24
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
   %      RD: 100.0.0.181:1023 ip-prefix 30.30.2.0/24
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
 * >      RD: 2000:161 ip-prefix 220.161.225.0/24
                                 -                     -       -       0       i
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
 * >      RD: 2000:161 ip-prefix 2001:20:11:225::/64
                                 -                     -       100     0       ? Or-ID: 10.0.0.11 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:20:225::/64
                                 -                     0       100     0       ? Or-ID: 10.0.0.20 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:28:225::/64
                                 -                     0       100     0       ? Or-ID: 10.0.0.28 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:29:225::/64
                                 -                     0       100     0       ? Or-ID: 10.0.0.29 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:36:225::/64
                                 -                     0       100     0       ? Or-ID: 192.168.20.36 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:58:225::/64
                                 -                     -       100     0       i Or-ID: 10.0.0.58 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:59:225::/64
                                 -                     -       100     0       i Or-ID: 0.231.244.180 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:102:225::/64
                                 -                     -       100     0       i Or-ID: 10.0.1.2 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:107:225::/64
                                 -                     -       100     0       i Or-ID: 10.0.1.7 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:110:225::/64
                                 -                     -       100     0       i Or-ID: 10.0.1.10 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:142:225::/64
                                 -                     0       100     0       ? Or-ID: 100.0.0.42 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:144:225::/64
                                 -                     0       100     0       ? Or-ID: 100.0.0.44 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:152:225::/64
                                 -                     0       100     0       ? Or-ID: 100.0.0.52 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:153:225::/64
                                 -                     0       100     0       ?
 * >      RD: 2000:161 ip-prefix 2001:20:199:225::/64
                                 -                     0       100     0       ? Or-ID: 20.49.199.199 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:336:225::/64
                                 -                     -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
 * >      RD: 24:161 ip-prefix 2001:24:161:225::/64
                                 -                     -       -       0       i
 * >      RD: 2000:161 ip-prefix 2001:3024:161:225::/64
                                 -                     -       -       0       i
```

## show bgp vpn-ipv4 summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.161, local AS number 1
Neighbor Status Codes: m - Under maintenance
  Neighbor  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  2002::353 4 1               4352      1687    0    0 01:36:00 Estab   87     87
```

## show bgp vpn-ipv6 summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.161, local AS number 1
Neighbor Status Codes: m - Under maintenance
  Neighbor  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  2002::353 4 1               4352      1687    0    0 01:36:00 Estab   28     28
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
 * >      RD: 2000:161 ip-prefix 220.161.225.0/24
                                 100.0.0.161           -       100     0       i
 * >      RD: 2000:161 ip-prefix 2001:20:11:225::/64
                                 100.0.0.161           -       100     0       ? Or-ID: 10.0.0.11 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:20:225::/64
                                 100.0.0.161           0       100     0       ? Or-ID: 10.0.0.20 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:28:225::/64
                                 100.0.0.161           0       100     0       ? Or-ID: 10.0.0.28 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:29:225::/64
                                 100.0.0.161           0       100     0       ? Or-ID: 10.0.0.29 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:36:225::/64
                                 100.0.0.161           0       100     0       ? Or-ID: 192.168.20.36 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:58:225::/64
                                 100.0.0.161           -       100     0       i Or-ID: 10.0.0.58 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:59:225::/64
                                 100.0.0.161           -       100     0       i Or-ID: 0.231.244.180 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:102:225::/64
                                 100.0.0.161           -       100     0       i Or-ID: 10.0.1.2 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:107:225::/64
                                 100.0.0.161           -       100     0       i Or-ID: 10.0.1.7 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:110:225::/64
                                 100.0.0.161           -       100     0       i Or-ID: 10.0.1.10 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:142:225::/64
                                 100.0.0.161           0       100     0       ? Or-ID: 100.0.0.42 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:144:225::/64
                                 100.0.0.161           0       100     0       ? Or-ID: 100.0.0.44 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:152:225::/64
                                 100.0.0.161           0       100     0       ? Or-ID: 100.0.0.52 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:153:225::/64
                                 100.0.0.161           0       100     0       ?
 * >      RD: 2000:161 ip-prefix 2001:20:199:225::/64
                                 100.0.0.161           0       100     0       ? Or-ID: 20.49.199.199 C-LST: 100.0.0.53 
 * >      RD: 2000:161 ip-prefix 2001:20:336:225::/64
                                 100.0.0.161           -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
 * >      RD: 24:161 ip-prefix 2001:24:161:225::/64
                                 100.0.0.161           -       100     0       i
 * >      RD: 2000:161 ip-prefix 2001:3024:161:225::/64
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
 * >      RD: 100.0.0.56:4556 auto-discovery 56 0000:0000:0000:0000:0000
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.4:2301 auto-discovery 0 0000:0000:0000:0123:0123
                                 100.0.0.34            -       100     0       i Or-ID: 100.0.0.34 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2301 auto-discovery 0 0000:0000:0000:0123:0123
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2302 auto-discovery 0 0000:0000:0000:0123:0123
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2303 auto-discovery 0 0000:0000:0000:0123:0123
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.34:0 auto-discovery 0000:0000:0000:0123:0123
                                 100.0.0.34            -       100     0       i Or-ID: 100.0.0.34 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:1 auto-discovery 0000:0000:0000:0123:0123
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
   %      RD: 100.0.0.183:3301 auto-discovery 0 0000:00d2:0000:0000:00d2
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
   %      RD: 100.0.0.183:3302 auto-discovery 0 0000:00d2:0000:0000:00d2
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
   %      RD: 100.0.0.183:1 auto-discovery 0000:00d2:0000:0000:00d2
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 * >      RD: 100.0.30.9:10 auto-discovery 2320 0001:0203:0405:0607:0801
                                 100.0.30.9            -       100     0       i Or-ID: 100.0.30.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.30.9:10 auto-discovery 2321 0001:0203:0405:0607:0801
                                 100.0.30.9            -       100     0       i Or-ID: 100.0.30.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.30.9:0 auto-discovery 0001:0203:0405:0607:0801
                                 100.0.30.9            -       100     0       i Or-ID: 100.0.30.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:4558 auto-discovery 0 0048:5648:5648:5648:5648
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:4558 auto-discovery 0048:5648:5648:5648:5648
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.37.9:0 auto-discovery 0500:00fc:0000:0007:f000
                                 100.0.37.9            -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
   %      RD: 100.0.0.181:3301 mac-ip 0000.0181.0181
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.4:2301 mac-ip 0012.0100.0002
                                 100.0.0.34            -       100     0       i Or-ID: 100.0.0.34 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2301 mac-ip 0012.0100.0002
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2301 mac-ip 0012.0100.0002 20.30.1.68
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.31:2 mac-ip 0014.0100.0001
                                 100.0.0.31            -       100     0       ? Or-ID: 100.0.0.31 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.31:2 mac-ip 0014.0100.0001 20.10.31.31
                                 100.0.0.31            -       100     0       ? Or-ID: 100.0.0.31 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2056 mac-ip 0056.5656.5656 20.10.56.253
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2301 mac-ip 0056.5656.5656 20.30.1.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2302 mac-ip 0056.5656.5656 20.30.2.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.4:2301 mac-ip 00aa.aaaa.aaaa
                                 100.0.0.34            -       100     0       i Or-ID: 100.0.0.34 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.31:2 mac-ip 00aa.aaaa.aaaa 20.10.31.254
                                 100.0.0.31            -       100     0       ? Or-ID: 100.0.0.31 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2056 mac-ip 00aa.aaaa.aaaa 20.10.56.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2301 mac-ip 00aa.aaaa.aaaa 20.30.1.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2302 mac-ip 00aa.aaaa.aaaa 20.30.2.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.37.9:2032 mac-ip 2032 0015.0100.0001
                                 100.0.37.9            -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.37.9:2032 mac-ip 2032 0015.0100.0001 20.10.32.32
                                 100.0.37.9            -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.37.9:2032 mac-ip 2032 00aa.aaaa.aaaa
                                 100.0.37.9            -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.37.9:2032 mac-ip 2032 00aa.aaaa.aaaa 20.10.32.254
                                 100.0.37.9            -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.37.9:2032 mac-ip 2032 60c7.8d2d.4416
                                 100.0.37.9            -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.37.9:2032 mac-ip 2032 60c7.8d2d.4416 20.10.32.201
                                 100.0.37.9            -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2303 mac-ip 2303 0056.5656.5656 20.30.3.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2303 mac-ip 2303 00aa.aaaa.aaaa 20.30.3.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2304 mac-ip 2304 0056.5656.5656 20.30.4.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2304 mac-ip 2304 00aa.aaaa.aaaa 20.30.4.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.21:2021 imet 100.0.0.21
                                 100.0.0.21            0       100     0       i Or-ID: 100.0.0.21 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.21:2301 imet 100.0.0.21
                                 100.0.0.21            0       100     0       i Or-ID: 100.0.0.21 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.21:2302 imet 100.0.0.21
                                 100.0.0.21            0       100     0       i Or-ID: 100.0.0.21 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.26:2026 imet 100.0.0.26
                                 100.0.0.26            0       100     0       i Or-ID: 100.0.0.26 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.26:2301 imet 100.0.0.26
                                 100.0.0.26            0       100     0       i Or-ID: 100.0.0.26 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.26:2302 imet 100.0.0.26
                                 100.0.0.26            0       100     0       i Or-ID: 100.0.0.26 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.31:2 imet 100.0.0.31
                                 100.0.0.31            -       100     0       ? Or-ID: 100.0.0.31 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.4:2301 imet 100.0.0.34
                                 100.0.0.34            -       100     0       i Or-ID: 100.0.0.34 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2056 imet 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2301 imet 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2302 imet 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:4557 imet 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:4558 imet 100.0.0.56
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
 * >      RD: 100.0.37.9:2032 imet 2032 100.0.37.9
                                 100.0.37.9            -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.21:2303 imet 2303 100.0.0.21
                                 100.0.0.21            0       100     0       i Or-ID: 100.0.0.21 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.26:2303 imet 2303 100.0.0.26
                                 100.0.0.26            0       100     0       i Or-ID: 100.0.0.26 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2303 imet 2303 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2303 imet 2303 100.0.0.182
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.21:2304 imet 2304 100.0.0.21
                                 100.0.0.21            0       100     0       i Or-ID: 100.0.0.21 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.26:2304 imet 2304 100.0.0.26
                                 100.0.0.26            0       100     0       i Or-ID: 100.0.0.26 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2304 imet 2304 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2303 imet 2304 100.0.0.182
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.34:0 ethernet-segment 0000:0000:0000:0123:0123 100.0.0.34
                                 100.0.0.34            -       100     0       i Or-ID: 100.0.0.34 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:1 ethernet-segment 0000:0000:0000:0123:0123 100.0.0.182
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
   %      RD: 100.0.0.183:1 ethernet-segment 0000:00d2:0000:0000:00d2 100.0.0.183
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 * >      RD: 100.0.30.9:0 ethernet-segment 0001:0203:0405:0607:0801 100.0.30.9
                                 100.0.30.9            -       100     0       i Or-ID: 100.0.30.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:0 ethernet-segment 0048:5648:5648:5648:5648 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.31:2000 ip-prefix 20.10.31.0/24
                                 100.0.0.31            -       100     0       i Or-ID: 100.0.0.31 C-LST: 100.0.0.180 
 * >      RD: 100.0.37.9:2000 ip-prefix 20.10.32.0/24
                                 100.0.37.9            -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.37.9:2000 ip-prefix 20.10.32.32/32
                                 100.0.37.9            -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.37.9:2000 ip-prefix 20.10.32.201/32
                                 100.0.37.9            -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2000 ip-prefix 20.10.56.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.4:2000 ip-prefix 20.30.1.0/24
                                 100.0.0.34            0       100     0       ? Or-ID: 100.0.0.34 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2000 ip-prefix 20.30.1.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.182:2000 ip-prefix 20.30.1.0/24
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2000 ip-prefix 20.30.2.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2000 ip-prefix 20.30.3.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.56:2000 ip-prefix 20.30.4.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
   %      RD: 100.0.0.181:1023 ip-prefix 30.30.1.0/24
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
   %      RD: 100.0.0.181:1023 ip-prefix 30.30.2.0/24
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
```

## show bgp neighbors 2002::353 vpn-ipv4 advertised-routes

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast, q - Queued for advertisement
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 2000:161 IPv4 prefix 20.10.31.0/24
                                 2002::161             -       100     0       i Or-ID: 100.0.0.31 C-LST: 100.0.0.180 
 * >      RD: 2000:161 IPv4 prefix 20.10.31.31/32
                                 2002::161             -       100     0       ? Or-ID: 100.0.0.31 C-LST: 100.0.0.180 
 * >      RD: 2000:161 IPv4 prefix 20.10.31.254/32
                                 2002::161             -       100     0       ? Or-ID: 100.0.0.31 C-LST: 100.0.0.180 
 * >      RD: 2000:161 IPv4 prefix 20.10.32.0/24
                                 2002::161             -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
 * >      RD: 2000:161 IPv4 prefix 20.10.32.32/32
                                 2002::161             -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
 * >      RD: 2000:161 IPv4 prefix 20.10.32.201/32
                                 2002::161             -       100     0       i Or-ID: 100.0.37.9 C-LST: 100.0.0.180 
 * >      RD: 2000:161 IPv4 prefix 20.10.56.0/24
                                 2002::161             -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 2000:161 IPv4 prefix 20.30.1.0/24
                                 2002::161             -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 2000:161 IPv4 prefix 20.30.1.68/32
                                 2002::161             -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 * >      RD: 2000:161 IPv4 prefix 20.30.2.0/24
                                 2002::161             -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 2000:161 IPv4 prefix 20.30.3.0/24
                                 2002::161             -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 2000:161 IPv4 prefix 20.30.4.0/24
                                 2002::161             -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 * >      RD: 2000:161 IPv4 prefix 220.161.225.0/24
                                 2002::161             -       100     0       i
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
 * >      RD: 1011:1 IPv4 prefix 20.11.225.0/24
                                 2002::11              -       100     0       ? Or-ID: 10.0.0.11 C-LST: 100.0.0.53 
 * >      RD: 1:20 IPv4 prefix 20.20.225.0/24
                                 2002::20              0       100     0       ? Or-ID: 10.0.0.20 C-LST: 100.0.0.53 
 * >      RD: 1:28 IPv4 prefix 20.28.225.0/24
                                 2002::28              0       100     0       ? Or-ID: 10.0.0.28 C-LST: 100.0.0.53 
 * >      RD: 1:29 IPv4 prefix 20.29.225.0/24
                                 2002::29              0       100     0       ? Or-ID: 10.0.0.29 C-LST: 100.0.0.53 
 * >      RD: 1:36 IPv4 prefix 20.36.225.0/24
                                 2002::36              0       100     0       ? Or-ID: 192.168.20.36 C-LST: 100.0.0.53 
   %      RD: 10.0.0.57:10000 IPv4 prefix 20.54.1.0/24
                                 2002::57              -       100     0       65000 i Or-ID: 10.0.0.57 C-LST: 100.0.0.53 0.231.244.180 
   %      RD: 10.0.0.58:10000 IPv4 prefix 20.55.1.0/24
                                 2002::58              -       100     0       i Or-ID: 10.0.0.58 C-LST: 100.0.0.53 
   %      RD: 10.0.0.57:1 IPv4 prefix 20.57.111.0/24
                                 2002::57              -       100     0       65000 i Or-ID: 10.0.0.57 C-LST: 100.0.0.53 0.231.244.180 
   %      RD: 10.0.0.57:128 IPv4 prefix 20.57.111.0/24
                                 2002::57              -       100     0       65000 i Or-ID: 10.0.0.57 C-LST: 100.0.0.53 0.231.244.180 
   %      RD: 10.0.0.57:129 IPv4 prefix 20.57.111.0/24
                                 2002::57              -       100     0       65000 i Or-ID: 10.0.0.57 C-LST: 100.0.0.53 0.231.244.180 
   %      RD: 10.0.0.57:130 IPv4 prefix 20.57.111.0/24
                                 2002::57              -       100     0       65000 i Or-ID: 10.0.0.57 C-LST: 100.0.0.53 0.231.244.180 
   %      RD: 10.0.0.57:131 IPv4 prefix 20.57.111.0/24
                                 2002::57              -       100     0       65000 i Or-ID: 10.0.0.57 C-LST: 100.0.0.53 0.231.244.180 
   %      RD: 10.0.0.57:132 IPv4 prefix 20.57.111.0/24
                                 2002::57              -       100     0       65000 i Or-ID: 10.0.0.57 C-LST: 100.0.0.53 0.231.244.180 
   %      RD: 10.0.0.57:211 IPv4 prefix 20.57.111.0/24
                                 2002::57              -       100     0       65000 i Or-ID: 10.0.0.57 C-LST: 100.0.0.53 0.231.244.180 
 * >      RD: 1:58 IPv4 prefix 20.58.225.0/24
                                 2002::58              -       100     0       i Or-ID: 10.0.0.58 C-LST: 100.0.0.53 
   %      RD: 10.0.0.59:209 IPv4 prefix 20.59.111.0/24
                                 2002::59              -       100     0       i Or-ID: 0.231.244.180 C-LST: 100.0.0.53 
 * >      RD: 1:59 IPv4 prefix 20.59.225.0/24
                                 2002::59              -       100     0       i Or-ID: 0.231.244.180 C-LST: 100.0.0.53 
   %      RD: 10.0.0.103:8 IPv4 prefix 20.83.111.0/24
                                 2002::303             -       100     0       65000 i Or-ID: 192.168.21.3 C-LST: 100.0.0.53 0.231.244.180 
 * >      RD: 1:302 IPv4 prefix 20.102.225.0/24
                                 2002::302             -       100     0       i Or-ID: 10.0.1.2 C-LST: 100.0.0.53 
 * >      RD: 1:307 IPv4 prefix 20.107.225.0/24
                                 2002::307             -       100     0       i Or-ID: 10.0.1.7 C-LST: 100.0.0.53 
 * >      RD: 1:310 IPv4 prefix 20.110.225.0/24
                                 2002::310             -       100     0       i Or-ID: 10.0.1.10 C-LST: 100.0.0.53 
 * >      RD: 1:336 IPv4 prefix 20.136.225.0/24
                                 2002::336             -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
 * >      RD: 1:338 IPv4 prefix 20.138.225.0/24
                                 2002::338             -       100     0       ? Or-ID: 10.0.1.38 C-LST: 100.0.0.53 
          RD: 100:2 IPv4 prefix 20.139.221.0/24
                                 2002::36              0       100     0       ? Or-ID: 192.168.20.36 C-LST: 100.0.0.53 
 * >      RD: 1:342 IPv4 prefix 20.142.225.0/24
                                 2002::342             0       100     0       ? Or-ID: 100.0.0.42 C-LST: 100.0.0.53 
 * >      RD: 1:344 IPv4 prefix 20.144.225.0/24
                                 2002::344             0       100     0       ? Or-ID: 100.0.0.44 C-LST: 100.0.0.53 
 * >      RD: 1:352 IPv4 prefix 20.152.225.0/24
                                 2002::352             0       100     0       ? Or-ID: 100.0.0.52 C-LST: 100.0.0.53 
 * >      RD: 1:353 IPv4 prefix 20.153.225.0/24
                                 2002::353             0       100     0       ?
          RD: 3:20 IPv4 prefix 20.199.222.0/24
                                 2002::20              0       100     0       ? Or-ID: 10.0.0.20 C-LST: 100.0.0.53 
          RD: 100:1 IPv4 prefix 20.199.222.0/24
                                 2002::199             0       100     0       ? Or-ID: 20.49.199.199 C-LST: 100.0.0.53 
 * >      RD: 1:199 IPv4 prefix 20.199.225.0/24
                                 2002::199             0       100     0       ? Or-ID: 20.49.199.199 C-LST: 100.0.0.53 
 * >      RD: 21:199 IPv4 prefix 20.199.225.0/24
                                 2002::199             0       100     0       ? Or-ID: 20.49.199.199 C-LST: 100.0.0.53 
   %      RD: 100:1 IPv4 prefix 20.219.225.0/24
                                 2002::419             -       0       0       i Or-ID: 192.0.0.1 C-LST: 100.0.0.53 
 * >      RD: 21:11 IPv4 prefix 21.11.225.0/24
                                 2002::11              -       100     0       ? Or-ID: 10.0.0.11 C-LST: 100.0.0.53 
          RD: 1:21 IPv4 prefix 21.20.225.0/24
                                 2002::20              0       100     0       ? Or-ID: 10.0.0.20 C-LST: 100.0.0.53 
          RD: 1:21 IPv4 prefix 21.28.225.0/24
                                 2002::28              0       100     0       ? Or-ID: 10.0.0.28 C-LST: 100.0.0.53 
 * >      RD: 1:21 IPv4 prefix 21.29.225.0/24
                                 2002::29              0       100     0       ? Or-ID: 10.0.0.29 C-LST: 100.0.0.53 
          RD: 1:21 IPv4 prefix 21.36.225.0/24
                                 2002::36              0       100     0       ? Or-ID: 192.168.20.36 C-LST: 100.0.0.53 
 * >      RD: 21:58 IPv4 prefix 21.58.225.0/24
                                 2002::58              -       100     0       i Or-ID: 10.0.0.58 C-LST: 100.0.0.53 
   %      RD: 21:59 IPv4 prefix 21.59.225.0/24
                                 2002::59              -       100     0       i Or-ID: 0.231.244.180 C-LST: 100.0.0.53 
 * >      RD: 21:302 IPv4 prefix 21.102.225.0/24
                                 2002::302             -       100     0       i Or-ID: 10.0.1.2 C-LST: 100.0.0.53 
          RD: 21:307 IPv4 prefix 21.107.225.0/24
                                 2002::307             -       100     0       i Or-ID: 10.0.1.7 C-LST: 100.0.0.53 
 * >      RD: 21:310 IPv4 prefix 21.110.225.0/24
                                 2002::310             -       100     0       i Or-ID: 10.0.1.10 C-LST: 100.0.0.53 
          RD: 21:336 IPv4 prefix 21.136.225.0/24
                                 2002::336             -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
 * >      RD: 21:338 IPv4 prefix 21.138.225.0/24
                                 2002::338             -       100     0       ? Or-ID: 10.0.1.38 C-LST: 100.0.0.53 
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
 * >      RD: 24:342 IPv4 prefix 24.142.225.0/24
                                 2002::342             0       100     0       ? Or-ID: 100.0.0.42 C-LST: 100.0.0.53 
 * >      RD: 24:344 IPv4 prefix 24.144.225.0/24
                                 2002::344             0       100     0       ? Or-ID: 100.0.0.44 C-LST: 100.0.0.53 
 * >      RD: 24:352 IPv4 prefix 24.152.225.0/24
                                 2002::352             0       100     0       ? Or-ID: 100.0.0.52 C-LST: 100.0.0.53 
 * >      RD: 24:353 IPv4 prefix 24.153.225.0/24
                                 2002::353             0       100     0       ?
 * >      RD: 22:199 IPv4 prefix 30.199.225.0/24
                                 2002::199             0       100     0       ? Or-ID: 20.49.199.199 C-LST: 100.0.0.53 
          RD: 40:336 IPv4 prefix 40.136.225.0/24
                                 2002::336             -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
   %      RD: 10.0.0.57:6001 IPv4 prefix 57.1.0.0/24
                                 2002::57              -       100     0       65000 i Or-ID: 10.0.0.57 C-LST: 100.0.0.53 0.231.244.180 
   %      RD: 100:2 IPv4 prefix 128.219.225.0/24
                                 2002::419             -       0       0       i Or-ID: 192.0.0.1 C-LST: 100.0.0.53 
          RD: 129:11 IPv4 prefix 129.11.225.0/24
                                 2002::11              -       100     0       ? Or-ID: 10.0.0.11 C-LST: 100.0.0.53 
          RD: 129:20 IPv4 prefix 129.20.225.0/24
                                 2002::20              0       100     0       ? Or-ID: 10.0.0.20 C-LST: 100.0.0.53 
          RD: 129:29 IPv4 prefix 129.29.225.0/24
                                 2002::29              0       100     0       ? Or-ID: 10.0.0.29 C-LST: 100.0.0.53 
          RD: 129:36 IPv4 prefix 129.36.225.0/24
                                 2002::36              0       100     0       ? Or-ID: 192.168.20.36 C-LST: 100.0.0.53 
          RD: 10.0.0.59:129 IPv4 prefix 129.58.225.0/24
                                 2002::58              -       100     0       i Or-ID: 10.0.0.58 C-LST: 100.0.0.53 
          RD: 1:129 IPv4 prefix 129.59.225.0/24
                                 2002::59              -       100     0       i Or-ID: 0.231.244.180 C-LST: 100.0.0.53 
          RD: 129:302 IPv4 prefix 129.102.225.0/24
                                 2002::302             -       100     0       i Or-ID: 10.0.1.2 C-LST: 100.0.0.53 
          RD: 129:307 IPv4 prefix 129.107.225.0/24
                                 2002::307             -       100     0       i Or-ID: 10.0.1.7 C-LST: 100.0.0.53 
          RD: 129:310 IPv4 prefix 129.110.225.0/24
                                 2002::310             -       100     0       i Or-ID: 10.0.1.10 C-LST: 100.0.0.53 
          RD: 129:336 IPv4 prefix 129.136.225.0/24
                                 2002::336             -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
          RD: 129:338 IPv4 prefix 129.138.225.0/24
                                 2002::338             -       100     0       ? Or-ID: 10.0.1.38 C-LST: 100.0.0.53 
          RD: 129:342 IPv4 prefix 129.142.225.0/24
                                 2002::342             0       100     0       ? Or-ID: 100.0.0.42 C-LST: 100.0.0.53 
          RD: 129:353 IPv4 prefix 129.153.225.0/24
                                 2002::353             0       100     0       ?
   %      RD: 100:3 IPv4 prefix 129.219.225.0/24
                                 2002::419             -       0       0       i Or-ID: 192.0.0.1 C-LST: 100.0.0.53 
 * >      RD: 130:11 IPv4 prefix 130.11.225.0/24
                                 2002::11              -       100     0       ? Or-ID: 10.0.0.11 C-LST: 100.0.0.53 
          RD: 130:36 IPv4 prefix 130.36.225.0/24
                                 2002::36              0       100     0       ? Or-ID: 192.168.20.36 C-LST: 100.0.0.53 
 * >      RD: 10.0.0.59:130 IPv4 prefix 130.58.225.0/24
                                 2002::58              -       100     0       i Or-ID: 10.0.0.58 C-LST: 100.0.0.53 
 * >      RD: 1:130 IPv4 prefix 130.59.225.0/24
                                 2002::59              -       100     0       i Or-ID: 0.231.244.180 C-LST: 100.0.0.53 
          RD: 130:336 IPv4 prefix 130.136.225.0/24
                                 2002::336             -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
          RD: 130:338 IPv4 prefix 130.138.225.0/24
                                 2002::338             -       100     0       ? Or-ID: 10.0.1.38 C-LST: 100.0.0.53 
   %      RD: 100:4 IPv4 prefix 130.219.225.0/24
                                 2002::419             -       0       0       i Or-ID: 192.0.0.1 C-LST: 100.0.0.53 
 * >      RD: 10.0.0.59:131 IPv4 prefix 131.58.225.0/24
                                 2002::58              -       100     0       i Or-ID: 10.0.0.58 C-LST: 100.0.0.53 
 * >      RD: 1:131 IPv4 prefix 131.59.225.0/24
                                 2002::59              -       100     0       i Or-ID: 0.231.244.180 C-LST: 100.0.0.53 
          RD: 131:336 IPv4 prefix 131.136.225.0/24
                                 2002::336             -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
          RD: 131:338 IPv4 prefix 131.138.225.0/24
                                 2002::338             -       100     0       ? Or-ID: 10.0.1.38 C-LST: 100.0.0.53 
   %      RD: 100:5 IPv4 prefix 131.219.225.0/24
                                 2002::419             -       0       0       i Or-ID: 192.0.0.1 C-LST: 100.0.0.53 
   %      RD: 100:6 IPv4 prefix 132.219.225.0/24
                                 2002::419             -       0       0       i Or-ID: 192.0.0.1 C-LST: 100.0.0.53 
   %      RD: 100:7 IPv4 prefix 133.219.225.0/24
                                 2002::419             -       0       0       i Or-ID: 192.0.0.1 C-LST: 100.0.0.53 
   %      RD: 100:8 IPv4 prefix 134.219.225.0/24
                                 2002::419             -       0       0       i Or-ID: 192.0.0.1 C-LST: 100.0.0.53 
```

## show bgp neighbors 2002::353 vpn-ipv6 advertised-routes

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast, q - Queued for advertisement
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 2000:161 IPv6 prefix 2001:3024:161:225::/64
                                 2002::161             -       100     0       i
```

## show bgp neighbors 2002::353 vpn-ipv6 received-routes

```text
BGP routing table information for VRF default
Router identifier 100.0.0.161, local AS number 1
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
   %      RD: 10.0.0.103:8 IPv6 prefix 2001:0:83:111::/64
                                 2002::303             -       100     0       65000 i Or-ID: 192.168.21.3 C-LST: 100.0.0.53 0.231.244.180 
 * >      RD: 1011:1 IPv6 prefix 2001:20:11:225::/64
                                 2002::11              -       100     0       ? Or-ID: 10.0.0.11 C-LST: 100.0.0.53 
 * >      RD: 1:20 IPv6 prefix 2001:20:20:225::/64
                                 2002::20              0       100     0       ? Or-ID: 10.0.0.20 C-LST: 100.0.0.53 
 * >      RD: 1:28 IPv6 prefix 2001:20:28:225::/64
                                 2002::28              0       100     0       ? Or-ID: 10.0.0.28 C-LST: 100.0.0.53 
 * >      RD: 1:29 IPv6 prefix 2001:20:29:225::/64
                                 2002::29              0       100     0       ? Or-ID: 10.0.0.29 C-LST: 100.0.0.53 
 * >      RD: 1:36 IPv6 prefix 2001:20:36:225::/64
                                 2002::36              0       100     0       ? Or-ID: 192.168.20.36 C-LST: 100.0.0.53 
 * >      RD: 1:58 IPv6 prefix 2001:20:58:225::/64
                                 2002::58              -       100     0       i Or-ID: 10.0.0.58 C-LST: 100.0.0.53 
 * >      RD: 1:59 IPv6 prefix 2001:20:59:225::/64
                                 2002::59              -       100     0       i Or-ID: 0.231.244.180 C-LST: 100.0.0.53 
 * >      RD: 1:302 IPv6 prefix 2001:20:102:225::/64
                                 2002::302             -       100     0       i Or-ID: 10.0.1.2 C-LST: 100.0.0.53 
 * >      RD: 1:307 IPv6 prefix 2001:20:107:225::/64
                                 2002::307             -       100     0       i Or-ID: 10.0.1.7 C-LST: 100.0.0.53 
 * >      RD: 1:310 IPv6 prefix 2001:20:110:225::/64
                                 2002::310             -       100     0       i Or-ID: 10.0.1.10 C-LST: 100.0.0.53 
 * >      RD: 1:342 IPv6 prefix 2001:20:142:225::/64
                                 2002::342             0       100     0       ? Or-ID: 100.0.0.42 C-LST: 100.0.0.53 
 * >      RD: 1:344 IPv6 prefix 2001:20:144:225::/64
                                 2002::344             0       100     0       ? Or-ID: 100.0.0.44 C-LST: 100.0.0.53 
 * >      RD: 1:352 IPv6 prefix 2001:20:152:225::/64
                                 2002::352             0       100     0       ? Or-ID: 100.0.0.52 C-LST: 100.0.0.53 
 * >      RD: 1:353 IPv6 prefix 2001:20:153:225::/64
                                 2002::353             0       100     0       ?
 * >      RD: 1:199 IPv6 prefix 2001:20:199:225::/64
                                 2002::199             0       100     0       ? Or-ID: 20.49.199.199 C-LST: 100.0.0.53 
 * >      RD: 1:336 IPv6 prefix 2001:20:336:225::/64
                                 2002::336             -       100     0       ? Or-ID: 10.0.1.36 C-LST: 100.0.0.53 
          RD: 1:21 IPv6 prefix 2001:21:20:225::/64
                                 2002::20              0       100     0       ? Or-ID: 10.0.0.20 C-LST: 100.0.0.53 
 * >      RD: 21:302 IPv6 prefix 2001:21:102:225::/64
                                 2002::302             -       100     0       i Or-ID: 10.0.1.2 C-LST: 100.0.0.53 
          RD: 21:307 IPv6 prefix 2001:21:107:225::/64
                                 2002::307             -       100     0       i Or-ID: 10.0.1.7 C-LST: 100.0.0.53 
 * >      RD: 21:310 IPv6 prefix 2001:21:110:225::/64
                                 2002::310             -       100     0       i Or-ID: 10.0.1.10 C-LST: 100.0.0.53 
          RD: 129:20 IPv6 prefix 2001:129:20:225::/64
                                 2002::20              0       100     0       ? Or-ID: 10.0.0.20 C-LST: 100.0.0.53 
          RD: 129:29 IPv6 prefix 2001:129:29:225::/64
                                 2002::29              0       100     0       ? Or-ID: 10.0.0.29 C-LST: 100.0.0.53 
          RD: 129:302 IPv6 prefix 2001:129:102:225::/64
                                 2002::302             -       100     0       i Or-ID: 10.0.1.2 C-LST: 100.0.0.53 
          RD: 129:307 IPv6 prefix 2001:129:107:225::/64
                                 2002::307             -       100     0       i Or-ID: 10.0.1.7 C-LST: 100.0.0.53 
          RD: 129:310 IPv6 prefix 2001:129:110:225::/64
                                 2002::310             -       100     0       i Or-ID: 10.0.1.10 C-LST: 100.0.0.53 
   %      RD: 10.0.0.57:1 IPv6 prefix 2600:50:10:57::/64
                                 2002::57              -       100     0       65000 i Or-ID: 10.0.0.57 C-LST: 100.0.0.53 0.231.244.180 
   %      RD: 10.0.0.57:6001 IPv6 prefix 5757:1::/64
                                 2002::57              -       100     0       65000 i Or-ID: 10.0.0.57 C-LST: 100.0.0.53 0.231.244.180 
```

## show ipv6 route vrf T5-SR-IPVPN-SRv6-GW

```text

VRF: T5-SR-IPVPN-SRv6-GW
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
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 595, SRv6 SID fcbb:0:1011:e001::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:20:225::/64 [200/0]
           via fcbb:0:20::/48, SRv6 Transport tunnel index 603, SRv6 SID fcbb:0:20:e122::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:28:225::/64 [200/0]
           via fcbb:0:28::/48, SRv6 Transport tunnel index 593, SRv6 SID fcbb:0:28:e101::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:29:225::/64 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 595, SRv6 SID fcbb:0:1029:e101::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:36:225::/64 [200/0]
           via fcbb:0:36::/48, SRv6 Transport tunnel index 594, SRv6 SID fcbb:0:36:e027::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:58:225::/64 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 595, SRv6 SID fcbb:0:1058:e029::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:59:225::/64 [200/0]
           via fcbb:0:59::/48, SRv6 Transport tunnel index 602, SRv6 SID fcbb:0:59:e018::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:102:225::/64 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 595, SRv6 SID fcbb:0:1302:e004::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:107:225::/64 [200/0]
           via fcbb:0:307::/48, SRv6 Transport tunnel index 597, SRv6 SID fcbb:0:307:e004::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:110:225::/64 [200/0]
           via fcbb:0:1310::/48, SRv6 Transport tunnel index 600, SRv6 SID fcbb:0:1310:e015::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:142:225::/64 [200/0]
           via fcbb:0:342::/48, SRv6 Transport tunnel index 609, SRv6 SID fcbb:0:342:e012::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:144:225::/64 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 595, SRv6 SID fcbb:0:1344:e013::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:152:225::/64 [200/0]
           via fcbb:0:352::/48, SRv6 Transport tunnel index 598, SRv6 SID fcbb:0:352:e015::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:153:225::/64 [200/0]
           via fcbb:0:1353::/48, SRv6 Transport tunnel index 605, SRv6 SID fcbb:0:1353:e004::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:199:225::/64 [200/0]
           via fcbb:0:1000::/36, SRv6 Transport tunnel index 595, SRv6 SID fcbb:0:1199:e026::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 B I      2001:20:336:225::/64 [200/0]
           via fcbb:0:336::/48, SRv6 Transport tunnel index 599, SRv6 SID fcbb:0:336:e664::
              via fe80::fa7a:41ff:fe18:8910, Ethernet10
 C        2001:3024:161:225::/64 [0/0]
           via Vlan3024, directly connected

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

 B I      20.10.31.31/32 [200/0]
           via 100.0.0.31/32, IS-IS SR tunnel index 13, label 756647
              via 20.161.180.180, Ethernet45/1, label 900031
 B I      20.10.31.254/32 [200/0]
           via 100.0.0.31/32, IS-IS SR tunnel index 13, label 756647
              via 20.161.180.180, Ethernet45/1, label 900031
 B I      20.10.31.0/24 [200/0]
           via 100.0.0.31/32, IS-IS SR tunnel index 13, label 756647
              via 20.161.180.180, Ethernet45/1, label 900031
 B I      20.10.32.32/32 [200/0]
           via 100.0.37.9/32, IS-IS SR tunnel index 5, label 354
              via 20.161.180.180, Ethernet45/1, label 900379
 B I      20.10.32.201/32 [200/0]
           via 100.0.37.9/32, IS-IS SR tunnel index 5, label 354
              via 20.161.180.180, Ethernet45/1, label 900379
 B I      20.10.32.0/24 [200/0]
           via 100.0.37.9/32, IS-IS SR tunnel index 5, label 354
              via 20.161.180.180, Ethernet45/1, label 900379
 B I      20.10.56.0/24 [200/0]
           via 100.0.0.56/32, IS-IS SR tunnel index 10, label 524281
              via 20.161.180.180, Ethernet45/1, label 900056
 B I      20.30.1.68/32 [200/0]
           via 100.0.0.182/32, IS-IS SR tunnel index 17, label 362146
              via 20.161.180.180, Ethernet45/1, label 900182
 B I      20.30.1.0/24 [200/0]
           via 100.0.0.56/32, IS-IS SR tunnel index 10, label 524281
              via 20.161.180.180, Ethernet45/1, label 900056
 B I      20.30.2.0/24 [200/0]
           via 100.0.0.56/32, IS-IS SR tunnel index 10, label 524281
              via 20.161.180.180, Ethernet45/1, label 900056
 B I      20.30.3.0/24 [200/0]
           via 100.0.0.56/32, IS-IS SR tunnel index 10, label 524281
              via 20.161.180.180, Ethernet45/1, label 900056
 B I      20.30.4.0/24 [200/0]
           via 100.0.0.56/32, IS-IS SR tunnel index 10, label 524281
              via 20.161.180.180, Ethernet45/1, label 900056
 C        220.161.225.0/24
           directly connected, Vlan3024

```

