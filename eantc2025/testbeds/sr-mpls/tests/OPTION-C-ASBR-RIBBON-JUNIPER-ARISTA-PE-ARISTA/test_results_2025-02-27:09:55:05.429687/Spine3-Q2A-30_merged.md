# Test results for Spine3-Q2A-30

## show version

```text
Arista DCS-7280SR3E-40YC6-F
Hardware version: 11.00
Serial number: SGD22060176
Hardware MAC address: c4ca.2b45.a215
System MAC address: c4ca.2b45.a215

Software image version: 4.33.1.1F
Architecture: x86_64
Internal build version: 4.33.1.1F-40155285.43311F
Internal build ID: 2170da2c-90c5-421e-adc1-86266708cffc
Image format version: 3.0
Image optimization: Default

Uptime: 6 days, 19 hours and 17 minutes
Total memory: 8099700 kB
Free memory: 4742484 kB

```

## show interfaces counters rates | nz

```text
Port      Name                 Intvl  In Mbps      %  In Kpps Out Mbps      %
Et1       Arista_PE31_31        0:01      4.2   0.0%        5      3.8   0.0%
Et2       Arista-PE32-Q2C-32 E  0:01      4.0   0.0%        5      4.2   0.0%
Et9       Ciena-5134-72 port 2  0:01      0.0   0.0%        0      0.0   0.0%
Et11      Juniper-156 port 590  0:01      0.0   0.0%        0      0.0   0.0%
Et21      Juniper-156 port 592  0:01      0.0   0.0%        0      0.0   0.0%
Et22      "Link to Juniper 179  0:01      0.0   0.0%        0      0.0   0.0%
Et31      Ciena-8140-66 port 2  0:01      0.0   0.0%        0      0.0   0.0%
Et35      Juniper-131-JCNR 42   0:01      0.0   0.0%        0      0.0   0.0%

Port      Out Kpps
Et1              5
Et2              5
```

## show ip interface brief | exclude una

```text
                                                                        Address
Interface          IP Address        Status      Protocol          MTU  Owner  
------------------ ----------------- ----------- --------------- ------ -------
Ethernet1          20.30.31.30/24    up          up               1500         
Ethernet2          20.30.32.30/24    up          up               1500         
Ethernet3          20.30.120.30/24   up          up               1500         
Ethernet4          20.30.217.30/24   admin down  down             1500         
Ethernet5          20.30.214.30/24   up          up               1500         
Ethernet6          21.30.214.30/24   down        down             1500         
Ethernet7          20.30.184.30/24   down        down             1500         
Ethernet8          21.30.217.30/24   admin down  down             1500         
Ethernet9          20.30.72.30/24    up          up               1500         
Ethernet10         21.30.120.30/24   admin down  down             1500         
Ethernet11         20.30.156.30/24   down        down             1500         
Ethernet12         20.30.84.30/24    up          up               1500         
Ethernet13         20.30.53.30/24    down        down             1500         
Ethernet14         20.30.122.30/24   up          up               1500         
Ethernet15         20.30.221.30/24   down        down             1500         
Ethernet16         21.30.84.30/24    admin down  down             1500         
Ethernet17         20.30.124.30/24   admin down  down             1500         
Ethernet18         21.30.124.30/24   down        down             1500         
Ethernet19         20.30.128.30/24   admin down  down             1500         
Ethernet20         21.30.128.30/24   down        notpresent       1500         
Ethernet21         21.30.156.30/24   admin down  down             1500         
Ethernet29         21.30.32.30/24    admin down  down             1500         
Ethernet31         20.30.66.30/24    up          up               1500         
Ethernet35         20.30.131.30/24   admin down  down             1500         
Ethernet40         20.30.179.30/24   admin down  down             1500         
Ethernet46/1.71    50.10.30.1/24     down        lowerlayerdown   1500         
Loopback0          10.0.0.30/32      up          up              65535         
Loopback1000       10.0.30.30/32     up          up              65535         
Loopback5001       10.0.0.30/32      up          up              65535         
Loopback5128       10.128.0.30/32    up          up              65535         
Loopback7001       10.0.30.30/32     up          up              65535         
Management1        192.168.20.30/23  up          up               1500         

```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
IGP       default  Arista-PE31-Q2C-31 L2   Ethernet1          P2P               UP    29          2B                  
IGP       default  Arista-PE32-Q2C-32 L2   Ethernet2          P2P               UP    23          44                  
IGP       default  Ciena-8140-66    L2   Ethernet31         P2P               UP    22          01                  
IGP       default  Ciena-5134-72    L2   Ethernet9          P2P               UP    21          01                  
IGP       default  Ericsson_84_R6678 L2   Ethernet12         P2P               UP    21          02                  
IGP       default  0000.0000.0120   L2   Ethernet3          P2P               UP    22          01                  
IGP       default  0000.0000.0122   L2   Ethernet14         P2P               UP    29          01                  
IGP       default  Nokia-SXR-214    L2   Ethernet5          P2P               UP    20          00                  
```

## show isis database detail

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: 2-23-5G VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-2-23.00-00       320  42015  1105    123 L2  0000.0000.3030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 805 s
      NLPID: 0xCC(IPv4)
      Hostname: Arista-Spine3-Q2A-2-23
      Area addresses: 49.0001
      Interface address: 10.0.30.30
      Reachability         : 10.0.30.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 330 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.30.30 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000

Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00      7332  39141  1090    988 L2  0000.0000.0030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 790 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-Spine3-Q2A-30
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.30.122.30
      Interface address: 20.30.120.30
      Interface address: 20.30.32.30
      Interface address: 20.30.31.30
      Interface address: 20.30.214.30
      Interface address: 20.30.84.30
      Interface address: 20.30.72.30
      Interface address: 20.30.66.30
      Interface address: 10.0.0.30
      Interface address: 2001:0:30:120::30
      Interface address: 2001:0:30:32::30
      Interface address: 2001:0:30:214::30
      Interface address: 2001:0:30:84::30
      Interface address: 2001:0:30:72::30
      Interface address: 2001:0:30:66::30
      Interface address: 2002::30
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 50
        IPv4 Neighbor Address: 20.30.32.32
        IPv4 Interface Address: 20.30.32.30
        Adj-sid: 378650 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 100
        IPv4 Neighbor Address: 20.30.214.214
        IPv4 Interface Address: 20.30.214.30
        Adj-sid: 378660 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-8140-66.00    Metric: 100
        IPv4 Neighbor Address: 20.30.66.66
        IPv4 Interface Address: 20.30.66.30
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 100
        IPv4 Neighbor Address: 20.30.84.84
        IPv4 Interface Address: 20.30.84.30
        Adj-sid: 378648 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-5134-72.00    Metric: 100
        IPv4 Neighbor Address: 20.30.72.72
        IPv4 Interface Address: 20.30.72.30
        Adj-sid: 378684 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-PE32-Q2C-32.00 Metric: 10
        Adj-sid: 378651 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Ericsson_84_R6678.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:84::175
        Global IPv6 Interface Address: 2001:0:30:84::30
        Adj-sid: 378649 flags: [L V F] weight: 0x0
      Reachability         : 20.30.122.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.30.120.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.30.32.0/24 Metric: 50 Type: 1 Up
      Reachability         : 20.30.31.0/24 Metric: 75 Type: 1 Up
      Reachability         : 20.30.214.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.30.84.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.30.66.0/24 Metric: 100 Type: 1 Up
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
        SR Prefix-SID: 158 Flags: [N] Algorithm: 128
        SR Prefix-SID: 159 Flags: [N] Algorithm: 129
        SR Prefix-SID: 160 Flags: [N] Algorithm: 130
      Reachability (MT-IPv6): 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:32::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:72::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:66::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::30/128 Metric: 10 Type: 1 Up
        SR Prefix-SID: 430 Flags: [N] Algorithm: 0
        SR Prefix-SID: 558 Flags: [N] Algorithm: 128
        SR Prefix-SID: 559 Flags: [N] Algorithm: 129
        SR Prefix-SID: 560 Flags: [N] Algorithm: 130
      Router Capabilities: Router Id: 10.0.0.30 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 237
          Exclude admin groups: 1
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 255
    Arista-Spine3-Q2A-30.00-01        98  38964   808    305 L2  0000.0000.0030.00-01  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 508 s
      Interface address: 2001:0:30:31::30
      IS Neighbor          : 0000.0000.0120.00   Metric: 100
        IPv4 Neighbor Address: 20.30.120.120
        IPv4 Interface Address: 20.30.120.30
        Adj-sid: 378652 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0122.00   Metric: 100
        IPv4 Neighbor Address: 20.30.122.122
        IPv4 Interface Address: 20.30.122.30
        Adj-sid: 378700 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE31-Q2C-31.00 Metric: 75
        IPv4 Neighbor Address: 20.30.31.31
        IPv4 Interface Address: 20.30.31.30
        Adj-sid: 378688 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-PE31-Q2C-31.00 Metric: 10
        Adj-sid: 378689 flags: [L V F] weight: 0x0
      Reachability (MT-IPv6): 2001:0:30:31::/64 Metric: 10 Type: 1 Up
    Arista-PE31-Q2C-31.00-00      1013   2713  1157    266 L2  0000.0000.0031.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE31-Q2C-31
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 10.0.0.31
      Interface address: 20.30.31.31
      Interface address: 2002::31
      Interface address: 2001:0:30:31::31
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.31.30
        IPv4 Interface Address: 20.30.31.31
        Adj-sid: 394917 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        Adj-sid: 394918 flags: [L V F] weight: 0x0
      Reachability         : 10.0.0.31/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 31 Flags: [N] Algorithm: 0
      Reachability         : 20.30.31.0/24 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::31/128 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:31::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.31 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
    Arista-PE32-Q2C-32.00-00      1145   3373  1038    308 L2  0000.0000.0032.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE32-Q2C-32
      Area addresses: 49.0002
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 209.209.209.202
      Interface address: 20.30.32.32
      Interface address: 10.0.0.32
      Interface address: 2001:0:30:32::32
      Interface address: 2002::32
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.32.30
        IPv4 Interface Address: 20.30.32.32
        Adj-sid: 362144 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        Adj-sid: 362145 flags: [L V F] weight: 0x0
      Reachability         : 10.0.0.175/32 Metric: 10 Type: 1 Down
        SR Prefix-SID: 175 Flags: [R N P] Algorithm: 0
      Reachability         : 209.209.209.202/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 202 Flags: [P] Algorithm: 0
      Reachability         : 20.30.32.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.32/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 32 Flags: [N] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:30:32::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::32/128 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.32 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
    Ciena-8140-66.00-00          17  60850  1112    112 L2  0000.0000.0067.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-8140-66
      Area addresses: 49.0002
      Topology: 0 (IPv4)
      Interface address: 20.30.66.66
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
      Reachability         : 10.0.0.66/32 Metric: 0 Type: 1 Up
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 209.209.209.202/32 Metric: 0 Type: 1 Up
    Ciena-5134-72.00-00         294  59575   836    209 L2  0000.0000.0072.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-5134-72
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.72
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.72.30
        IPv4 Interface Address: 20.30.72.72
        Adj-sid: 16005 flags: [L V] weight: 0x0
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.72/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 72 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.72 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ericsson_84_R6678.00-00      1160   2971   653    238 L2  0000.0000.0084.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Ericsson_84_R6678
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.84
      Interface address: 2001:0:30:84::175
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Interface Address: 20.30.84.84
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:84::30
        Global IPv6 Interface Address: 2001:0:30:84::175
      Reachability         : 10.0.0.84/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 84 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.84 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    0000.0000.0120.00-00       7022  22021   962    381 L2  0000.0000.0120.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Interface address: 20.30.120.120
      Interface address: 209.209.209.202
      Interface address: 2001:0:30:120::120
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.120.30
        IPv4 Interface Address: 20.30.120.120
        IPv6 Neighbor Address: 2001:0:30:120::30
        Global IPv6 Interface Address: 2001:0:30:120::120
        Adj-sid: 1144 flags: [L V] weight: 0x0
        Adj-sid: 1143 flags: [L V F] weight: 0x0
      Reachability         : 10.0.0.120/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 120 Flags: [R P] Algorithm: 0
      Reachability         : 10.0.0.175/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 120 Flags: [R P] Algorithm: 0
      Reachability         : 20.30.120.0/24 Metric: 10 Type: 1 Up
      Reachability         : 209.209.209.202/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 202 Flags: [N] Algorithm: 0
      Reachability          : 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:120:175::/64 Metric: 0 Type: 1 Up
        SR Prefix-SID: 120 Flags: [R P] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.120 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  13
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
    0000.0000.0122.00-00        376  12696  1157    467 L2  0000.0000.0122.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Interface address: 10.0.0.122
      Interface address: 20.30.122.122
      Interface address: 2001:0:30:122::30
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.122.30
        IPv4 Interface Address: 20.30.122.122
        Adj-sid: 1147 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.122/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 122 Flags: [N] Algorithm: 0
      Reachability         : 20.30.122.0/24 Metric: 10 Type: 1 Up
      Reachability         : 30.122.190.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.64.122.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.74.122.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.88.122.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.119.122.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.122.125.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.122.130.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.122.158.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.122.162.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.122.169.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.122.216.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.122.218.0/24 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:30:122::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:87:122::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:122:162::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:122:169::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:122:188::/64 Metric: 0 Type: 1 Up
      Reachability          : 2002::122/128 Metric: 0 Type: 1 Up
      Reachability          : 2600:30:122:190::/64 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.122 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  13
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
 U  Juniper-156-PTX10002-36QDD.00-00      2465  48498   413    316 L2  0000.0000.0156.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-156-PTX10002-36QDD
      Area addresses: 49.0001
      Interface address: 10.0.0.156
      Interface address: 209.209.209.202
      Interface address: 2002::156
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.156.30
        IPv4 Interface Address: 20.30.156.156
        IPv6 Neighbor Address: 2001:0:30:156::30
        Global IPv6 Interface Address: 2001:0:30:156::156
        Adj-sid: 40 flags: [L V F] weight: 0x0
        Adj-sid: 39 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.156/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 156 Flags: [N] Algorithm: 0
      Reachability         : 209.209.209.202/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 202 Flags: [N] Algorithm: 0
      Reachability         : 10.0.0.175/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 175 Flags: [N P] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.156 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Nokia-SXR-214.00-00       34879  28493   610    349 L2  0000.0000.0214.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SXR-214
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 209.209.209.202
      Interface address: 10.0.0.214
      Interface address: 20.30.214.214
      Interface address: 2000::214
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.214.30
        IPv4 Interface Address: 20.30.214.214
        Adj-sid: 30049 flags: [L V] weight: 0x0
      Reachability         : 20.30.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.175/32 Metric: 10 Type: 1 Down
        SR Prefix-SID: 175 Flags: [R N P] Algorithm: 0
      Reachability         : 209.209.209.202/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 202 Flags: [P] Algorithm: 0
      Reachability         : 10.0.0.214/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 214 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2000::214/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.214 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  15
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
 U  221.00-00                   107  11306   432     79 L2  0221.0221.0221.00-00  <>
      NLPID: 0xCC(IPv4)
      Area addresses: 49.0001
      Router Capabilities: Router Id: 10.0.0.221 Flags: []
        SR Local Block:
          SRLB Base: 16 Range: 15344
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
      Unsupported TLV: Type: 14 Length: 2
 U  221.00-01                   106   3066   833     32 L2  0221.0221.0221.00-01  <>
      Hostname: 221
 U  221.00-02                   124  28431   475    205 L2  0221.0221.0221.00-02  <>
      Interface address: 20.30.221.221
      Interface address: 10.0.0.221
      Interface address: 209.209.209.202
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 100
        IPv4 Neighbor Address: 20.30.221.30
        IPv4 Interface Address: 20.30.221.221
        Adj-sid: 756648 flags: [L V B] weight: 0x0
        Adj-sid: 756647 flags: [L V] weight: 0x0
      Reachability         : 20.30.221.0/24 Metric: 100 Type: 1 Up
      Reachability         : 10.0.0.221/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 221 Flags: [N] Algorithm: 0
      Reachability         : 209.209.209.202/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 202 Flags: [] Algorithm: 0

```

## show isis database traffic-engineering

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: 2-23-5G VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-2-23.00-00       320  42015  1105    123 L2  0000.0000.3030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 805 s
      NLPID: 0xCC(IPv4)
      Hostname: Arista-Spine3-Q2A-2-23
      Area addresses: 49.0001
      Interface address: 10.0.30.30
      Reachability         : 10.0.30.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 330 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.30.30 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000

Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00      7332  39141  1090    988 L2  0000.0000.0030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 790 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-Spine3-Q2A-30
      TE IPv4 router ID: 10.0.0.30
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.30.122.30
      Interface address: 20.30.120.30
      Interface address: 20.30.32.30
      Interface address: 20.30.31.30
      Interface address: 20.30.214.30
      Interface address: 20.30.84.30
      Interface address: 20.30.72.30
      Interface address: 20.30.66.30
      Interface address: 10.0.0.30
      Interface address: 2001:0:30:120::30
      Interface address: 2001:0:30:32::30
      Interface address: 2001:0:30:214::30
      Interface address: 2001:0:30:84::30
      Interface address: 2001:0:30:72::30
      Interface address: 2001:0:30:66::30
      Interface address: 2002::30
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 50
        IPv4 Neighbor Address: 20.30.32.32
        IPv4 Interface Address: 20.30.32.30
        Adj-sid: 378650 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Nokia-SXR-214.00    Metric: 100
        IPv4 Neighbor Address: 20.30.214.214
        IPv4 Interface Address: 20.30.214.30
        Adj-sid: 378660 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Ciena-8140-66.00    Metric: 100
        IPv4 Neighbor Address: 20.30.66.66
        IPv4 Interface Address: 20.30.66.30
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 100
        IPv4 Neighbor Address: 20.30.84.84
        IPv4 Interface Address: 20.30.84.30
        Adj-sid: 378648 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Ciena-5134-72.00    Metric: 100
        IPv4 Neighbor Address: 20.30.72.72
        IPv4 Interface Address: 20.30.72.30
        Adj-sid: 378684 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor (MT-IPv6): Arista-PE32-Q2C-32.00 Metric: 10
        Adj-sid: 378651 flags: [L V F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor (MT-IPv6): Ericsson_84_R6678.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:84::175
        Global IPv6 Interface Address: 2001:0:30:84::30
        Adj-sid: 378649 flags: [L V F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      Reachability         : 20.30.122.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.30.120.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.30.32.0/24 Metric: 50 Type: 1 Up
      Reachability         : 20.30.31.0/24 Metric: 75 Type: 1 Up
      Reachability         : 20.30.214.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.30.84.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.30.66.0/24 Metric: 100 Type: 1 Up
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
        SR Prefix-SID: 158 Flags: [N] Algorithm: 128
        SR Prefix-SID: 159 Flags: [N] Algorithm: 129
        SR Prefix-SID: 160 Flags: [N] Algorithm: 130
      Reachability (MT-IPv6): 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:32::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:72::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:66::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::30/128 Metric: 10 Type: 1 Up
        SR Prefix-SID: 430 Flags: [N] Algorithm: 0
        SR Prefix-SID: 558 Flags: [N] Algorithm: 128
        SR Prefix-SID: 559 Flags: [N] Algorithm: 129
        SR Prefix-SID: 560 Flags: [N] Algorithm: 130
      Router Capabilities: Router Id: 10.0.0.30 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 237
          Exclude admin groups: 1
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 255
    Arista-Spine3-Q2A-30.00-01        98  38964   808    305 L2  0000.0000.0030.00-01  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 508 s
      Interface address: 2001:0:30:31::30
      IS Neighbor          : 0000.0000.0120.00   Metric: 100
        IPv4 Neighbor Address: 20.30.120.120
        IPv4 Interface Address: 20.30.120.30
        Adj-sid: 378652 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : 0000.0000.0122.00   Metric: 100
        IPv4 Neighbor Address: 20.30.122.122
        IPv4 Interface Address: 20.30.122.30
        Adj-sid: 378700 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Arista-PE31-Q2C-31.00 Metric: 75
        IPv4 Neighbor Address: 20.30.31.31
        IPv4 Interface Address: 20.30.31.30
        Adj-sid: 378688 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor (MT-IPv6): Arista-PE31-Q2C-31.00 Metric: 10
        Adj-sid: 378689 flags: [L V F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      Reachability (MT-IPv6): 2001:0:30:31::/64 Metric: 10 Type: 1 Up
    Arista-PE31-Q2C-31.00-00      1013   2713  1157    266 L2  0000.0000.0031.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE31-Q2C-31
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 10.0.0.31
      Interface address: 20.30.31.31
      Interface address: 2002::31
      Interface address: 2001:0:30:31::31
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.31.30
        IPv4 Interface Address: 20.30.31.31
        Adj-sid: 394917 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        Adj-sid: 394918 flags: [L V F] weight: 0x0
      Reachability         : 10.0.0.31/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 31 Flags: [N] Algorithm: 0
      Reachability         : 20.30.31.0/24 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::31/128 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:31::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.31 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
    Arista-PE32-Q2C-32.00-00      1145   3373  1038    308 L2  0000.0000.0032.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE32-Q2C-32
      Area addresses: 49.0002
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 209.209.209.202
      Interface address: 20.30.32.32
      Interface address: 10.0.0.32
      Interface address: 2001:0:30:32::32
      Interface address: 2002::32
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.32.30
        IPv4 Interface Address: 20.30.32.32
        Adj-sid: 362144 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        Adj-sid: 362145 flags: [L V F] weight: 0x0
      Reachability         : 10.0.0.175/32 Metric: 10 Type: 1 Down
        SR Prefix-SID: 175 Flags: [R N P] Algorithm: 0
      Reachability         : 209.209.209.202/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 202 Flags: [P] Algorithm: 0
      Reachability         : 20.30.32.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.32/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 32 Flags: [N] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:30:32::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::32/128 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.32 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
    Ciena-8140-66.00-00          17  60850  1112    112 L2  0000.0000.0067.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-8140-66
      Area addresses: 49.0002
      Topology: 0 (IPv4)
      Interface address: 20.30.66.66
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        Local link ID: 1073731845
        Remote link ID: 110
      Reachability         : 10.0.0.66/32 Metric: 0 Type: 1 Up
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 209.209.209.202/32 Metric: 0 Type: 1 Up
    Ciena-5134-72.00-00         294  59575   835    209 L2  0000.0000.0072.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-5134-72
      TE IPv4 router ID: 10.0.0.72
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.72
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.72.30
        IPv4 Interface Address: 20.30.72.72
        Adj-sid: 16005 flags: [L V] weight: 0x0
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Local link ID: 1073731838
        Remote link ID: 109
        Application Specific Link Attributes:
          Standard applications: [L] RSVP-TE SR-TE LFA Flex-Algo
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.72/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 72 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.72 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ericsson_84_R6678.00-00      1160   2971   653    238 L2  0000.0000.0084.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Ericsson_84_R6678
      TE IPv4 router ID: 10.0.0.84
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.84
      Interface address: 2001:0:30:84::175
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Interface Address: 20.30.84.84
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:84::30
        Global IPv6 Interface Address: 2001:0:30:84::175
      Reachability         : 10.0.0.84/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 84 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.84 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    0000.0000.0120.00-00       7022  22021   962    381 L2  0000.0000.0120.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      TE IPv4 router ID: 10.0.0.120
      Area addresses: 49.0001
      Interface address: 20.30.120.120
      Interface address: 209.209.209.202
      Interface address: 2001:0:30:120::120
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.120.30
        IPv4 Interface Address: 20.30.120.120
        IPv6 Neighbor Address: 2001:0:30:120::30
        Global IPv6 Interface Address: 2001:0:30:120::120
        Adj-sid: 1144 flags: [L V] weight: 0x0
        Adj-sid: 1143 flags: [L V F] weight: 0x0
        TE default metric: 10
        Maximum link BW: 0.00 bps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
        Local link ID: 1
        Remote link ID: 135
      Reachability         : 10.0.0.120/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 120 Flags: [R P] Algorithm: 0
      Reachability         : 10.0.0.175/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 120 Flags: [R P] Algorithm: 0
      Reachability         : 20.30.120.0/24 Metric: 10 Type: 1 Up
      Reachability         : 209.209.209.202/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 202 Flags: [N] Algorithm: 0
      Reachability          : 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:120:175::/64 Metric: 0 Type: 1 Up
        SR Prefix-SID: 120 Flags: [R P] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.120 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  13
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
    0000.0000.0122.00-00        376  12696  1157    467 L2  0000.0000.0122.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      TE IPv4 router ID: 10.0.0.122
      Area addresses: 49.0001
      Interface address: 10.0.0.122
      Interface address: 20.30.122.122
      Interface address: 2001:0:30:122::30
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.122.30
        IPv4 Interface Address: 20.30.122.122
        Adj-sid: 1147 flags: [L V] weight: 0x0
        TE default metric: 10
        Maximum link BW: 0.00 bps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
        Local link ID: 1
        Remote link ID: 158
      Reachability         : 10.0.0.122/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 122 Flags: [N] Algorithm: 0
      Reachability         : 20.30.122.0/24 Metric: 10 Type: 1 Up
      Reachability         : 30.122.190.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.64.122.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.74.122.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.88.122.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.119.122.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.122.125.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.122.130.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.122.158.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.122.162.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.122.169.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.122.216.0/24 Metric: 0 Type: 1 Up
      Reachability         : 101.122.218.0/24 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:30:122::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:87:122::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:122:162::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:122:169::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:122:188::/64 Metric: 0 Type: 1 Up
      Reachability          : 2002::122/128 Metric: 0 Type: 1 Up
      Reachability          : 2600:30:122:190::/64 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.122 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  13
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
 U  Juniper-156-PTX10002-36QDD.00-00      2465  48498   413    316 L2  0000.0000.0156.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-156-PTX10002-36QDD
      TE IPv4 router ID: 10.0.0.156
      TE IPv6 router ID: 2002::156
      Area addresses: 49.0001
      Interface address: 10.0.0.156
      Interface address: 209.209.209.202
      Interface address: 2002::156
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.156.30
        IPv4 Interface Address: 20.30.156.156
        IPv6 Neighbor Address: 2001:0:30:156::30
        Global IPv6 Interface Address: 2001:0:30:156::156
        Adj-sid: 40 flags: [L V F] weight: 0x0
        Adj-sid: 39 flags: [L V] weight: 0x0
        Local link ID: 1009
        Remote link ID: 56
      Reachability         : 10.0.0.156/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 156 Flags: [N] Algorithm: 0
      Reachability         : 209.209.209.202/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 202 Flags: [N] Algorithm: 0
      Reachability         : 10.0.0.175/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 175 Flags: [N P] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.156 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Nokia-SXR-214.00-00       34879  28493   610    349 L2  0000.0000.0214.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SXR-214
      TE IPv4 router ID: 10.0.0.214
      TE IPv6 router ID: 2000::214
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 209.209.209.202
      Interface address: 10.0.0.214
      Interface address: 20.30.214.214
      Interface address: 2000::214
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.214.30
        IPv4 Interface Address: 20.30.214.214
        Adj-sid: 30049 flags: [L V] weight: 0x0
        TE default metric: 10
        Maximum link BW: 80.00 Mbps
        Application Specific Link Attributes:
          Standard applications: [L] SR-TE
      Reachability         : 20.30.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.175/32 Metric: 10 Type: 1 Down
        SR Prefix-SID: 175 Flags: [R N P] Algorithm: 0
      Reachability         : 209.209.209.202/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 202 Flags: [P] Algorithm: 0
      Reachability         : 10.0.0.214/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 214 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2000::214/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.214 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  15
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
      Shared Risk Link Group:  Neighbor Arista-Spine3-Q2A-30.00 (Numbered)
        Interface Address: 20.30.214.214
        Neighbor Address: 20.30.214.30
        Group ID: 1
      Application Specific Shared Risk Link Group:  Neighbor Arista-Spine3-Q2A-30.00
        Standard applications: [L] SR-TE
        Local link identifier: 10
        Remote link identifier: 49
        IPv4 interface address: 20.30.214.214
        IPv4 neighbor address: 20.30.214.30
 U  221.00-00                   107  11306   432     79 L2  0221.0221.0221.00-00  <>
      NLPID: 0xCC(IPv4)
      TE IPv4 router ID: 10.0.0.221
      Area addresses: 49.0001
      Router Capabilities: Router Id: 10.0.0.221 Flags: []
        SR Local Block:
          SRLB Base: 16 Range: 15344
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
      Unsupported TLV: Type: 14 Length: 2
 U  221.00-01                   106   3066   833     32 L2  0221.0221.0221.00-01  <>
      Hostname: 221
 U  221.00-02                   124  28431   475    205 L2  0221.0221.0221.00-02  <>
      Interface address: 20.30.221.221
      Interface address: 10.0.0.221
      Interface address: 209.209.209.202
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 100
        IPv4 Neighbor Address: 20.30.221.30
        IPv4 Interface Address: 20.30.221.221
        Adj-sid: 756648 flags: [L V B] weight: 0x0
        Adj-sid: 756647 flags: [L V] weight: 0x0
        Administrative group (Color): ARISTA(2)
        TE default metric: 100
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Min/Max unidirectional link delay: 100/100 us
      Reachability         : 20.30.221.0/24 Metric: 100 Type: 1 Up
      Reachability         : 10.0.0.221/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 221 Flags: [N] Algorithm: 0
      Reachability         : 209.209.209.202/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 202 Flags: [] Algorithm: 0

```

## show isis flex-algo path

```text
Flex algo paths for IPv4 address family
Topology ID: Level-2
   Destination                Algorithm         Next Hop    Interface
-------------------------- ----------------- -------------- ---------
   Arista-Spine3-Q2A-30       MIN-LATENCY                            
                                                                     
   Arista-Spine3-Q2A-30       MIN-TE                                 
                                                                     
   Arista-Spine3-Q2A-30       ADMIN                                  
                                                                     

Flex algo paths for IPv6 address family
Topology ID: Level-2
   Destination                Algorithm         Next Hop    Interface
-------------------------- ----------------- -------------- ---------
   Arista-Spine3-Q2A-30       MIN-LATENCY                            
                                                                     
   Arista-Spine3-Q2A-30       MIN-TE                                 
                                                                     
   Arista-Spine3-Q2A-30       ADMIN                                  
                                                                     

```

## show isis flex-algo path detail

```text
Flex algo paths for IPv4 address family
Topology ID: Level-2
Destination: Arista-Spine3-Q2A-30
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 20:26:39 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 20:26:39 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 20:26:39 ago
Next Hop Interface
-------- ---------

Flex algo paths for IPv6 address family
Topology ID: Level-2
Destination: Arista-Spine3-Q2A-30
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 20:26:39 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 20:26:39 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 20:26:39 ago
Next Hop Interface
-------- ---------

```

## show isis segment-routing tunnel

```text
 Index    Endpoint              Next Hop/Tunnel Index    Interface    Labels   
-------- --------------------- ------------------------ ------------- ---------
 7        10.0.0.175/32         TI-LFA (2)               -            [ 20175 ]
 8        10.0.0.84/32          20.30.84.84              Ethernet12   [ 20084 ]
 14       10.0.0.72/32          20.30.72.72              Ethernet9    [ 3 ]    
 17       10.0.0.120/32         20.30.120.120            Ethernet3    [ 20120 ]
 20       10.0.0.32/32          20.30.32.32              Ethernet2    [ 3 ]    
 21       10.0.0.214/32         20.30.214.214            Ethernet5    [ 20214 ]
 33       209.209.209.202/32    TI-LFA (3)               -            [ 3 ]    
 34       10.0.0.31/32          20.30.31.31              Ethernet1    [ 3 ]    
 35       10.0.0.122/32         20.30.122.122            Ethernet14   [ 3 ]    

```

## show isis segment-routing prefix-segments

```text

System ID: Arista-Spine3-Q2A-2-23			Instance: '2-23-5G'
SR supported Data-plane: MPLS			SR Router ID: 10.0.30.30

Node: 1      Proxy-Node: 0      Prefix: 0       Total Segments: 1

Flag Descriptions: R: Re-advertised, N: Node Segment, P: no-PHP
                   E: Explicit-NULL, V: Value, L: Local
Segment status codes: * - Self originated Prefix, L1 - level 1, L2 - level 2, ! - SR-unreachable,
                      # - Some IS-IS next-hops are SR-unreachable
   Prefix                      SID   Label Type       Flags                        System ID       Level Protection  Algorithm   
   ------------------------- ----- ------- ---------- ---------------------------- --------------- ----- ----------- -------------
*  10.0.30.30/32               330   20330 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-2-23 L2    unprotected SPF         

System ID: Arista-Spine3-Q2A-30			Instance: 'IGP'
SR supported Data-plane: MPLS			SR Router ID: 10.0.30.30

Node: 15     Proxy-Node: 0      Prefix: 2       Total Segments: 17

Flag Descriptions: R: Re-advertised, N: Node Segment, P: no-PHP
                   E: Explicit-NULL, V: Value, L: Local
Segment status codes: * - Self originated Prefix, L1 - level 1, L2 - level 2, ! - SR-unreachable,
                      # - Some IS-IS next-hops are SR-unreachable
   Prefix                      SID   Label Type       Flags                        System ID       Level Protection  Algorithm   
   ------------------------- ----- ------- ---------- ---------------------------- --------------- ----- ----------- -------------
*  10.0.0.30/32                 30   20030 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected SPF         
*  10.0.0.30/32                158   20158 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-LATENCY 
*  10.0.0.30/32                159   20159 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-TE      
*  10.0.0.30/32                160   20160 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected ADMIN       
   10.0.0.31/32                 31   20031 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE31-Q2C-31 L2    node with SRLG loose SPF         
   10.0.0.32/32                 32   20032 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node with SRLG loose SPF         
   10.0.0.72/32                 72   20072 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    node with SRLG loose SPF         
   10.0.0.84/32                 84   20084 Node       R:0 N:1 P:1 E:0 V:0 L:0      Ericsson_84_R6678 L2    node with SRLG loose SPF         
   10.0.0.120/32               120   20120 Prefix     R:1 N:0 P:1 E:0 V:0 L:0      0000.0000.0120  L2    node with SRLG loose SPF         
   10.0.0.122/32               122   20122 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0122  L2    node with SRLG loose SPF         
   10.0.0.175/32               175   20175 Node       R:1 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node with SRLG loose SPF         
   10.0.0.175/32               175   20175 Node       R:1 N:1 P:1 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node with SRLG loose SPF         
   10.0.0.214/32               214   20214 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node with SRLG loose SPF         
   209.209.209.202/32          202   20202 Prefix     R:0 N:0 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node with SRLG loose SPF         
   209.209.209.202/32          202   20202 Prefix     R:0 N:0 P:1 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node with SRLG loose SPF         
   209.209.209.202/32          202   20202 Prefix     R:0 N:0 P:1 E:0 V:0 L:0      0000.0000.0120  L2    node with SRLG loose SPF         
*  2002::30/128                430   20430 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected SPF         
*  2002::30/128                558   20558 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-LATENCY 
*  2002::30/128                559   20559 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-TE      
*  2002::30/128                560   20560 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected ADMIN       
```

## show ip ospf segment-routing

```text
```

## show ip ospf segment-routing global-blocks

```text
```

## show ip ospf segment-routing bindings

```text
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

 C        10.0.0.30/32
           directly connected, Loopback0
 I L2     10.0.0.31/32 [115/75]
           via 20.30.31.31, Ethernet1
 I L2     10.0.0.32/32 [115/50]
           via 20.30.32.32, Ethernet2
 I L2     10.0.0.66/32 [115/100]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.72/32 [115/110]
           via 20.30.72.72, Ethernet9
 I L2     10.0.0.84/32 [115/110]
           via 20.30.84.84, Ethernet12
 I L2     10.0.0.120/32 [115/100]
           via 20.30.120.120, Ethernet3
 I L2     10.0.0.122/32 [115/100]
           via 20.30.122.122, Ethernet14
 I L2     10.0.0.175/32 [115/100]
           via 20.30.120.120, Ethernet3
 I L2     10.0.0.214/32 [115/100]
           via 20.30.214.214, Ethernet5
 C        10.0.30.30/32
           directly connected, Loopback1000
 C        20.30.31.0/24
           directly connected, Ethernet1
 C        20.30.32.0/24
           directly connected, Ethernet2
 C        20.30.66.0/24
           directly connected, Ethernet31
 C        20.30.72.0/24
           directly connected, Ethernet9
 C        20.30.84.0/24
           directly connected, Ethernet12
 C        20.30.120.0/24
           directly connected, Ethernet3
 C        20.30.122.0/24
           directly connected, Ethernet14
 C        20.30.214.0/24
           directly connected, Ethernet5
 I L2     30.122.190.0/24 [115/100]
           via 20.30.122.122, Ethernet14
 I L2     101.64.122.0/24 [115/100]
           via 20.30.122.122, Ethernet14
 I L2     101.74.122.0/24 [115/100]
           via 20.30.122.122, Ethernet14
 I L2     101.88.122.0/24 [115/100]
           via 20.30.122.122, Ethernet14
 I L2     101.119.122.0/24 [115/100]
           via 20.30.122.122, Ethernet14
 I L2     101.122.125.0/24 [115/100]
           via 20.30.122.122, Ethernet14
 I L2     101.122.130.0/24 [115/100]
           via 20.30.122.122, Ethernet14
 I L2     101.122.158.0/24 [115/100]
           via 20.30.122.122, Ethernet14
 I L2     101.122.162.0/24 [115/100]
           via 20.30.122.122, Ethernet14
 I L2     101.122.169.0/24 [115/100]
           via 20.30.122.122, Ethernet14
 I L2     101.122.216.0/24 [115/100]
           via 20.30.122.122, Ethernet14
 I L2     101.122.218.0/24 [115/100]
           via 20.30.122.122, Ethernet14
 I L2     209.209.209.202/32 [115/60]
           via 20.30.32.32, Ethernet2


VRF: 2-23-5G-L3VPN
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

 C        10.0.30.30/32
           directly connected, Loopback7001


VRF: FLEXALGO
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

 C        10.128.0.30/32
           directly connected, Loopback5128


VRF: RED
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

 C        10.0.0.30/32
           directly connected, Loopback5001
 B I      10.0.0.31/32
           directly connected, Null0
 B I      50.10.31.0/24
           directly connected, Null0
 B E      50.10.53.0/24
           directly connected, Null0
 B I      50.10.72.0/24
           directly connected, Null0
 B I      50.10.84.0/24
           directly connected, Null0
 B I      50.10.122.0/24
           directly connected, Null0
 B E      50.10.128.0/24
           directly connected, Null0
 B E      50.10.179.0/24
           directly connected, Null0
 B E      50.10.184.0/24
           directly connected, Null0
 B E      50.10.216.0/24
           directly connected, Null0


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

## show ipv6 route

```text

VRF: default
Displaying 10 of 20 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 C        2001:0:30:31::/64 [0/0]
           via Ethernet1, directly connected
 C        2001:0:30:32::/64 [0/0]
           via Ethernet2, directly connected
 C        2001:0:30:66::/64 [0/0]
           via Ethernet31, directly connected
 C        2001:0:30:72::/64 [0/0]
           via Ethernet9, directly connected
 C        2001:0:30:84::/64 [0/0]
           via Ethernet12, directly connected
 C        2001:0:30:120::/64 [0/0]
           via Ethernet3, directly connected
 C        2001:0:30:214::/64 [0/0]
           via Ethernet5, directly connected
 C        2002::30/128 [0/0]
           via Loopback0, directly connected
 I L2     2002::31/128 [115/20]
           via fe80::6abf:6cff:fe35:1e31, Ethernet1
 I L2     2002::32/128 [115/20]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2

```

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 22 routes 
MPLS next-hop resolution allow default route: False
Metric Codes:
          A - Active metric
Via Type Codes:
          M - MPLS via, LP - LDP pseudowire via,
          I - IP lookup via, V - VLAN via,
          VA - EVPN VLAN aware via, ES - EVPN ethernet segment via,
          VF - EVPN VLAN flood via, AF - EVPN VLAN aware flood via,
          NG - Nexthop group via, BP - BGP pseudowire via,
          VP - VPWS pseudowire via, MSP - Static pseudowire via

 20031   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.31.31 Ethernet1
 20032   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.32.32 Ethernet2
 20072   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.72.72 Ethernet9
 20084   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.84.84 Ethernet12
 20120   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.120.120 Ethernet3
 20122   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.122.122 Ethernet14
 20175   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 2
                    via 20.30.120.120, Ethernet3, label imp-null(3)
                    backup via 20.30.32.32, Ethernet2, label imp-null(3)
 20202   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 3
                    via 20.30.32.32, Ethernet2, label 20202
                    backup via 20.30.120.120, Ethernet3, label imp-null(3)
 20214   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.214.214 Ethernet5
 362144   [0]
                via I, ipv4, vrf FLEXALGO
 362145   [0]
                via I, ipv4, vrf RED
 362146   [0]
                via I, ipv6, vrf RED
 378648  A[1]
                via M, 20.30.84.84, pop
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1018
 378649  A[1]
                via M, fe80::5a70:7fff:fe9f:c403, pop
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1018
 378650  A[1]
                via M, 20.30.32.32, pop
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1019
 378651  A[1]
                via M, fe80::d6af:f7ff:fe2f:1396, pop
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1019
 378652  A[1]
                via M, 20.30.120.120, pop
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1006
 378660  A[1]
                via M, 20.30.214.214, pop
                    EgressACL: apply
                    directly connected, Ethernet5
                    18:5b:00:61:ac:6f, vlan 1023
 378684  A[1]
                via M, 20.30.72.72, pop
                    EgressACL: apply
                    directly connected, Ethernet9
                    e0:9b:27:c4:c5:84, vlan 1017
 378688  A[1]
                via M, 20.30.31.31, pop
                    EgressACL: apply
                    directly connected, Ethernet1
                    68:bf:6c:35:1e:31, vlan 1011
 378689  A[1]
                via M, fe80::6abf:6cff:fe35:1e31, pop
                    EgressACL: apply
                    directly connected, Ethernet1
                    68:bf:6c:35:1e:31, vlan 1011
 378700  A[1]
                via M, 20.30.122.122, pop
                    EgressACL: apply
                    directly connected, Ethernet14
                    bc:31:e2:c1:50:b1, vlan 1015
```

## show mpls lfib route

```text
MPLS forwarding table (Label [metric] Vias) - 22 routes 
MPLS next-hop resolution allow default route: False
Via Type Codes:
          M - MPLS via, LP - LDP pseudowire via,
          I - IP lookup via, V - VLAN via,
          VA - EVPN VLAN aware via, ES - EVPN ethernet segment via,
          VF - EVPN VLAN flood via, AF - EVPN VLAN aware flood via,
          NG - Nexthop group via, BP - BGP pseudowire via,
          VP - VPWS pseudowire via, MSP - Static pseudowire via
Source Codes:
          G - gRIBI, S - Static MPLS route,
          B2 - BGP L2 EVPN, B3 - BGP L3 VPN,
          R - RSVP, P - Pseudowire,
          L - LDP, M - MLDP,
          I>BL - IS-IS SR to BGP LU, IP - IS-IS SR prefix segment,
          IA - IS-IS SR adjacency segment, I>L - IS-IS SR to LDP,
          L>I - LDP to IS-IS SR, OP - Ospf SR prefix segment,
          OA - Ospf SR adjacency segment, OL - Ospf SR segment to LDP,
          L0 - LDP to Ospf SR segment, BL - BGP LU,
          BL>L - BGP LU to LDP, L>BL - LDP to BGP LU,
          ST - SR TE policy, SMP - SR P2MP,
          BL>I - BGP LU to IS-IS SR, BLS - BGP Link State,
          DE - Debug LFIB

 IP    20031    [1], 10.0.0.31/32
                via M, 20.30.31.31, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    20032    [1], 10.0.0.32/32
                via M, 20.30.32.32, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet2
 IP    20072    [1], 10.0.0.72/32
                via M, 20.30.72.72, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet9
 IP    20084    [1], 10.0.0.84/32
                via M, 20.30.84.84, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet12
 IP    20120    [1], 10.0.0.120/32
                via M, 20.30.120.120, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet3
 IP    20122    [1], 10.0.0.122/32
                via M, 20.30.122.122, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet14
 IP    20175    [1], 10.0.0.175/32
                via TI-LFA tunnel index 2, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.120.120, Ethernet3, label imp-null(3)
                    backup via 20.30.32.32, Ethernet2, label imp-null(3)
 IP    20202    [1], 209.209.209.202/32
                via TI-LFA tunnel index 3, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.32, Ethernet2, label 20202
                    backup via 20.30.120.120, Ethernet3, label imp-null(3)
 IP    20214    [1], 10.0.0.214/32
                via M, 20.30.214.214, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 B3    362144   [0]
                via I, ipv4, vrf FLEXALGO
 B3    362145   [0]
                via I, ipv4, vrf RED
 B3    362146   [0]
                via I, ipv6, vrf RED
 IA    378648   [1]
                via M, 20.30.84.84, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet12
 IA    378649   [1]
                via M, fe80::5a70:7fff:fe9f:c403, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet12
 IA    378650   [1]
                via M, 20.30.32.32, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
 IA    378651   [1]
                via M, fe80::d6af:f7ff:fe2f:1396, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
 IA    378652   [1]
                via M, 20.30.120.120, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
 IA    378660   [1]
                via M, 20.30.214.214, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet5
 IA    378684   [1]
                via M, 20.30.72.72, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet9
 IA    378688   [1]
                via M, 20.30.31.31, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
 IA    378689   [1]
                via M, fe80::6abf:6cff:fe35:1e31, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
 IA    378700   [1]
                via M, 20.30.122.122, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet14
```

## show bgp evpn

```text
BGP routing table information for VRF default
Router identifier 10.0.0.30, local AS number 64512
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
```

## show bgp vpn-ipv4

```text
BGP routing table information for VRF default
Router identifier 10.0.0.30, local AS number 64512
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 10.0.0.31:5001 IPv4 prefix 10.0.0.31/32
                                 10.0.0.31             -       100     0       i
 * >      RD: 10.0.0.31:5001 IPv4 prefix 50.10.31.0/24
                                 10.0.0.31             -       100     0       i
 * >      RD: 53:5001 IPv4 prefix 50.10.53.0/24
                                 10.0.0.53             -       100     0       65000 ?
 * >      RD: 72:5001 IPv4 prefix 50.10.72.0/24
                                 10.0.0.72             -       100     0       ?
 * >      RD: 84:5001 IPv4 prefix 50.10.84.0/24
                                 10.0.0.84             0       100     0       ?
 * >      RD: 122:5001 IPv4 prefix 50.10.122.0/24
                                 10.0.0.122            0       100     0       ?
 * >      RD: 65000:128 IPv4 prefix 50.10.128.0/24
                                 10.0.0.128            -       100     0       65000 ?
 * >      RD: 179:5001 IPv4 prefix 50.10.179.0/24
                                 10.0.0.179            -       100     0       65000 i
 * >      RD: 184:5001 IPv4 prefix 50.10.184.0/24
                                 10.0.0.184            -       100     0       65000 i
 * >      RD: 216:5001 IPv4 prefix 50.10.216.0/24
                                 10.0.0.216            -       100     0       65000 i
 * >      RD: 216:7001 IPv4 prefix 50.10.216.0/24
                                 10.0.0.216            -       100     0       65000 i
```

## show bgp vpn-ipv6

```text
BGP routing table information for VRF default
Router identifier 10.0.0.30, local AS number 64512
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
```

## show bgp ipv4 labeled-unicast

```text
BGP routing table information for VRF default
Router identifier 10.0.0.30, local AS number 64512
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
```

## show bgp neighbors

```text
BGP neighbor is 10.0.0.31, remote AS 65001, internal link
 Description: Arista-PE31-Q2C
  BGP version 4, remote router ID 10.0.0.31, VRF default
  Inherits configuration from and member of peer-group OPTION-C-RIGHT-PEER
  Last read 00:00:45, last write 00:00:11
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:15
  Keepalive timer is active, time left: 00:00:37
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:39:07
  Number of transitions to established: 6
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Cease/connection rejected, Last time 16:35:51, First time 16:36:05, Repeats 3
  Last rcvd notification:Cease/administrative reset, Last time 00:39:08, First time 12:37:35, Repeats 1
  Last sent socket-error:Connect (Network is unreachable), Last time 17:26:32, First time 6d16h, Repeats 3027
  Types of communities advertised: standard extended large
  Enhanced route refresh stale path removal disabled
  Outbound enhanced route refresh enabled
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: received
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised and received and negotiated
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: advertised
    Additional-paths send capability:
      VPN-IPv4: received
      VPN-IPv6: received
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: yes
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 00:38:16
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 2
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                                  Sent      Rcvd
    Opens:                           6        10
    Notifications:                   7         2
    Updates:                        78        13
    Keepalives:                   1218      1236
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:               1309      1261
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         9         2              2                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 256000, warning limit is 204800
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 65001, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 37667
Remote TCP address is 10.0.0.31, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1448
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 7,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.2ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 508.07 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.32, remote AS 64512, internal link
 Description: Arista-PE32-Q2C
  BGP version 4, remote router ID 10.0.0.32, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 20:19:02, last write 20:18:34
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Idle, Peer is not activated in any address-family mode
  Peering failure hint: Peer is not activated in any address-family mode
  Number of transitions to established: 5
  Last state was Established
  Last event was ReapplyInboundPolicy
  Last sent notification:Cease/connection rejected, Last time 17:25:33, First time 20:18:32, Repeats 60
  Last sent socket-error:Connect (Network is unreachable), Last time 20:23:19, First time 2d19h, Repeats 606
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: received
    Multiprotocol VPN-IPv6: advertised and received
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
    Enhanced route refresh: advertised and received
    Send End-of-RIB messages: advertised and received
    Additional-paths recv capability:
      VPN-IPv6: advertised
    Additional-paths send capability:
      VPN-IPv4: received
      VPN-IPv6: received
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  5        66
    Notifications:         65         0
    Updates:              552        30
    Keepalives:          6558      6621
    Route Refresh:          0         0
    Total messages:      7180      6717
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Remote TCP address is 10.0.0.32

BGP neighbor is 10.0.0.53, remote AS 64512, internal link
 Description: Arrcus-53
  BGP version 4, remote router ID 10.0.0.53, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 2d19h, last write 2d19h
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Idle, Peer is not activated in any address-family mode
  Peering failure hint: Peer is not activated in any address-family mode
  Number of transitions to established: 5
  Last state was Active
  Last event was ReapplyInboundPolicy
  Last sent notification:Cease/connection rejected, Last time 18:03:17, First time 18:44:34, Repeats 114
  Last sent socket-error:Connect (Network is unreachable), Last time 2d19h, First time 2d20h, Repeats 30
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 with MPLS Labels: received
    Multiprotocol VPN-IPv4: advertised and received
    Multiprotocol VPN-IPv6: advertised and received
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: no
      IPv4 with MPLS Labels is enabled, Forwarding State is preserved
      VPN-IPv4 is enabled, Forwarding State is preserved
      VPN-IPv6 is enabled, Forwarding State is preserved
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  5       120
    Notifications:        120         0
    Updates:              596        18
    Keepalives:          6479      5541
    Route Refresh:          0         2
    Total messages:      7200      5681
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Remote TCP address is 10.0.0.53

BGP neighbor is 10.0.0.72, remote AS 65001, internal link
 Description: Ciena-5134-72
  BGP version 4, remote router ID 10.0.0.72, VRF default
  Inherits configuration from and member of peer-group OPTION-C-RIGHT-PEER
  Last read 00:00:39, last write 00:00:31
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:21
  Keepalive timer is active, time left: 00:00:26
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 15:51:39
  Number of transitions to established: 25
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Cease/connection rejected, Last time 16:35:51, First time 16:36:01, Repeats 2
  Last rcvd notification:Cease/peer de-configured, Last time 15:52:17, First time 16:39:40, Repeats 6
  Last sent socket-error:Connect (Connection refused), Last time 15:51:54, First time 17:48:00, Repeats 44
  Last rcvd socket-error:Connection reset by peer, Last time 15:59:03, First time 5d21h, Repeats 37
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Four Octet ASN: advertised
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 0
      Restart-State bit: no
      Graceful notification: no
      VPN-IPv4 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 15:51:28
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                 63        28
    Notifications:          8        19
    Updates:              630        67
    Keepalives:          7387      6310
    Route Refresh:          0         6
    Total messages:      8088      6430
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        10         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 256000, warning limit is 204800
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 65001, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 179
Remote TCP address is 10.0.0.72, remote port is 43777
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1460
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 7,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.6ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 183.94 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.84, remote AS 65001, internal link
 Description: Ericsson_84
  BGP version 4, remote router ID 10.0.0.84, VRF default
  Inherits configuration from and member of peer-group OPTION-C-RIGHT-PEER
  Last read 00:00:03, last write 00:00:12
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:27
  Keepalive timer is active, time left: 00:00:09
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 16:35:46
  Number of transitions to established: 4
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Cease/other configuration change, Last time 16:36:06
  Last sent socket-error:Connect (Network is unreachable), Last time 18:06:30, First time 2d20h, Repeats 59
  Last rcvd socket-error:Connection reset by peer, Last time 16:47:48
  Types of communities advertised: standard extended large
  Enhanced route refresh stale path removal disabled
  Outbound enhanced route refresh enabled
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised and received and negotiated
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: no
      VPN-IPv4 is enabled, Forwarding State is preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 16:35:46
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                                  Sent      Rcvd
    Opens:                           4         4
    Notifications:                   3         0
    Updates:                       426        10
    Keepalives:                   8823      7556
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:               9256      7570
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        10         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 256000, warning limit is 204800
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 65001, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 32927
Remote TCP address is 10.0.0.84, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1428
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,7
    Retransmission Timeout (rto): 432.0ms
    Round-trip Time (rtt/rtvar): 231.9ms/0.2ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 0.49 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.120, remote AS 64512, internal link
 Description: Huawei_120
  BGP version 4, remote router ID 10.0.0.120, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 2d19h, last write 2d19h
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Idle, Administratively shut down
  Peering failure hint: Administratively shut down
  Number of transitions to established: 9
  Last state was Active
  Last event was AdminShutdown
  Last sent notification:Hold Timer Expired Error/None, Last time 2d19h, First time 2d19h, Repeats 1
  Last rcvd notification:Cease/connection collision resolution, Last time 2d20h
  Last sent socket-error:Connect (Network is unreachable), Last time 22:36:33, First time 2d19h, Repeats 15
  Last rcvd socket-error:Connection reset by peer, Last time 2d19h, First time 2d19h, Repeats 1
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received
    Multiprotocol VPN-IPv6: advertised and received
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                 10        14
    Notifications:         10         1
    Updates:              637        92
    Keepalives:          5179      5177
    Route Refresh:          0         2
    Total messages:      5836      5286
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Remote TCP address is 10.0.0.120

BGP neighbor is 10.0.0.122, remote AS 65001, internal link
 Description: H3C_122
  BGP version 4, remote router ID 10.0.0.122, VRF default
  Inherits configuration from and member of peer-group OPTION-C-RIGHT-PEER
  Last read 00:00:25, last write 00:00:14
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:35
  Keepalive timer is active, time left: 00:00:31
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:25:38
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvKeepAlive
  Last sent socket-error:Connect (Connection refused), Last time 00:25:52, First time 01:46:01, Repeats 35
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised
    Additional-paths recv capability:
      VPN-IPv4: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: No
      Number of stale paths removed after graceful restart: 0
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  1         1
    Notifications:          0         0
    Updates:               21         2
    Keepalives:            26        29
    Route Refresh:          0         0
    Total messages:        48        32
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        10         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 256000, warning limit is 204800
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 65001, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 179
Remote TCP address is 10.0.0.122, remote port is 42460
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1384
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 3,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.6ms/0.3ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 174.64 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.124, remote AS 64512, internal link
 Description: Huawei_124
  BGP version 4, remote router ID 0.0.0.0, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read never, last write never
  Hold time is 0, keepalive interval is 0 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Idle, Administratively shut down
  Peering failure hint: Administratively shut down
  Number of transitions to established: 0
  Last state was Active
  Last event was AdminShutdown
  Last sent socket-error:Connect (Network is unreachable), Last time 20:21:07, First time 2d19h, Repeats 583
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  0         0
    Notifications:          0         0
    Updates:                0         0
    Keepalives:             0         0
    Route Refresh:          0         0
    Total messages:         0         0
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Remote TCP address is 10.0.0.124

BGP neighbor is 10.0.0.128, remote AS 64512, internal link
 Description: Huawei_128
  BGP version 4, remote router ID 10.0.0.128, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 5d22h, last write 5d22h
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Idle, Administratively shut down
  Peering failure hint: Administratively shut down
  Number of transitions to established: 1
  Last state was Active
  Last event was AdminShutdown
  Last sent notification:Open Message Error/unsupported capability, Last time 5d22h, First time 5d23h, Repeats 38
    Sent data: 0x010400010080010400020080
  Last rcvd notification:Cease/peer de-configured, Last time 5d23h
  Last sent socket-error:Connect (Network is unreachable), Last time 20:56:08, First time 2d19h, Repeats 10
  Last rcvd socket-error:Connection reset by peer, Last time 5d23h, First time 5d23h, Repeats 5
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised
    Multiprotocol VPN-IPv6: advertised
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                 46        40
    Notifications:         39         1
    Updates:               25         2
    Keepalives:             2         1
    Route Refresh:          0         0
    Total messages:       112        44
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Remote TCP address is 10.0.0.128

BGP neighbor is 10.0.0.131, remote AS 64512, internal link
 Description: Juniper-131-JCNR
  BGP version 4, remote router ID 10.0.0.131, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 20:18:38, last write 20:18:33
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Idle, Administratively shut down
  Peering failure hint: Administratively shut down
  Number of transitions to established: 5
  Last state was Established
  Last event was AdminShutdown
  Last sent notification:Cease/connection rejected, Last time 17:51:13, First time 20:18:31, Repeats 71
  Last rcvd notification:Cease/connection rejected, Last time 2d20h
  Last sent socket-error:Connect (Network is unreachable), Last time 20:23:25, First time 2d19h, Repeats 604
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: received
    Multiprotocol VPN-IPv6: advertised and received
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received
    Additional-paths recv capability:
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
    Long Lived Graceful Restart received:
      Helper only
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  7        79
    Notifications:         77         1
    Updates:              588        18
    Keepalives:         13194     12459
    Route Refresh:          0         0
    Total messages:     13866     12557
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Remote TCP address is 10.0.0.131

BGP neighbor is 10.0.0.156, remote AS 64512, internal link
 Description: Juniper-156
  BGP version 4, remote router ID 10.0.0.156, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 20:18:35, last write 20:18:34
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Idle, Administratively shut down
  Peering failure hint: Administratively shut down
  Number of transitions to established: 6
  Last state was Established
  Last event was AdminShutdown
  Last sent notification:Cease/connection rejected, Last time 20:11:49, First time 20:18:32, Repeats 17
  Last rcvd notification:Cease/connection rejected, Last time 2d20h
  Last sent socket-error:Connect (Network is unreachable), Last time 20:24:48, First time 2d19h, Repeats 648
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: received
    Multiprotocol VPN-IPv6: advertised and received
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received
    Additional-paths recv capability:
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
    Long Lived Graceful Restart received:
      Helper only
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  7        25
    Notifications:         22         2
    Updates:              474       134
    Keepalives:         13158     12397
    Route Refresh:          0         0
    Total messages:     13661     12558
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Remote TCP address is 10.0.0.156

BGP neighbor is 10.0.0.175, remote AS 65000, external link
 Description: Juniper-175
  BGP version 4, remote router ID 10.0.0.175, VRF default
  Inherits configuration from and member of peer-group OPTION-C-LEFT-PEER
  Last read 00:00:23, last write 00:00:21
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:07
  Keepalive timer is active, time left: 00:00:05
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 16:35:46
  Number of transitions to established: 4
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Cease/connection rejected, Last time 16:35:50, First time 16:36:04, Repeats 4
  Last rcvd notification:Open Message Error/bad AS number, Last time 19:29:04, First time 19:30:42, Repeats 9
  Types of communities advertised: standard extended large
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
    Long Lived Graceful Restart received:
      Helper only
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 16:35:46
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are disabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are disabled
  AIGP attribute send and receive for IPv6 Unicast are disabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are disabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                 33        38
    Notifications:         27        10
    Updates:               56        63
    Keepalives:          2739      2551
    Route Refresh:          0         0
    Total messages:      2855      2662
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         5         6              6                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 256000, warning limit is 204800
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 65001, local router ID 10.0.0.30
TTL is 3, external peer can be 3 hops away
Local TCP address is 10.0.0.30, local port is 46439
Remote TCP address is 10.0.0.175, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1448
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.5ms/0.1ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 228.48 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.179, remote AS 64512, internal link
 Description: Juniper-179
  BGP version 4, remote router ID 10.0.0.179, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 20:18:34, last write 20:18:34
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Idle, Administratively shut down
  Peering failure hint: Administratively shut down
  Number of transitions to established: 6
  Last state was Established
  Last event was AdminShutdown
  Last sent notification:Cease/connection rejected, Last time 18:35:37, First time 20:18:32, Repeats 53
  Last rcvd notification:Cease/connection rejected, Last time 2d20h
  Last sent socket-error:Connect (Network is unreachable), Last time 20:24:51, First time 2d19h, Repeats 602
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: received
    Multiprotocol VPN-IPv6: advertised and received
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received
    Additional-paths recv capability:
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
    Long Lived Graceful Restart received:
      Helper only
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                341       395
    Notifications:        393         1
    Updates:              567        32
    Keepalives:         10911     10315
    Route Refresh:          0         2
    Total messages:     12212     10745
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Remote TCP address is 10.0.0.179

BGP neighbor is 10.0.0.184, remote AS 64512, internal link
 Description: IXIA
  BGP version 4, remote router ID 0.0.0.0, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read never, last write never
  Hold time is 0, keepalive interval is 0 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Idle, Administratively shut down
  Peering failure hint: Administratively shut down
  Number of transitions to established: 0
  Last state was Active
  Last event was AdminShutdown
  Last sent socket-error:Connect (Network is unreachable), Last time 20:19:47, First time 6d16h, Repeats 2987
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  0         0
    Notifications:          0         0
    Updates:                0         0
    Keepalives:             0         0
    Route Refresh:          0         0
    Total messages:         0         0
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Remote TCP address is 10.0.0.184

BGP neighbor is 10.0.0.214, remote AS 64512, internal link
 Description: Nokia-SXR-214
  BGP version 4, remote router ID 10.0.0.214, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 2d23h, last write 2d19h
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Idle, Administratively shut down
  Peering failure hint: Administratively shut down
  Number of transitions to established: 1
  Last state was Active
  Last event was AdminShutdown
  Last rcvd notification:Cease/administrative shutdown, Last time 2d23h
  Last sent socket-error:Connect (Network is unreachable), Last time 1d16h, First time 2d01h, Repeats 5
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received
    Multiprotocol VPN-IPv6: advertised and received
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 300
      Restart-State bit: no
      Graceful notification: no
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                106         1
    Notifications:          0         1
    Updates:              301         5
    Keepalives:         12497     10669
    Route Refresh:          0         1
    Total messages:     12904     10677
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Remote TCP address is 10.0.0.214

BGP neighbor is 10.0.0.216, remote AS 64512, internal link
 Description: 2-23-5G-NOKIA-216
  BGP version 4, remote router ID 10.0.0.216, VRF default
  Inherits configuration from and member of peer-group 2-23-5G-RR
  Last read 18:45:59, last write 18:45:45
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Idle, Administratively shut down
  Peering failure hint: Administratively shut down
  Number of transitions to established: 1
  Last state was Established
  Last event was AdminShutdown
  Last sent notification:Cease/connection rejected, Last time 18:30:50, First time 18:45:45, Repeats 25
  Types of communities advertised: standard extended large
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received
    Multiprotocol L2VPN EVPN: advertised and received
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received
    Additional-paths recv capability:
      VPN-IPv4: advertised
      L2VPN EVPN: advertised
    Additional-paths send capability:
      VPN-IPv4: received
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      L2VPN EVPN is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: no
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  1        27
    Notifications:         27         0
    Updates:               14       182
    Keepalives:            21        18
    Route Refresh:          0         0
    Total messages:        63       227
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 256000, warning limit is 204800
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 129
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 4
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 4
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
    Last treat-as-withdraw attribute error: Nexthop is local address
    Last update with error received at: 18:54:04
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Remote TCP address is 10.0.0.216

BGP neighbor is 10.0.0.217, remote AS 64512, internal link
 Description: Nokia
  BGP version 4, remote router ID 10.0.0.217, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 2d19h, last write 2d19h
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Idle, Administratively shut down
  Peering failure hint: Administratively shut down
  Number of transitions to established: 2
  Last state was Connect
  Last event was AdminShutdown
  Last sent notification:Hold Timer Expired Error/None, Last time 2d19h
  Last sent socket-error:Connect (Network is unreachable), Last time 20:22:07, First time 2d19h, Repeats 532
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received
    Multiprotocol VPN-IPv6: advertised and received
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: no
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  2         2
    Notifications:          1         0
    Updates:              514        17
    Keepalives:         13144     11245
    Route Refresh:          0         2
    Total messages:     13661     11266
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Remote TCP address is 10.0.0.217

BGP neighbor is 10.0.0.221, remote AS 64512, internal link
 Description: Ribbon-221
  BGP version 4, remote router ID 10.0.0.221, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 20:19:11, last write 20:19:11
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Idle, Administratively shut down
  Peering failure hint: Administratively shut down
  Number of transitions to established: 16
  Last state was Active
  Last event was AdminShutdown
  Last sent notification:Hold Timer Expired Error/None, Last time 2d00h, First time 6d00h, Repeats 6
  Last rcvd notification:Cease/connection rejected, Last time 20:19:11, First time 20:20:22, Repeats 1
  Last sent socket-error:Connect (Connection refused), Last time 20:21:31, First time 20:23:12, Repeats 6
  Last rcvd socket-error:Connection reset by peer, Last time 2d19h, First time 6d16h, Repeats 8
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received
    Multiprotocol VPN-IPv6: advertised and received
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
    Enhanced route refresh: advertised and received
    Send End-of-RIB messages: advertised
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                 19        16
    Notifications:          7         2
    Updates:              956        51
    Keepalives:          6501     15241
    Route Refresh:         20        10
    Total messages:      7503     15320
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Remote TCP address is 10.0.0.221

BGP neighbor is 10.0.1.156, remote AS 64512, internal link
 Description: 2-23-5G-JUNIPER-156
  BGP version 4, remote router ID 10.0.0.156, VRF default
  Inherits configuration from and member of peer-group 2-23-5G-RR
  Last read 20:11:42, last write 20:11:28
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Idle, Administratively shut down
  Peering failure hint: Administratively shut down
  Number of transitions to established: 3
  Last state was Established
  Last event was AdminShutdown
  Last sent notification:Cease/administrative shutdown, Last time 20:11:28
  Last rcvd notification:Cease/peer de-configured, Last time 2d17h
  Types of communities advertised: standard extended large
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received
    Multiprotocol L2VPN EVPN: advertised and received
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received
    Additional-paths recv capability:
      VPN-IPv4: advertised
      L2VPN EVPN: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      L2VPN EVPN is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
    Long Lived Graceful Restart received:
      Helper only
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  3         3
    Notifications:          2         1
    Updates:               68       474
    Keepalives:          6579      6021
    Route Refresh:          0         0
    Total messages:      6652      6499
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 256000, warning limit is 204800
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 5
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Remote TCP address is 10.0.1.156

```

## show bgp labeled-unicast tunnel

```text
Index Endpoint Nexthop/Tunnel Index Interface Labels Contributing  Metric/Type 
----- -------- -------------------- --------- ------ ------------- ------------

   Metric 2       Pref    Pref 2
-------------- ---------- ------

```

## show bgp labeled-unicast forwarding

```text
   Index       Nexthop       Interface    Labels
----------- ------------- --------------- ------

```

## show tunnel rib system-tunnel-rib brief

```text
Tunnel RIB: system-tunnel-rib
Endpoint           Tunnel Type    Index(es)  Tunnel Preference  IGP Preference 
------------------ -------------- ---------- ------------------ ---------------
10.0.0.31/32       IS-IS SR IPv4  34         65                 115            
10.0.0.32/32       IS-IS SR IPv4  20         65                 115            
10.0.0.72/32       IS-IS SR IPv4  14         65                 115            
10.0.0.84/32       IS-IS SR IPv4  8          65                 115            
10.0.0.120/32      IS-IS SR IPv4  17         65                 115            
10.0.0.122/32      IS-IS SR IPv4  35         65                 115            
10.0.0.175/32      IS-IS SR IPv4  7          65                 115            
10.0.0.214/32      IS-IS SR IPv4  21         65                 115            
209.209.209.202/32 IS-IS SR IPv4  33         65                 115            

   IGP Metric    Metric Type
---------------- -----------
   75            metric     
   50            metric     
   110           metric     
   110           metric     
   100           metric     
   100           metric     
   100           metric     
   100           metric     
   60            metric     

```

## show tunnel rib colored brief

```text
Tunnel RIB: system-colored-tunnel-rib
 Endpoint     Color     Tunnel Type     Index(es)     Tunnel Preference     IGP Preference     IGP Metric   Metric Type
----------- --------- --------------- ------------- --------------------- ------------------ -------------- -----------

```

## show rib route ip

```text
VRF: default, Protocol: connected
Codes: C - Connected, S - Static, P - Route Input, G - Gribi
       B - BGP, O - Ospf, O3 - Ospf3, I - Isis, R - Rip, VL - VRF Leak
       > - Best Route, * - Unresolved Next hop
       EM - Exact match of the SR-TE Policy
       NM - Null endpoint match of the SR-TE Policy
       AM - Any endpoint match of the SR-TE Policy
       L - Part of a recursive route resolution loop
       A - Next hop not resolved in ARP/ND
       NF - Not in FEC
>C    10.0.0.30/32 [0 pref/0 metric] updated 2d20h ago
         via Loopback0, directly connected
>C    10.0.30.30/32 [0 pref/0 metric] updated 2d20h ago
         via Loopback1000, directly connected
>C    20.30.31.0/24 [0 pref/0 metric] updated 18:02:15 ago
         via Ethernet1, directly connected
>C    20.30.32.0/24 [0 pref/0 metric] updated 18:04:52 ago
         via Ethernet2, directly connected
>C    20.30.66.0/24 [0 pref/0 metric] updated 5d16h ago
         via Ethernet31, directly connected
>C    20.30.72.0/24 [0 pref/0 metric] updated 18:06:23 ago
         via Ethernet9, directly connected
>C    20.30.84.0/24 [0 pref/0 metric] updated 18:05:54 ago
         via Ethernet12, directly connected
>C    20.30.120.0/24 [0 pref/0 metric] updated 17:17:51 ago
         via Ethernet3, directly connected
>C    20.30.122.0/24 [0 pref/0 metric] updated 16:48:09 ago
         via Ethernet14, directly connected
>C    20.30.214.0/24 [0 pref/0 metric] updated 18:03:42 ago
         via Ethernet5, directly connected
VRF: default, Protocol: route-input
Codes: C - Connected, S - Static, P - Route Input, G - Gribi
       B - BGP, O - Ospf, O3 - Ospf3, I - Isis, R - Rip, VL - VRF Leak
       > - Best Route, * - Unresolved Next hop
       EM - Exact match of the SR-TE Policy
       NM - Null endpoint match of the SR-TE Policy
       AM - Any endpoint match of the SR-TE Policy
       L - Part of a recursive route resolution loop
       A - Next hop not resolved in ARP/ND
       NF - Not in FEC
>P    0.0.0.0/8 [1 pref/0 metric] updated 6d19h ago
         via Null0, directly connected [NF]
>P    127.0.0.0/8 [1 pref/0 metric] updated 6d19h ago
         via :: [1 pref/1 metric] type ipv4
            via , directly connected
VRF: default, Protocol: isis
Codes: C - Connected, S - Static, P - Route Input, G - Gribi
       B - BGP, O - Ospf, O3 - Ospf3, I - Isis, R - Rip, VL - VRF Leak
       > - Best Route, * - Unresolved Next hop
       EM - Exact match of the SR-TE Policy
       NM - Null endpoint match of the SR-TE Policy
       AM - Any endpoint match of the SR-TE Policy
       L - Part of a recursive route resolution loop
       A - Next hop not resolved in ARP/ND
       NF - Not in FEC
>I    10.0.0.31/32 [115 pref/75 metric] updated 00:29:46 ago
         via 20.30.31.31, Ethernet1
>I    10.0.0.32/32 [115 pref/50 metric] updated 00:59:05 ago
         via 20.30.32.32, Ethernet2
>I    10.0.0.66/32 [115 pref/100 metric] updated 01:12:23 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.72/32 [115 pref/110 metric] updated 01:12:23 ago
         via 20.30.72.72, Ethernet9
>I    10.0.0.84/32 [115 pref/110 metric] updated 01:12:23 ago
         via 20.30.84.84, Ethernet12
>I    10.0.0.120/32 [115 pref/100 metric] updated 01:12:23 ago
         via 20.30.120.120, Ethernet3
>I    10.0.0.122/32 [115 pref/100 metric] updated 01:12:23 ago
         via 20.30.122.122, Ethernet14
>I    10.0.0.175/32 [115 pref/100 metric] updated 00:01:51 ago
         via 20.30.120.120, Ethernet3
>I    10.0.0.214/32 [115 pref/100 metric] updated 01:12:23 ago
         via 20.30.214.214, Ethernet5
>I    30.122.190.0/24 [115 pref/100 metric] updated 01:12:23 ago
         via 20.30.122.122, Ethernet14
>I    101.64.122.0/24 [115 pref/100 metric] updated 01:12:23 ago
         via 20.30.122.122, Ethernet14
>I    101.74.122.0/24 [115 pref/100 metric] updated 01:12:23 ago
         via 20.30.122.122, Ethernet14
>I    101.88.122.0/24 [115 pref/100 metric] updated 01:12:23 ago
         via 20.30.122.122, Ethernet14
>I    101.119.122.0/24 [115 pref/100 metric] updated 01:12:23 ago
         via 20.30.122.122, Ethernet14
>I    101.122.125.0/24 [115 pref/100 metric] updated 01:12:23 ago
         via 20.30.122.122, Ethernet14
>I    101.122.130.0/24 [115 pref/100 metric] updated 01:12:23 ago
         via 20.30.122.122, Ethernet14
>I    101.122.158.0/24 [115 pref/100 metric] updated 01:12:23 ago
         via 20.30.122.122, Ethernet14
>I    101.122.162.0/24 [115 pref/100 metric] updated 01:12:23 ago
         via 20.30.122.122, Ethernet14
>I    101.122.169.0/24 [115 pref/100 metric] updated 01:12:23 ago
         via 20.30.122.122, Ethernet14
>I    101.122.216.0/24 [115 pref/100 metric] updated 01:12:23 ago
         via 20.30.122.122, Ethernet14
>I    101.122.218.0/24 [115 pref/100 metric] updated 01:12:23 ago
         via 20.30.122.122, Ethernet14
>I    209.209.209.202/32 [115 pref/60 metric] updated 00:01:51 ago
         via 20.30.32.32, Ethernet2
```

## show rib route ipv6

```text
VRF: default, Protocol: connected
Codes: C - Connected, S - Static, P - Route Input, G - Gribi
       B - BGP, O - Ospf, O3 - Ospf3, I - Isis, R - Rip, VL - VRF Leak
       > - Best Route, * - Unresolved Next hop
       EM - Exact match of the SR-TE Policy
       NM - Null endpoint match of the SR-TE Policy
       AM - Any endpoint match of the SR-TE Policy
       L - Part of a recursive route resolution loop
       A - Next hop not resolved in ARP/ND
       NF - Not in FEC
>C    2001:0:30:31::/64 [0 pref/0 metric] updated 18:02:15 ago
         via Ethernet1, directly connected
>C    2001:0:30:32::/64 [0 pref/0 metric] updated 18:04:52 ago
         via Ethernet2, directly connected
>C    2001:0:30:66::/64 [0 pref/0 metric] updated 5d16h ago
         via Ethernet31, directly connected
>C    2001:0:30:72::/64 [0 pref/0 metric] updated 18:06:23 ago
         via Ethernet9, directly connected
>C    2001:0:30:84::/64 [0 pref/0 metric] updated 18:05:54 ago
         via Ethernet12, directly connected
>C    2001:0:30:120::/64 [0 pref/0 metric] updated 17:17:51 ago
         via Ethernet3, directly connected
>C    2001:0:30:214::/64 [0 pref/0 metric] updated 18:03:42 ago
         via Ethernet5, directly connected
>C    2002::30/128 [0 pref/0 metric] updated 2d20h ago
         via Loopback0, directly connected
VRF: default, Protocol: route-input
Codes: C - Connected, S - Static, P - Route Input, G - Gribi
       B - BGP, O - Ospf, O3 - Ospf3, I - Isis, R - Rip, VL - VRF Leak
       > - Best Route, * - Unresolved Next hop
       EM - Exact match of the SR-TE Policy
       NM - Null endpoint match of the SR-TE Policy
       AM - Any endpoint match of the SR-TE Policy
       L - Part of a recursive route resolution loop
       A - Next hop not resolved in ARP/ND
       NF - Not in FEC
>P    ::/96 [1 pref/0 metric] updated 6d19h ago
         via Null0, directly connected [NF]
>P    ::ffff:127.0.0.0/104 [1 pref/0 metric] updated 6d19h ago
         via :: [1 pref/1 metric] type ipv6
            via , directly connected
>P    fe80::/10 [1 pref/0 metric] updated 6d19h ago
VRF: default, Protocol: isis
Codes: C - Connected, S - Static, P - Route Input, G - Gribi
       B - BGP, O - Ospf, O3 - Ospf3, I - Isis, R - Rip, VL - VRF Leak
       > - Best Route, * - Unresolved Next hop
       EM - Exact match of the SR-TE Policy
       NM - Null endpoint match of the SR-TE Policy
       AM - Any endpoint match of the SR-TE Policy
       L - Part of a recursive route resolution loop
       A - Next hop not resolved in ARP/ND
       NF - Not in FEC
>I    2002::31/128 [115 pref/20 metric] updated 17:24:40 ago
         via fe80::6abf:6cff:fe35:1e31, Ethernet1
>I    2002::32/128 [115 pref/20 metric] updated 17:44:04 ago
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
```

## show platform sand l3 summary

```text
Number of vrfs: 5

Ipv4:
  Routes:       96   backlog:  0  unprogrammed:  0
  Adjacencies:  104  backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       26   backlog:  0  unprogrammed:  0
  Adjacencies:  104  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       19  backlog:  0  unprogrammed:  0
  Adjacencies:  10  backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4136  ecmp fecs:  0  fec entries:  4136
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  10  ecmp fecs:  0  fec entries:  10
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   96  unprogrammed:   0   
  Routes6:  26  unprogrammed6:  0   
  Backlog:  0 

Jericho2 Lpm:
  TCAM entries used:   4   Percent free:  99  ADS2 entries used:   9  Percent free:  99
  Pivot buckets used:  6   Rows used:     2   Entries Per Bucket:  1  Percent free:  99
  Route buckets used:  23  Rows used:     5   Entries Per Bucket:  5  Percent free:  99

Lem:
  IPv4  Host in Lem:            disabled
  IPv4  Prefix-lengths in Lem:  None    
  IPv6  Host in Lem:            disabled
  IPv6  Prefix-lengths in Lem:  None    
  Number of downloads:        0
  Number of overflow events:  0

Egress Arp rewrite entries in use (in each fap):
  FixedSystem: 8
Egress Arp remote rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Ip tunnel rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Mpls (for outer 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Mpls (for inner 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 1
Egress Sflow rewrite entries in use (in each fap):
  FixedSystem: 0

Egress rewrite chains in backlog: resource-full 0, no-interface 0

Glem entries used per fap :
  FixedSystem: 4105

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  795  allocs:  7780  frees:  7733  shuffles:  0  cmds:  0
  Zombies:     0    purges:    0
  Quarantine:  0/0  shuffles:  0  deletes:  0   
  Preserved FECs: 0
    First FEC preserved: never
    Last FEC preserved: never
  Fec insertion failures:  0
  Level1  Fecs:
    Non-ecmp fecs:            0    ecmp fecs:            1 
    Non-ecmp (Percent free):  100  ecmp (Percent free):  99
  Level2  Fecs:
    Non-ecmp fecs:            0    ecmp fecs:            0  
    Non-ecmp (Percent free):  100  ecmp (Percent free):  100
  Level3  Fecs:
    Non-ecmp fecs:            94  ecmp fecs:            0  
    Non-ecmp (Percent free):  99  ecmp (Percent free):  100

Lpm Detail:
  Requests:  37090  cleanses:  3750  batches:  3750  avg batch size:  9

Jericho Arp:
  ArpTable writes:      157034  queued      0   
  IngressTable writes:  243720  queued      0   
  Coprocessors:         1       in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  1    
  Number of uncountable MPLS tunnels:      1    
  Number of MPLSoGRE tunnels:              0    
  Number of uncountable MPLSoGRE tunnels:  0    
  Number of IP tunnels:                    0    
  Number of uncountable IP tunnels:        0    
  Shuffle tunnel enabled:                  False
```

## show platform jericho2 ip route

```text
Tunnel Type: M(mpls), G(gre), MoG(mpls-over-gre), MoU(mpls-over-udp), I(ip-in-ip), IPoU(ip-over-udp)
             vxlan-o(vxlan outer-rewrite info), vxlan-i(vxlan inner-rewrite info)
CW  - Control word
FL  - Flow label
EL  - Entropy label
ELI - Entropy label indicator
*   - Routes in LEM
D   - ECMP is divergent across switching chips
 ----------------------------------------------------------------------------------------------------------
|                                 Routing Table                                            |              |
|----------------------------------------------------------------------------------------------------------
|VRF|   Destination    |     |                    |     |        |                   | ECMP|  FEC | Tunnel
| ID|      Subnet      | Cmd |     Destination    | VID | Outlif |   MAC / CPU Code  |Index| Index|T Value
 ----------------------------------------------------------------------------------------------------------
|0  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318922|   -   
|0  |10.0.0.30/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |10.0.0.31/32      |ROUTE| Et1                |1011 |103434  | 68:bf:6c:35:1e:31 |  -  |318792|   -   
|0  |10.0.0.32/32      |ROUTE| Et2                |1019 |103425  | d4:af:f7:2f:13:96 |  -  |318768|   -   
|0  |10.0.0.66/32      |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318932|   -   
|0  |10.0.0.72/32      |ROUTE| Et9                |1017 |103422  | e0:9b:27:c4:c5:84 |  -  |318988|   -   
|0  |10.0.0.84/32      |ROUTE| Et12               |1018 |103423  | 58:70:7f:9f:c4:03 |  -  |318974|   -   
|0  |10.0.0.120/32     |ROUTE| Et3                |1006 |103426  | bc:31:e2:e1:ec:2c |  -  |318790|   -   
|0  |10.0.0.122/32     |ROUTE| Et14               |1015 |103428  | bc:31:e2:c1:50:b1 |  -  |318930|   -   
|0  |10.0.0.175/32     |ROUTE| Et3                |1006 |103426  | bc:31:e2:e1:ec:2c |  -  |318790|   -   
|0  |10.0.0.214/32     |ROUTE| Et5                |1023 |103427  | 18:5b:00:61:ac:6f |  -  |318962|   -   
|0  |10.0.30.30/32     |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.31.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.31.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.31.31/32    |ROUTE| Et1                |1011 |103434  | 68:bf:6c:35:1e:31 |  -  |318796|   -   
|0  |20.30.31.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.31.0/24     |TRAP | CoppSystemL3DstMiss|1011 |1011    | ArpTrap           |  -  |315682|   -   
|0  |20.30.32.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.32.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.32.32/32    |ROUTE| Et2                |1019 |103425  | d4:af:f7:2f:13:96 |  -  |318784|   -   
|0  |20.30.32.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.32.0/24     |TRAP | CoppSystemL3DstMiss|1019 |1019    | ArpTrap           |  -  |315690|   -   
|0  |20.30.66.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.66.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.66.66/32    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318992|   -   
|0  |20.30.66.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.66.0/24     |TRAP | CoppSystemL3DstMiss|1020 |1020    | ArpTrap           |  -  |315691|   -   
|0  |20.30.72.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.72.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.72.72/32    |ROUTE| Et9                |1017 |103422  | e0:9b:27:c4:c5:84 |  -  |318982|   -   
|0  |20.30.72.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.72.0/24     |TRAP | CoppSystemL3DstMiss|1017 |1017    | ArpTrap           |  -  |315688|   -   
|0  |20.30.84.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.84.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.84.84/32    |ROUTE| Et12               |1018 |103423  | 58:70:7f:9f:c4:03 |  -  |318972|   -   
|0  |20.30.84.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.84.0/24     |TRAP | CoppSystemL3DstMiss|1018 |1018    | ArpTrap           |  -  |315689|   -   
|0  |20.30.120.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.120.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.120.120/32  |ROUTE| Et3                |1006 |103426  | bc:31:e2:e1:ec:2c |  -  |318944|   -   
|0  |20.30.120.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.120.0/24    |TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |  -  |315677|   -   
|0  |20.30.122.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.122.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.122.122/32  |ROUTE| Et14               |1015 |103428  | bc:31:e2:c1:50:b1 |  -  |318986|   -   
|0  |20.30.122.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.122.0/24    |TRAP | CoppSystemL3DstMiss|1015 |1015    | ArpTrap           |  -  |315686|   -   
|0  |20.30.214.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.214.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.214.214/32  |ROUTE| Et5                |1023 |103427  | 18:5b:00:61:ac:6f |  -  |318940|   -   
|0  |20.30.214.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.214.0/24    |TRAP | CoppSystemL3DstMiss|1023 |1023    | ArpTrap           |  -  |315694|   -   
|0  |30.122.190.0/24   |ROUTE| Et14               |1015 |103428  | bc:31:e2:c1:50:b1 |  -  |318930|   -   
|0  |101.64.122.0/24   |ROUTE| Et14               |1015 |103428  | bc:31:e2:c1:50:b1 |  -  |318930|   -   
|0  |101.74.122.0/24   |ROUTE| Et14               |1015 |103428  | bc:31:e2:c1:50:b1 |  -  |318930|   -   
|0  |101.88.122.0/24   |ROUTE| Et14               |1015 |103428  | bc:31:e2:c1:50:b1 |  -  |318930|   -   
|0  |101.119.122.0/24  |ROUTE| Et14               |1015 |103428  | bc:31:e2:c1:50:b1 |  -  |318930|   -   
|0  |101.122.125.0/24  |ROUTE| Et14               |1015 |103428  | bc:31:e2:c1:50:b1 |  -  |318930|   -   
|0  |101.122.130.0/24  |ROUTE| Et14               |1015 |103428  | bc:31:e2:c1:50:b1 |  -  |318930|   -   
|0  |101.122.158.0/24  |ROUTE| Et14               |1015 |103428  | bc:31:e2:c1:50:b1 |  -  |318930|   -   
|0  |101.122.162.0/24  |ROUTE| Et14               |1015 |103428  | bc:31:e2:c1:50:b1 |  -  |318930|   -   
|0  |101.122.169.0/24  |ROUTE| Et14               |1015 |103428  | bc:31:e2:c1:50:b1 |  -  |318930|   -   
|0  |101.122.216.0/24  |ROUTE| Et14               |1015 |103428  | bc:31:e2:c1:50:b1 |  -  |318930|   -   
|0  |101.122.218.0/24  |ROUTE| Et14               |1015 |103428  | bc:31:e2:c1:50:b1 |  -  |318930|   -   
|0  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|0  |209.209.209.202/32|ROUTE| Et2                |1019 |103425  | d4:af:f7:2f:13:96 |  -  |318768|   -   
|0  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|1  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318968|   -   
|1  |10.0.0.30/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|1  |10.0.0.31/32      |DROP | DROP               |0    |  -     |                   |  -  |318950|   -   
|1  |50.10.31.0/24     |DROP | DROP               |0    |  -     |                   |  -  |318950|   -   
|1  |50.10.53.0/24     |DROP | DROP               |0    |  -     |                   |  -  |318938|   -   
|1  |50.10.72.0/24     |DROP | DROP               |0    |  -     |                   |  -  |318936|   -   
|1  |50.10.84.0/24     |DROP | DROP               |0    |  -     |                   |  -  |318776|   -   
|1  |50.10.122.0/24    |DROP | DROP               |0    |  -     |                   |  -  |318782|   -   
|1  |50.10.128.0/24    |DROP | DROP               |0    |  -     |                   |  -  |318798|   -   
|1  |50.10.179.0/24    |DROP | DROP               |0    |  -     |                   |  -  |318778|   -   
|1  |50.10.184.0/24    |DROP | DROP               |0    |  -     |                   |  -  |318934|   -   
|1  |50.10.216.0/24    |DROP | DROP               |0    |  -     |                   |  -  |318946|   -   
|1  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|1  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|2  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318970|   -   
|2  |10.128.0.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|2  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|2  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|3  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318966|   -   
|3  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|3  |192.168.20.0/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|3  |192.168.20.30/32  |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|3  |192.168.21.255/32 |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|3  |192.168.20.0/23   |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|3  |0.0.0.0/0         |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|4  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318960|   -   
|4  |10.0.30.30/32     |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|4  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|4  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   

```

## show platform jericho2 fec all

```text
Tunnel Type: Mpop(mpls pop), Mpush(mpls push), Mswap(mpls swap),
             MoG(mpls-over-gre), T(IPv4 tunnels GRE/GUE/VXLAN),
             N(Ipsec tunnel NAT-T [IP,SPORT,DPORT])
CW  - Control word
FL  - Flow label
EL  - Entropy label
ELI - Entropy label indicator
D   - ECMP is divergent across switching chips
 -----------------------------------------------------------------------------------------------
|                                              FEC Entry                                        |
 -----------------------------------------------------------------------------------------------
|     |      |     |                    |     |        |                   |
| ECMP|  FEC |     |                    |     |        |                   |
|Index| Index| Cmd |     Destination    | VID | Outlif |   MAC / CPU Code  |    Tunnel Value
 -----------------------------------------------------------------------------------------------
|  -  |314666|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |314667|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |314669|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |314671|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |315677|TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |   -   
|  -  |315682|TRAP | CoppSystemL3DstMiss|1011 |1011    | ArpTrap           |   -   
|  -  |315686|TRAP | CoppSystemL3DstMiss|1015 |1015    | ArpTrap           |   -   
|  -  |315688|TRAP | CoppSystemL3DstMiss|1017 |1017    | ArpTrap           |   -   
|  -  |315689|TRAP | CoppSystemL3DstMiss|1018 |1018    | ArpTrap           |   -   
|  -  |315690|TRAP | CoppSystemL3DstMiss|1019 |1019    | ArpTrap           |   -   
|  -  |315691|TRAP | CoppSystemL3DstMiss|1020 |1020    | ArpTrap           |   -   
|  -  |315694|TRAP | CoppSystemL3DstMiss|1023 |1023    | ArpTrap           |   -   
|  -  |318768|ROUTE| Et2                |1019 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |318770|ROUTE| Et2                |1019 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |318772|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318774|ROUTE| Et14               |1015 |103428  | bc:31:e2:c1:50:b1 |   -   
|  -  |318776|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318778|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318780|ROUTE| Et3                |1006 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |318782|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318784|ROUTE| Et2                |1019 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |318786|ROUTE| Et2                |1019 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |318788|ROUTE| Et3                |1006 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |318789|ROUTE| Et2                |1019 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |318790|ROUTE| Et3                |1006 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |318792|ROUTE| Et1                |1011 |103434  | 68:bf:6c:35:1e:31 |   -   
|  -  |318794|ROUTE| Et1                |1011 |103434  | 68:bf:6c:35:1e:31 |   -   
|  -  |318796|ROUTE| Et1                |1011 |103434  | 68:bf:6c:35:1e:31 |   -   
|  -  |318798|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318922|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318924|ROUTE| Et12               |1018 |103423  | 58:70:7f:9f:c4:03 |   -   
|  -  |318926|ROUTE| Et12               |1018 |103423  | 58:70:7f:9f:c4:03 |   -   
|  -  |318928|ROUTE| Et12               |1018 |103423  | 58:70:7f:9f:c4:03 |   -   
|  -  |318930|ROUTE| Et14               |1015 |103428  | bc:31:e2:c1:50:b1 |   -   
|  -  |318932|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   
|  -  |318934|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318936|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318938|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318940|ROUTE| Et5                |1023 |103427  | 18:5b:00:61:ac:6f |   -   
|  -  |318942|ROUTE| Et1                |1011 |103434  | 68:bf:6c:35:1e:31 |   -   
|  -  |318944|ROUTE| Et3                |1006 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |318946|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318948|ROUTE| Et2                |1019 |103421  | d4:af:f7:2f:13:96 |Mpush 20202
|  -  |318949|ROUTE| Et3                |1006 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |318950|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318952|ROUTE| Et1                |1011 |103434  | 68:bf:6c:35:1e:31 |   -   
|  -  |318956|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318958|ROUTE| Et5                |1023 |103427  | 18:5b:00:61:ac:6f |   -   
|  -  |318960|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318962|ROUTE| Et5                |1023 |103427  | 18:5b:00:61:ac:6f |   -   
|  -  |318964|ROUTE| Et2                |1019 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |318966|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318968|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318970|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318972|ROUTE| Et12               |1018 |103423  | 58:70:7f:9f:c4:03 |   -   
|  -  |318974|ROUTE| Et12               |1018 |103423  | 58:70:7f:9f:c4:03 |   -   
|  -  |318982|ROUTE| Et9                |1017 |103422  | e0:9b:27:c4:c5:84 |   -   
|  -  |318986|ROUTE| Et14               |1015 |103428  | bc:31:e2:c1:50:b1 |   -   
|  -  |318988|ROUTE| Et9                |1017 |103422  | e0:9b:27:c4:c5:84 |   -   
|  -  |318990|ROUTE| Et9                |1017 |103422  | e0:9b:27:c4:c5:84 |   -   
|  -  |318992|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   

```

## show interfaces counters queue | nz

```text
Aggregate VoQ Counters
Egress                     Traffic               Pkts             Octets           DropPkts         DropOctets
Port                       Class  
--------------------------------------------------------------------------------------------------------------
Et1                        TC1                7481220          808651826                  0                  0
Et1                        TC6                  26153            2152183                  0                  0
Et1                        TC7                  46016           11345030                  0                  0
Et2                        TC1                 600891           62499016                  0                  0
Et2                        TC6                  10658             865204                  0                  0
Et2                        TC7                  42111           10875782                  0                  0
Et3                        TC1                     96               9648                  0                  0
Et3                        TC6                  16354            1336616                  0                  0
Et3                        TC7                  38144           18714233                  0                  0
Et5                        TC1                     28               1884                  0                  0
Et5                        TC6                  13978            1137057                  0                  0
Et5                        TC7                  43480           11032189                  0                  0
Et9                        TC1                 147120           75228799                  0                  0
Et9                        TC6                  30618            2398209                  0                  0
Et9                        TC7                  48744           19120869                  0                  0
Et10                       TC1                      5                320                  0                  0
Et10                       TC7                    612             801479                  0                  0
Et11                       TC1                2048631          326049712                  0                  0
Et11                       TC6                  16770            1359473                  0                  0
Et11                       TC7                  60573           15661816                  0                  0
Et12                       TC1                 147267           75241877                  0                  0
Et12                       TC6                  27437            2213886                  0                  0
Et12                       TC7                  43889           10407513                  0                  0
Et13                       TC1                     13               1488                  0                  0
Et13                       TC6                     81               6841                  0                  0
Et13                       TC7                   1998             700199                  0                  0
Et14                       TC1                    276              21520                  0                  0
Et14                       TC6                   2171             175880                  0                  0
Et14                       TC7                  38834           31354001                  0                  0
Et15                       TC1                4964047          516258703                  0                  0
Et15                       TC6             1510629857       105744184636         2326123603       162828652210
Et15                       TC7                  67125           17496419                  0                  0
Et31                       TC1             9453790953       907563931600         1964025485       188546446560
Et31                       TC6                9176770          880947572                  0                  0
Et31                       TC7                3020953          253887695                  0                  0
Et33                       TC1                     70               4568                  0                  0
Et33                       TC7                   2606             368167                  0                  0
Et36                       TC1                     78               5080                  0                  0
Et36                       TC7                   3222             783915                  0                  0
Et39                       TC7                 130865            9683014                  0                  0
Et46/1                     TC1             9446957822       913472496086                  0                  0
Et46/1                     TC6                9174270          887839316                  0                  0
Et46/1                     TC7                    725             175834                  0                  0
OlpFap0                    TC7                     47               3196                  0                  0

Egress Queue Counters
Port                 Traffic DropPrec   DestType          OutEnqPkts      OutEnqOctets       OutDropPkts     OutDropOctets
                     Class
Et1                  TC1     DP0-3      UC                   7481284         808658226                 0                 0
Et1                  TC6     DP0-3      UC                     26153           2152183                 0                 0
Et1                  TC7     DP0-3      UC                     46018          11138337                 0                 0
Et2                  TC1     DP0-3      UC                    600956          62505776                 0                 0
Et2                  TC6     DP0-3      UC                     10658            865204                 0                 0
Et2                  TC7     DP0-3      UC                     42111          10694027                 0                 0
Et3                  TC1     DP0-3      UC                        96              9648                 0                 0
Et3                  TC6     DP0-3      UC                     16354           1336616                 0                 0
Et3                  TC7     DP0-3      UC                     38144          18528656                 0                 0
Et5                  TC1     DP0-3      UC                        28              1884                 0                 0
Et5                  TC6     DP0-3      UC                     13978           1137057                 0                 0
Et5                  TC7     DP0-3      UC                     43481          10844176                 0                 0
Et9                  TC1     DP0-3      UC                    147120          75228799                 0                 0
Et9                  TC6     DP0-3      UC                     30618           2398209                 0                 0
Et9                  TC7     DP0-3      UC                     48744          18894006                 0                 0
Et10                 TC1     DP0-3      UC                         5               320                 0                 0
Et10                 TC7     DP0-3      UC                       612            798644                 0                 0
Et11                 TC1     DP0-3      UC                   2048631         326049712                 0                 0
Et11                 TC6     DP0-3      UC                     16770           1359473                 0                 0
Et11                 TC7     DP0-3      UC                     60573          15427246                 0                 0
Et12                 TC1     DP0-3      UC                    147267          75241877                 0                 0
Et12                 TC6     DP0-3      UC                     27437           2213886                 0                 0
Et12                 TC7     DP0-3      UC                     43889          10157410                 0                 0
Et13                 TC1     DP0-3      UC                        13              1488                 0                 0
Et13                 TC6     DP0-3      UC                        81              6841                 0                 0
Et13                 TC7     DP0-3      UC                      1998            690322                 0                 0
Et14                 TC1     DP0-3      UC                       276             21520                 0                 0
Et14                 TC6     DP0-3      UC                      2171            175880                 0                 0
Et14                 TC7     DP0-3      UC                     38834          31173621                 1               241
Et15                 TC1     DP0-3      UC                   4964047         516258703                 0                 0
Et15                 TC6     DP0-3      UC                1510629857      105744184636                 0                 0
Et15                 TC7     DP0-3      UC                     67125          17277760                 0                 0
Et31                 TC1     DP0-3      UC                9453397319      905632036884                 0                 0
Et31                 TC6     DP0-3      UC                   9149659         876313660                 0                 0
Et31                 TC7     DP0-3      UC                   3020984         219575772                 0                 0
Et33                 TC1     DP0-3      UC                        70              4568                 0                 0
Et33                 TC7     DP0-3      UC                      2606            352872                 0                 0
Et36                 TC1     DP0-3      UC                        78              5080                 0                 0
Et36                 TC7     DP0-3      UC                      3222            764098                 0                 0
Et39                 TC7     DP0-3      UC                    130865           8634109                 0                 0
Et46/1               TC1     DP0-3      UC                9445887958      913369789142                 0                 0
Et46/1               TC6     DP0-3      UC                   9142765         884814836                 0                 0
Et46/1               TC7     DP0-3      UC                       725            170759                 0                 0
OlpFap0              TC3,7   DP0-3      UC                        47              2867                 0                 0

```

## show sync-e esmc detail

```text
Interface Ethernet31
Last received quality level: QL-SSU-B, SSM: 0b1000/0xff, Type: Information
Last received source MAC: e46d.7fe3.c810
Last received valid message time: 2025-02-26 15:35:14
Last received extended QL TLV: not received
Last received invalid message time: never
Received valid message count: 89848
Received invalid message count: 0
ESMC messages received by type
Event: 5
Information: 89843
ESMC messages received by QL (SSM code)
QL-PRC (0b0010): 25961
QL-SSU-B (0b1000): 63887
Last sent quality level: QL-DNU, SSM: 0b1111/0xff, Type: Information
Last sent source MAC: c4ca.2b45.a234
Last sent message time: 2025-02-27 09:55:16
Sent message count: 155801
ESMC messages sent by type
Event: 1
Information: 155800
ESMC messages sent by QL (SSM code)
QL-EEC1 (0b1011): 23
QL-DNU (0b1111): 155778

Interface Ethernet39
Last received quality level: QL-DNU, SSM: 0b1111/0xff, Type: Information
Last received source MAC: 0011.0100.0001
Last received valid message time: 2025-02-26 11:18:08
Last received extended QL TLV: not received
Last received invalid message time: never
Received valid message count: 861
Received invalid message count: 0
ESMC messages received by type
Information: 861
ESMC messages received by QL (SSM code)
QL-DNU (0b1111): 861
Last sent quality level: QL-EEC1, SSM: 0b1011/0xff, Type: Information
Last sent source MAC: c4ca.2b45.a23c
Last sent message time: 2025-02-27 09:55:16
Sent message count: 84038
ESMC messages sent by type
Event: 2
Information: 84036
ESMC messages sent by QL (SSM code)
QL-PRC (0b0010): 18022
QL-SSU-B (0b1000): 41
QL-EEC1 (0b1011): 65975

```

## show sync-e selection

```text
Input      QL        Priority Status     
---------- --------- -------- -----------
Ethernet31 QL-FAILED      127 signal fail
Ethernet39 QL-FAILED      127 signal fail

```

## show ptp

```text
PTP Mode: Boundary Clock
PTP Profile: G8275.1
Clock Identity: c4:ca:2b:ff:ff:45:a2:15
Grandmaster Clock Identity: c4:ca:2b:ff:ff:45:a2:15
Number of slave ports: 0
Number of master ports: 1
Offset From Master (nanoseconds): 0
Mean Path Delay (nanoseconds): 0
Steps Removed: 0
Skew (estimated local-to-master clock frequency ratio): 1.0
   Interface       State          Transport    Delay    
                                               Mechanism
--------------- -------------- --------------- ---------
   Et31            Master         layer2       e2e      
   Et39            Disabled       layer2       e2e      

```

## show ptp interface

```text
Interface Ethernet1
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet2
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet3
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet4
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet5
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet6
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet7
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet8
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet9
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet10
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet11
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet12
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet13
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet14
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet15
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet16
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet17
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet18
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet19
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet20
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet21
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet22
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet23
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet24
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet25
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet26
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet27
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet28
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet29
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet30
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet31
PTP: Enabled
Port state: Master 
Sync interval: 0.0625 seconds
Announce interval: 0.125 seconds
Announce interval timeout multiplier: 3
Delay mechanism: end to end
Delay request message interval: 0.0625 seconds
Local Priority: 128
Transport mode: layer 2
Destination MAC address: 01:80:c2:00:00:0e
Announce messages sent: 524894
Announce messages received: 714025
Sync messages sent: 1042229
Sync messages received: 1416704
Follow up messages sent: 1042229
Follow up messages received: 0
Delay request messages sent: 1409672
Delay request messages received: 0
Delay response messages sent: 0
Delay response messages received: 1409666
Peer delay request messages sent: 0
Peer delay request messages received: 0
Peer delay response messages sent: 0
Peer delay response messages received: 0
Peer delay response follow up messages sent: 0
Peer delay response follow up messages received: 0
Management messages sent: 0
Management messages received: 0
Signaling messages sent: 0
Signaling messages received: 0

Interface Ethernet32
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet33
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet34
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet35
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet36
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet37
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet38
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet39
PTP: Enabled
Port state: Disabled 
Sync interval: 0.0625 seconds
Announce interval: 0.125 seconds
Announce interval timeout multiplier: 3
Delay mechanism: end to end
Delay request message interval: 0.0625 seconds
Local Priority: 128
Transport mode: layer 2
Destination MAC address: 01:80:c2:00:00:0e

Interface Ethernet40
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet41/1
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet42/1
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet43/1
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet44/1
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet45/1
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet46/1
PTP: Disabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

```

## show ptp interface counters

```text
Interface Ethernet31
Announce messages sent: 524894
Announce messages received: 714025
Sync messages sent: 1042230
Sync messages received: 1416704
Follow up messages sent: 1042230
Follow up messages received: 0
Delay request messages sent: 1409672
Delay request messages received: 0
Delay response messages sent: 0
Delay response messages received: 1409666
Peer delay request messages sent: 0
Peer delay request messages received: 0
Peer delay response messages sent: 0
Peer delay response messages received: 0
Peer delay response follow up messages sent: 0
Peer delay response follow up messages received: 0
Management messages sent: 0
Management messages received: 0
Signaling messages sent: 0
Signaling messages received: 0
```

## show patch panel detail

```text
PW Fault Legend:
   ET-IN - Ethernet receive fault
   ET-OUT - Ethernet transmit fault
   TUN-IN - Tunnel receive fault
   TUN-OUT - Tunnel transmit fault
   NF - Pseudowire not forwarding (other reason)

Patch: 2-23-5G-H3C-120-PATCH_PANEL, Status: Down, Last change: 20:11:39 ago
   Connector 1: Ethernet46/1.1120
      Status: Awaiting internal VLAN
   Connector 2: BGP VPWS 2-23-5G-EVI-H3C Pseudowire H3C-120-PW
      Status: Interface unavailable
      Local MPLS label: 411299
      EVPN VPWS type: VLAN-based
      Flow label used: no
Patch: 2-23-5G-JUNIPER-179-PATCH_PANEL, Status: Down, Last change: 18:45:55 ago
   Connector 1: Ethernet46/1.1179
      Status: Awaiting internal VLAN
   Connector 2: BGP VPWS 2-23-5G-EVI-JUNIPER Pseudowire JUNIPER-179-PW
      Status: Interface unavailable
      Local MPLS label: 411298
      EVPN VPWS type: VLAN-based
      Flow label used: no
Patch: 2-23-5G-NOKIA-214-PATCH_PANEL, Status: Down, Last change: 18:45:55 ago
   Connector 1: Ethernet46/1.1214
      Status: Awaiting internal VLAN
   Connector 2: BGP VPWS 2-23-5G-EVI-NOKIA Pseudowire NOKIA-214-PW
      Status: Interface unavailable
      Local MPLS label: 411296
      EVPN VPWS type: VLAN-based
      Flow label used: no
```

## show bgp evpn instance

```text
```

## show interfaces counters queue | nz

```text
Aggregate VoQ Counters
Egress                     Traffic               Pkts             Octets           DropPkts         DropOctets
Port                       Class  
--------------------------------------------------------------------------------------------------------------
Et1                        TC1                7481220          808651826                  0                  0
Et1                        TC6                  26153            2152183                  0                  0
Et1                        TC7                  46016           11345030                  0                  0
Et2                        TC1                 600891           62499016                  0                  0
Et2                        TC6                  10658             865204                  0                  0
Et2                        TC7                  42111           10875782                  0                  0
Et3                        TC1                     96               9648                  0                  0
Et3                        TC6                  16354            1336616                  0                  0
Et3                        TC7                  38144           18714233                  0                  0
Et5                        TC1                     28               1884                  0                  0
Et5                        TC6                  13978            1137057                  0                  0
Et5                        TC7                  43480           11032189                  0                  0
Et9                        TC1                 147120           75228799                  0                  0
Et9                        TC6                  30618            2398209                  0                  0
Et9                        TC7                  48744           19120869                  0                  0
Et10                       TC1                      5                320                  0                  0
Et10                       TC7                    612             801479                  0                  0
Et11                       TC1                2048631          326049712                  0                  0
Et11                       TC6                  16770            1359473                  0                  0
Et11                       TC7                  60573           15661816                  0                  0
Et12                       TC1                 147267           75241877                  0                  0
Et12                       TC6                  27437            2213886                  0                  0
Et12                       TC7                  43889           10407513                  0                  0
Et13                       TC1                     13               1488                  0                  0
Et13                       TC6                     81               6841                  0                  0
Et13                       TC7                   1998             700199                  0                  0
Et14                       TC1                    276              21520                  0                  0
Et14                       TC6                   2171             175880                  0                  0
Et14                       TC7                  38834           31354001                  0                  0
Et15                       TC1                4964047          516258703                  0                  0
Et15                       TC6             1510629857       105744184636         2326123603       162828652210
Et15                       TC7                  67125           17496419                  0                  0
Et31                       TC1             9453790953       907563931600         1964025485       188546446560
Et31                       TC6                9176770          880947572                  0                  0
Et31                       TC7                3020953          253887695                  0                  0
Et33                       TC1                     70               4568                  0                  0
Et33                       TC7                   2606             368167                  0                  0
Et36                       TC1                     78               5080                  0                  0
Et36                       TC7                   3222             783915                  0                  0
Et39                       TC7                 130865            9683014                  0                  0
Et46/1                     TC1             9446957822       913472496086                  0                  0
Et46/1                     TC6                9174270          887839316                  0                  0
Et46/1                     TC7                    725             175834                  0                  0
OlpFap0                    TC7                     47               3196                  0                  0

Egress Queue Counters
Port                 Traffic DropPrec   DestType          OutEnqPkts      OutEnqOctets       OutDropPkts     OutDropOctets
                     Class
Et1                  TC1     DP0-3      UC                   7481284         808658226                 0                 0
Et1                  TC6     DP0-3      UC                     26153           2152183                 0                 0
Et1                  TC7     DP0-3      UC                     46018          11138337                 0                 0
Et2                  TC1     DP0-3      UC                    600956          62505776                 0                 0
Et2                  TC6     DP0-3      UC                     10658            865204                 0                 0
Et2                  TC7     DP0-3      UC                     42111          10694027                 0                 0
Et3                  TC1     DP0-3      UC                        96              9648                 0                 0
Et3                  TC6     DP0-3      UC                     16354           1336616                 0                 0
Et3                  TC7     DP0-3      UC                     38144          18528656                 0                 0
Et5                  TC1     DP0-3      UC                        28              1884                 0                 0
Et5                  TC6     DP0-3      UC                     13978           1137057                 0                 0
Et5                  TC7     DP0-3      UC                     43481          10844176                 0                 0
Et9                  TC1     DP0-3      UC                    147120          75228799                 0                 0
Et9                  TC6     DP0-3      UC                     30618           2398209                 0                 0
Et9                  TC7     DP0-3      UC                     48744          18894006                 0                 0
Et10                 TC1     DP0-3      UC                         5               320                 0                 0
Et10                 TC7     DP0-3      UC                       612            798644                 0                 0
Et11                 TC1     DP0-3      UC                   2048631         326049712                 0                 0
Et11                 TC6     DP0-3      UC                     16770           1359473                 0                 0
Et11                 TC7     DP0-3      UC                     60573          15427246                 0                 0
Et12                 TC1     DP0-3      UC                    147267          75241877                 0                 0
Et12                 TC6     DP0-3      UC                     27437           2213886                 0                 0
Et12                 TC7     DP0-3      UC                     43889          10157410                 0                 0
Et13                 TC1     DP0-3      UC                        13              1488                 0                 0
Et13                 TC6     DP0-3      UC                        81              6841                 0                 0
Et13                 TC7     DP0-3      UC                      1998            690322                 0                 0
Et14                 TC1     DP0-3      UC                       276             21520                 0                 0
Et14                 TC6     DP0-3      UC                      2171            175880                 0                 0
Et14                 TC7     DP0-3      UC                     38834          31173621                 1               241
Et15                 TC1     DP0-3      UC                   4964047         516258703                 0                 0
Et15                 TC6     DP0-3      UC                1510629857      105744184636                 0                 0
Et15                 TC7     DP0-3      UC                     67125          17277760                 0                 0
Et31                 TC1     DP0-3      UC                9453397319      905632036884                 0                 0
Et31                 TC6     DP0-3      UC                   9149659         876313660                 0                 0
Et31                 TC7     DP0-3      UC                   3020984         219575772                 0                 0
Et33                 TC1     DP0-3      UC                        70              4568                 0                 0
Et33                 TC7     DP0-3      UC                      2606            352872                 0                 0
Et36                 TC1     DP0-3      UC                        78              5080                 0                 0
Et36                 TC7     DP0-3      UC                      3222            764098                 0                 0
Et39                 TC7     DP0-3      UC                    130865           8634109                 0                 0
Et46/1               TC1     DP0-3      UC                9445887958      913369789142                 0                 0
Et46/1               TC6     DP0-3      UC                   9142765         884814836                 0                 0
Et46/1               TC7     DP0-3      UC                       725            170759                 0                 0
OlpFap0              TC3,7   DP0-3      UC                        47              2867                 0                 0

```

