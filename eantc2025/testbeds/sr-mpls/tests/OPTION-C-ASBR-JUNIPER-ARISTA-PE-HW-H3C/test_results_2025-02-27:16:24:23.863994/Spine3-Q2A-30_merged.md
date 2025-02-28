# Test results for Spine3-Q2A-30

## show version

```text
Arista DCS-7280SR3E-40YC6-F
Hardware version: 11.00
Serial number: SGD22060176
Hardware MAC address: c4ca.2b45.a215
System MAC address: c4ca.2b45.a215

Software image version: 4.33.2F
Architecture: x86_64
Internal build version: 4.33.2F-40713977.4332F
Internal build ID: 9be15ae8-4cd7-46ac-ba91-9c051db88036
Image format version: 3.0
Image optimization: Default

Uptime: 1 hour and 23 minutes
Total memory: 8099700 kB
Free memory: 4979044 kB

```

## show interfaces counters rates | nz

```text
Port      Name                 Intvl  In Mbps      %  In Kpps Out Mbps      %
Et2       Arista-PE32-Q2C-32 E  0:01      8.0   0.1%       10      8.3   0.1%
Et9       Ciena-5134-72 port 2  0:01      0.0   0.0%        0      0.0   0.0%
Et11      Juniper-156 port 590  0:01      0.0   0.0%        0      0.0   0.0%
Et14      H3C-122               0:01      8.3   0.1%       10      7.7   0.1%
Et21      Juniper-156 port 592  0:01      0.0   0.0%        0      0.0   0.0%
Et22      "Link to Juniper 179  0:01      0.0   0.0%        0      0.0   0.0%
Et31      Ciena-8140-66 port 2  0:01      0.0   0.0%        0      0.0   0.0%
Et35      Juniper-131-JCNR 42   0:01      0.0   0.0%        0      0.0   0.0%

Port      Out Kpps
Et2             10
Et14            10
```

## show ip interface brief | exclude una

```text
                                                                        Address
Interface          IP Address        Status      Protocol          MTU  Owner  
------------------ ----------------- ----------- --------------- ------ -------
Ethernet1          20.30.31.30/24    up          up               1500         
Ethernet2          20.30.32.30/24    up          up               1500         
Ethernet3          20.30.120.30/24   admin down  down                0         
Ethernet4          20.30.217.30/24   admin down  down                0         
Ethernet5          20.30.214.30/24   up          up               1500         
Ethernet6          21.30.214.30/24   down        down             1500         
Ethernet7          20.30.184.30/24   down        down             1500         
Ethernet8          21.30.217.30/24   admin down  down                0         
Ethernet9          20.30.72.30/24    up          up               1500         
Ethernet10         21.30.120.30/24   admin down  down                0         
Ethernet11         20.30.156.30/24   down        down             1500         
Ethernet12         20.30.84.30/24    up          up               1500         
Ethernet13         20.30.53.30/24    down        down             1500         
Ethernet14         20.30.122.30/24   up          up               1500         
Ethernet15         20.30.221.30/24   down        notpresent       1500         
Ethernet16         21.30.84.30/24    admin down  down                0         
Ethernet17         20.30.124.30/24   admin down  down                0         
Ethernet18         21.30.124.30/24   down        down             1500         
Ethernet19         20.30.128.30/24   admin down  down                0         
Ethernet20         21.30.128.30/24   down        notpresent       1500         
Ethernet21         21.30.156.30/24   admin down  down                0         
Ethernet29         21.30.32.30/24    admin down  down                0         
Ethernet31         20.30.66.30/24    admin down  down             1500         
Ethernet35         20.30.131.30/24   admin down  down                0         
Ethernet40         20.30.179.30/24   admin down  down                0         
Ethernet46/1.71    50.10.30.1/24     down        lowerlayerdown   9214         
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
IGP       default  Arista-PE31-Q2C-31 L2   Ethernet1          P2P               UP    22          2B                  
IGP       default  Arista-PE32-Q2C-32 L2   Ethernet2          P2P               UP    22          81                  
IGP       default  Ciena-5134-72    L2   Ethernet9          P2P               UP    27          01                  
IGP       default  Ericsson_84_R6678 L2   Ethernet12         P2P               UP    29          02                  
IGP       default  0000.0000.0122   L2   Ethernet14         P2P               UP    28          01                  
IGP       default  Nokia-SXR-214    L2   Ethernet5          P2P               UP    27          00                  
```

## show isis database detail

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00      7498  26730  1163    667 L2  0000.0000.0030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 863 s
      NLPID: 0xCC(IPv4)
      Hostname: Arista-Spine3-Q2A-30
      Area addresses: 49.0001
      Interface address: 20.30.214.30
      Interface address: 20.30.122.30
      Interface address: 20.30.84.30
      Interface address: 20.30.72.30
      Interface address: 20.30.32.30
      Interface address: 20.30.31.30
      Interface address: 10.0.0.30
      IS Neighbor          : Nokia-SXR-214.00    Metric: 100
        IPv4 Neighbor Address: 20.30.214.214
        IPv4 Interface Address: 20.30.214.30
        Adj-sid: 378556 flags: [L V] weight: 0x0
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 100
        IPv4 Neighbor Address: 20.30.84.84
        IPv4 Interface Address: 20.30.84.30
        IPv6 Neighbor Address: 2001:0:30:84::175
        Global IPv6 Interface Address: 2001:0:30:84::30
        Adj-sid: 378546 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-5134-72.00    Metric: 100
        IPv4 Neighbor Address: 20.30.72.72
        IPv4 Interface Address: 20.30.72.30
        Adj-sid: 378552 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE31-Q2C-31.00 Metric: 100
        IPv4 Neighbor Address: 20.30.31.31
        IPv4 Interface Address: 20.30.31.30
        Adj-sid: 378551 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0122.00   Metric: 25
        IPv4 Neighbor Address: 20.30.122.122
        IPv4 Interface Address: 20.30.122.30
        Adj-sid: 378554 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 50
        IPv4 Neighbor Address: 20.30.32.32
        IPv4 Interface Address: 20.30.32.30
        Adj-sid: 378553 flags: [L V] weight: 0x0
      Reachability         : 20.30.214.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.30.122.0/24 Metric: 25 Type: 1 Up
      Reachability         : 20.30.84.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.30.32.0/24 Metric: 50 Type: 1 Up
      Reachability         : 20.30.31.0/24 Metric: 100 Type: 1 Up
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
        SR Prefix-SID: 158 Flags: [N] Algorithm: 128
        SR Prefix-SID: 159 Flags: [N] Algorithm: 129
        SR Prefix-SID: 160 Flags: [N] Algorithm: 130
      Router Capabilities: Router Id: 10.0.0.30 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 237
          Exclude admin groups: 1
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 255
    Arista-PE31-Q2C-31.00-00      1053  49017   550    244 L2  0000.0000.0031.00-00  <>
      LSP received time: 2025-02-27 16:13:35
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE31-Q2C-31
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.30.31.31
      Interface address: 10.0.0.31
      Interface address: 2001:0:30:31::31
      Interface address: 2002::31
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.31.30
        IPv4 Interface Address: 20.30.31.31
        Adj-sid: 394917 flags: [L V] weight: 0x0
      Reachability         : 20.30.31.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.31/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 31 Flags: [N] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:30:31::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::31/128 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.31 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
    Arista-PE32-Q2C-32.00-00      1222  45814  1005    205 L2  0000.0000.0032.00-00  <>
      LSP received time: 2025-02-27 16:21:11
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Arista-PE32-Q2C-32
      Area addresses: 49.0002
      Interface address: 20.30.32.32
      Interface address: 209.209.209.202
      Interface address: 10.0.0.32
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.32.30
        IPv4 Interface Address: 20.30.32.32
        Adj-sid: 362157 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.175/32 Metric: 10 Type: 1 Down
        SR Prefix-SID: 175 Flags: [R N P] Algorithm: 0
      Reachability         : 209.209.209.202/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 202 Flags: [P] Algorithm: 0
      Reachability         : 20.30.32.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.32/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 32 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.32 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    Ciena-5134-72.00-00         340  33845  1097    209 L2  0000.0000.0072.00-00  <>
      LSP received time: 2025-02-27 16:22:42
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-5134-72
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.72
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.72.30
        IPv4 Interface Address: 20.30.72.72
        Adj-sid: 16000 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.72/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 72 Flags: [N] Algorithm: 0
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.72 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ericsson_84_R6678.00-00      1213  43204  1015    187 L2  0000.0000.0084.00-00  <>
      LSP received time: 2025-02-27 16:21:20
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
      Reachability         : 10.0.0.84/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 84 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.84 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    0000.0000.0122.00-00        617  27929  1155    495 L2  0000.0000.0122.00-00  <>
      LSP received time: 2025-02-27 16:23:40
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Interface address: 10.0.0.122
      Interface address: 20.30.122.122
      Interface address: 2001:0:30:122::30
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.122.30
        IPv4 Interface Address: 20.30.122.122
        Adj-sid: 1151 flags: [L V] weight: 0x0
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
      Reachability          : 2001:0:122:125::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:122:162::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:122:169::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:122:188::/64 Metric: 0 Type: 1 Up
      Reachability          : 2002::122/128 Metric: 0 Type: 1 Up
      Reachability          : 2600:30:122:190::/64 Metric: 0 Type: 1 Up
      Reachability          : 3001:0:0:1::/64 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.122 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  13
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
 U  Juniper-156-PTX10002-36QDD.00-00      2556  51350   366    282 L2  0000.0000.0156.00-00  <>
      LSP received time: 2025-02-27 16:10:31
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
        Global IPv6 Interface Address: 2001:0:30:156::156
        Adj-sid: 119 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.156/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 156 Flags: [N] Algorithm: 0
      Reachability         : 209.209.209.202/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 202 Flags: [] Algorithm: 0
      Reachability         : 10.0.0.175/32 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.156 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Nokia-SXR-214.00-00       35070   9162  1187    349 L2  0000.0000.0214.00-00  <>
      LSP received time: 2025-02-27 16:24:12
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
        Adj-sid: 30059 flags: [L V] weight: 0x0
      Reachability         : 20.30.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 209.209.209.202/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 202 Flags: [P] Algorithm: 0
      Reachability         : 10.0.0.214/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 214 Flags: [N P] Algorithm: 0
      Reachability         : 10.0.0.175/32 Metric: 10 Type: 1 Down
        SR Prefix-SID: 175 Flags: [R N P] Algorithm: 0
      Reachability (MT-IPv6): 2000::214/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.214 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  15
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0

```

## show isis database traffic-engineering

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00      7498  26730  1163    667 L2  0000.0000.0030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 863 s
      NLPID: 0xCC(IPv4)
      Hostname: Arista-Spine3-Q2A-30
      TE IPv4 router ID: 10.0.0.30
      Area addresses: 49.0001
      Interface address: 20.30.214.30
      Interface address: 20.30.122.30
      Interface address: 20.30.84.30
      Interface address: 20.30.72.30
      Interface address: 20.30.32.30
      Interface address: 20.30.31.30
      Interface address: 10.0.0.30
      IS Neighbor          : Nokia-SXR-214.00    Metric: 100
        IPv4 Neighbor Address: 20.30.214.214
        IPv4 Interface Address: 20.30.214.30
        Adj-sid: 378556 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 100
        IPv4 Neighbor Address: 20.30.84.84
        IPv4 Interface Address: 20.30.84.30
        IPv6 Neighbor Address: 2001:0:30:84::175
        Global IPv6 Interface Address: 2001:0:30:84::30
        Adj-sid: 378546 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Ciena-5134-72.00    Metric: 100
        IPv4 Neighbor Address: 20.30.72.72
        IPv4 Interface Address: 20.30.72.30
        Adj-sid: 378552 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Arista-PE31-Q2C-31.00 Metric: 100
        IPv4 Neighbor Address: 20.30.31.31
        IPv4 Interface Address: 20.30.31.30
        Adj-sid: 378551 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : 0000.0000.0122.00   Metric: 25
        IPv4 Neighbor Address: 20.30.122.122
        IPv4 Interface Address: 20.30.122.30
        Adj-sid: 378554 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 50
        IPv4 Neighbor Address: 20.30.32.32
        IPv4 Interface Address: 20.30.32.30
        Adj-sid: 378553 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      Reachability         : 20.30.214.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.30.122.0/24 Metric: 25 Type: 1 Up
      Reachability         : 20.30.84.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.30.32.0/24 Metric: 50 Type: 1 Up
      Reachability         : 20.30.31.0/24 Metric: 100 Type: 1 Up
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
        SR Prefix-SID: 158 Flags: [N] Algorithm: 128
        SR Prefix-SID: 159 Flags: [N] Algorithm: 129
        SR Prefix-SID: 160 Flags: [N] Algorithm: 130
      Router Capabilities: Router Id: 10.0.0.30 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 237
          Exclude admin groups: 1
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 255
    Arista-PE31-Q2C-31.00-00      1053  49017   550    244 L2  0000.0000.0031.00-00  <>
      LSP received time: 2025-02-27 16:13:35
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE31-Q2C-31
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.30.31.31
      Interface address: 10.0.0.31
      Interface address: 2001:0:30:31::31
      Interface address: 2002::31
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.31.30
        IPv4 Interface Address: 20.30.31.31
        Adj-sid: 394917 flags: [L V] weight: 0x0
      Reachability         : 20.30.31.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.31/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 31 Flags: [N] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:30:31::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::31/128 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.31 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
    Arista-PE32-Q2C-32.00-00      1222  45814  1005    205 L2  0000.0000.0032.00-00  <>
      LSP received time: 2025-02-27 16:21:11
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Arista-PE32-Q2C-32
      Area addresses: 49.0002
      Interface address: 20.30.32.32
      Interface address: 209.209.209.202
      Interface address: 10.0.0.32
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.32.30
        IPv4 Interface Address: 20.30.32.32
        Adj-sid: 362157 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.175/32 Metric: 10 Type: 1 Down
        SR Prefix-SID: 175 Flags: [R N P] Algorithm: 0
      Reachability         : 209.209.209.202/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 202 Flags: [P] Algorithm: 0
      Reachability         : 20.30.32.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.32/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 32 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.32 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    Ciena-5134-72.00-00         340  33845  1097    209 L2  0000.0000.0072.00-00  <>
      LSP received time: 2025-02-27 16:22:42
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
        Adj-sid: 16000 flags: [L V] weight: 0x0
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Local link ID: 1073731838
        Remote link ID: 43
        Application Specific Link Attributes:
          Standard applications: [L] RSVP-TE SR-TE LFA Flex-Algo
      Reachability         : 10.0.0.72/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 72 Flags: [N] Algorithm: 0
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.72 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ericsson_84_R6678.00-00      1213  43204  1015    187 L2  0000.0000.0084.00-00  <>
      LSP received time: 2025-02-27 16:21:20
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
      Reachability         : 10.0.0.84/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 84 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.84 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    0000.0000.0122.00-00        617  27929  1155    495 L2  0000.0000.0122.00-00  <>
      LSP received time: 2025-02-27 16:23:40
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
        Adj-sid: 1151 flags: [L V] weight: 0x0
        TE default metric: 10
        Maximum link BW: 0.00 bps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
        Local link ID: 1
        Remote link ID: 50
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
      Reachability          : 2001:0:122:125::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:122:162::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:122:169::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:122:188::/64 Metric: 0 Type: 1 Up
      Reachability          : 2002::122/128 Metric: 0 Type: 1 Up
      Reachability          : 2600:30:122:190::/64 Metric: 0 Type: 1 Up
      Reachability          : 3001:0:0:1::/64 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.122 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  13
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
 U  Juniper-156-PTX10002-36QDD.00-00      2556  51350   365    282 L2  0000.0000.0156.00-00  <>
      LSP received time: 2025-02-27 16:10:31
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
        Global IPv6 Interface Address: 2001:0:30:156::156
        Adj-sid: 119 flags: [L V] weight: 0x0
        Local link ID: 1009
        Remote link ID: 45
      Reachability         : 10.0.0.156/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 156 Flags: [N] Algorithm: 0
      Reachability         : 209.209.209.202/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 202 Flags: [] Algorithm: 0
      Reachability         : 10.0.0.175/32 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.156 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Nokia-SXR-214.00-00       35070   9162  1187    349 L2  0000.0000.0214.00-00  <>
      LSP received time: 2025-02-27 16:24:12
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
        Adj-sid: 30059 flags: [L V] weight: 0x0
        TE default metric: 10
        Maximum link BW: 80.00 Mbps
        Application Specific Link Attributes:
          Standard applications: [L] SR-TE
      Reachability         : 20.30.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 209.209.209.202/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 202 Flags: [P] Algorithm: 0
      Reachability         : 10.0.0.214/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 214 Flags: [N P] Algorithm: 0
      Reachability         : 10.0.0.175/32 Metric: 10 Type: 1 Down
        SR Prefix-SID: 175 Flags: [R N P] Algorithm: 0
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
        Remote link identifier: 54
        IPv4 interface address: 20.30.214.214
        IPv4 neighbor address: 20.30.214.30

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
Last updated: 0:40:32 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 0:40:32 ago
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
Last updated: 0:40:32 ago
Next Hop Interface
-------- ---------

```

## show isis segment-routing tunnel

```text
 Index    Endpoint              Next Hop/Tunnel Index    Interface    Labels   
-------- --------------------- ------------------------ ------------- ---------
 1        10.0.0.84/32          20.30.84.84              Ethernet12   [ 20084 ]
 2        10.0.0.175/32         TI-LFA (1)               -            [ 20175 ]
 3        10.0.0.214/32         20.30.214.214            Ethernet5    [ 20214 ]
 4        209.209.209.202/32    TI-LFA (1)               -            [ 20202 ]
 5        10.0.0.122/32         20.30.122.122            Ethernet14   [ 3 ]    
 6        10.0.0.32/32          20.30.32.32              Ethernet2    [ 3 ]    
 8        10.0.0.72/32          20.30.72.72              Ethernet9    [ 3 ]    
 9        10.0.0.31/32          20.30.31.31              Ethernet1    [ 3 ]    

```

## show isis segment-routing prefix-segments

```text

System ID: Arista-Spine3-Q2A-30			Instance: 'IGP'
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.30

Node: 11     Proxy-Node: 0      Prefix: 1       Total Segments: 12

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
   10.0.0.122/32               122   20122 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0122  L2    node with SRLG loose SPF         
   10.0.0.175/32               175   20175 Node       R:1 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node with SRLG loose SPF         
   10.0.0.175/32               175   20175 Node       R:1 N:1 P:1 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node with SRLG loose SPF         
   10.0.0.214/32               214   20214 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node with SRLG loose SPF         
   209.209.209.202/32          202   20202 Prefix     R:0 N:0 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node with SRLG loose SPF         
   209.209.209.202/32          202   20202 Prefix     R:0 N:0 P:1 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node with SRLG loose SPF         
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
 I L2     10.0.0.31/32 [115/100]
           via 20.30.31.31, Ethernet1
 I L2     10.0.0.32/32 [115/50]
           via 20.30.32.32, Ethernet2
 I L2     10.0.0.72/32 [115/110]
           via 20.30.72.72, Ethernet9
 I L2     10.0.0.84/32 [115/110]
           via 20.30.84.84, Ethernet12
 I L2     10.0.0.122/32 [115/25]
           via 20.30.122.122, Ethernet14
 I L2     10.0.0.175/32 [115/60]
           via 20.30.32.32, Ethernet2
 I L2     10.0.0.214/32 [115/100]
           via 20.30.214.214, Ethernet5
 C        10.0.30.30/32
           directly connected, Loopback1000
 C        20.30.31.0/24
           directly connected, Ethernet1
 C        20.30.32.0/24
           directly connected, Ethernet2
 C        20.30.72.0/24
           directly connected, Ethernet9
 C        20.30.84.0/24
           directly connected, Ethernet12
 C        20.30.122.0/24
           directly connected, Ethernet14
 C        20.30.214.0/24
           directly connected, Ethernet5
 I L2     30.122.190.0/24 [115/25]
           via 20.30.122.122, Ethernet14
 I L2     101.64.122.0/24 [115/25]
           via 20.30.122.122, Ethernet14
 I L2     101.74.122.0/24 [115/25]
           via 20.30.122.122, Ethernet14
 I L2     101.88.122.0/24 [115/25]
           via 20.30.122.122, Ethernet14
 I L2     101.119.122.0/24 [115/25]
           via 20.30.122.122, Ethernet14
 I L2     101.122.125.0/24 [115/25]
           via 20.30.122.122, Ethernet14
 I L2     101.122.130.0/24 [115/25]
           via 20.30.122.122, Ethernet14
 I L2     101.122.158.0/24 [115/25]
           via 20.30.122.122, Ethernet14
 I L2     101.122.162.0/24 [115/25]
           via 20.30.122.122, Ethernet14
 I L2     101.122.169.0/24 [115/25]
           via 20.30.122.122, Ethernet14
 I L2     101.122.216.0/24 [115/25]
           via 20.30.122.122, Ethernet14
 I L2     101.122.218.0/24 [115/25]
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
Displaying 6 of 14 IPv6 routing table entries
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
 C        2001:0:30:72::/64 [0/0]
           via Ethernet9, directly connected
 C        2001:0:30:84::/64 [0/0]
           via Ethernet12, directly connected
 C        2001:0:30:214::/64 [0/0]
           via Ethernet5, directly connected
 C        2002::30/128 [0/0]
           via Loopback0, directly connected

```

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 17 routes 
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
 20122   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.122.122 Ethernet14
 20175   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.214.214, Ethernet5, label imp-null(3)
 20202   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.214.214, Ethernet5, label imp-null(3)
 20214   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.214.214 Ethernet5
 378546  A[1]
                via M, 20.30.84.84, pop
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1010
 378551  A[1]
                via M, 20.30.31.31, pop
                    EgressACL: apply
                    directly connected, Ethernet1
                    68:bf:6c:35:1e:31, vlan 1016
 378552  A[1]
                via M, 20.30.72.72, pop
                    EgressACL: apply
                    directly connected, Ethernet9
                    e0:9b:27:c4:c5:84, vlan 1009
 378553  A[1]
                via M, 20.30.32.32, pop
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1013
 378554  A[1]
                via M, 20.30.122.122, pop
                    EgressACL: apply
                    directly connected, Ethernet14
                    bc:31:e2:c1:50:b1, vlan 1014
 378556  A[1]
                via M, 20.30.214.214, pop
                    EgressACL: apply
                    directly connected, Ethernet5
                    18:5b:00:61:ac:6f, vlan 1022
 394912   [0]
                via I, ipv4, vrf RED
 394913   [0]
                via I, ipv6, vrf RED
 394914   [0]
                via I, ipv4, vrf FLEXALGO
```

## show mpls lfib route

```text
MPLS forwarding table (Label [metric] Vias) - 17 routes 
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
 IP    20122    [1], 10.0.0.122/32
                via M, 20.30.122.122, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet14
 IP    20175    [1], 10.0.0.175/32
                via TI-LFA tunnel index 1, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.214.214, Ethernet5, label imp-null(3)
 IP    20202    [1], 209.209.209.202/32
                via TI-LFA tunnel index 1, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.214.214, Ethernet5, label imp-null(3)
 IP    20214    [1], 10.0.0.214/32
                via M, 20.30.214.214, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IA    378546   [1]
                via M, 20.30.84.84, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet12
 IA    378551   [1]
                via M, 20.30.31.31, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
 IA    378552   [1]
                via M, 20.30.72.72, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet9
 IA    378553   [1]
                via M, 20.30.32.32, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
 IA    378554   [1]
                via M, 20.30.122.122, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet14
 IA    378556   [1]
                via M, 20.30.214.214, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet5
 B3    394912   [0]
                via I, ipv4, vrf RED
 B3    394913   [0]
                via I, ipv6, vrf RED
 B3    394914   [0]
                via I, ipv4, vrf FLEXALGO
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
 * >      RD: 10000:128 IPv4 prefix 20.128.197.0/24
                                 10.0.0.128            -       100     0       65000 ?
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
  Last read 00:00:35, last write 00:00:13
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:25
  Keepalive timer is active, time left: 00:00:30
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 01:17:24
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was ReapplyInboundPolicy
  Last sent socket-error:Connect (Network is unreachable), Last time 01:17:46, First time 01:20:43, Repeats 7
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
      Restart-State bit: yes
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 01:17:25
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 2
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
  Message Statistics:
                                  Sent      Rcvd
    Opens:                           1         1
    Notifications:                   0         0
    Updates:                        15         2
    Keepalives:                     91        92
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:                107        95
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        10         2              2                   0
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
Local TCP address is 10.0.0.30, local port is 44569
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
    Round-trip Time (rtt/rtvar): 0.3ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 450.74 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.32, remote AS 64512, internal link
 Description: Arista-PE32-Q2C
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
  BGP state is Idle, Peer is not activated in any address-family mode
  Peering failure hint: Peer is not activated in any address-family mode
  Number of transitions to established: 0
  Last state was Idle
  Last event was UnknownEvent
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
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
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

BGP neighbor is 10.0.0.53, remote AS 64512, internal link
 Description: Arrcus-53
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
  BGP state is Idle, Peer is not activated in any address-family mode
  Peering failure hint: Peer is not activated in any address-family mode
  Number of transitions to established: 0
  Last state was Idle
  Last event was UnknownEvent
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
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
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

BGP neighbor is 10.0.0.72, remote AS 65001, internal link
 Description: Ciena-5134-72
  BGP version 4, remote router ID 10.0.0.72, VRF default
  Inherits configuration from and member of peer-group OPTION-C-RIGHT-PEER
  Last read 00:00:26, last write 00:00:44
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:34
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 01:17:26
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was ReapplyInboundPolicy
  Last sent socket-error:Connect (Network is unreachable), Last time 01:17:47, First time 01:20:43, Repeats 7
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
      Restart-State bit: yes
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
      Received 01:17:16
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  1         1
    Notifications:          0         0
    Updates:               15         2
    Keepalives:            91        78
    Route Refresh:          0         0
    Total messages:       107        81
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        11         1              1                   0
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
Local TCP address is 10.0.0.30, local port is 46661
Remote TCP address is 10.0.0.72, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1460
  Total Number of TCP retransmissions: 1
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
    TCP Throughput: 187.18 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.84, remote AS 65001, internal link
 Description: Ericsson_84
  BGP version 4, remote router ID 10.0.0.84, VRF default
  Inherits configuration from and member of peer-group OPTION-C-RIGHT-PEER
  Last read 00:00:19, last write 00:00:10
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:11
  Keepalive timer is active, time left: 00:00:12
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:31:14
  Number of transitions to established: 2
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Hold Timer Expired Error/None, Last time 00:31:27
  Last sent socket-error:Connect (Network is unreachable), Last time 00:31:16, First time 01:20:43, Repeats 11
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
      Received 00:31:14
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
  Message Statistics:
                                  Sent      Rcvd
    Opens:                           2         2
    Notifications:                   1         0
    Updates:                        24         4
    Keepalives:                    182       151
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:                209       157
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        11         1              1                   0
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
Local TCP address is 10.0.0.30, local port is 36855
Remote TCP address is 10.0.0.84, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1428
  Total Number of TCP retransmissions: 1
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,7
    Retransmission Timeout (rto): 432.0ms
    Round-trip Time (rtt/rtvar): 229.9ms/1.8ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 0.50 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.120, remote AS 64512, internal link
 Description: Huawei_120
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
  Last state was Idle
  Last event was AdminShutdown
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
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
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

BGP neighbor is 10.0.0.122, remote AS 65001, internal link
 Description: H3C_122
  BGP version 4, remote router ID 10.0.0.122, VRF default
  Inherits configuration from and member of peer-group OPTION-C-RIGHT-PEER
  Last read 00:00:23, last write 00:00:25
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:37
  Keepalive timer is active, time left: 00:00:29
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:30:28
  Number of transitions to established: 2
  Last state was OpenConfirm
  Last event was RecvKeepAlive
  Last sent notification:Hold Timer Expired Error/None, Last time 00:30:43
  Last sent socket-error:Connect (Connection refused), Last time 00:30:29, First time 01:17:27, Repeats 4
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
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  2         3
    Notifications:          2         0
    Updates:               52         4
    Keepalives:            93        81
    Route Refresh:          0         3
    Total messages:       149        91
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        11         1              1                   0
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
Remote TCP address is 10.0.0.122, remote port is 23374
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
    Round-trip Time (rtt/rtvar): 0.8ms/0.5ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 133.40 Mbps
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
  Last state was Idle
  Last event was AdminShutdown
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
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
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

BGP neighbor is 10.0.0.128, remote AS 64512, internal link
 Description: Huawei_128
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
  Last state was Idle
  Last event was AdminShutdown
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
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
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

BGP neighbor is 10.0.0.131, remote AS 64512, internal link
 Description: Juniper-131-JCNR
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
  Last state was Idle
  Last event was AdminShutdown
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
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
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

BGP neighbor is 10.0.0.156, remote AS 64512, internal link
 Description: Juniper-156
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
  Last state was Idle
  Last event was AdminShutdown
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
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
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

BGP neighbor is 10.0.0.175, remote AS 65000, external link
 Description: Juniper-175
  BGP version 4, remote router ID 10.0.0.175, VRF default
  Inherits configuration from and member of peer-group OPTION-C-LEFT-PEER
  Last read 00:00:05, last write 00:00:12
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:25
  Keepalive timer is active, time left: 00:00:11
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 01:17:09
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was ReapplyInboundPolicy
  Last sent socket-error:Connect (Network is unreachable), Last time 01:17:55, First time 01:20:43, Repeats 7
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
      Restart-State bit: yes
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
      Received 01:17:09
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 7
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are disabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are disabled
  AIGP attribute send and receive for IPv6 Unicast are disabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are disabled
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  1         1
    Notifications:          0         0
    Updates:                9        13
    Keepalives:           177       169
    Route Refresh:          0         0
    Total messages:       187       183
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         5         7              7                   0
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
Local TCP address is 10.0.0.30, local port is 39067
Remote TCP address is 10.0.0.175, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1448
  Total Number of TCP retransmissions: 12
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,7
    Retransmission Timeout (rto): 832.0ms
    Round-trip Time (rtt/rtvar): 84.8ms/168.3ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 2
    Slow-start Threshold (ssthresh): 2
    TCP Throughput: 0.27 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.179, remote AS 64512, internal link
 Description: Juniper-179
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
  Last state was Idle
  Last event was AdminShutdown
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
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
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
  Last state was Idle
  Last event was AdminShutdown
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
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
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

BGP neighbor is 10.0.0.214, remote AS 64512, internal link
 Description: Nokia-SXR-214
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
  Last state was Idle
  Last event was AdminShutdown
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
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
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

BGP neighbor is 10.0.0.216, remote AS 64512, internal link
 Description: 2-23-5G-NOKIA-216
  BGP version 4, remote router ID 0.0.0.0, VRF default
  Inherits configuration from and member of peer-group 2-23-5G-RR
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
  Last state was Idle
  Last event was AdminShutdown
  Types of communities advertised: standard extended large
  Neighbor Capabilities:
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
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

BGP neighbor is 10.0.0.217, remote AS 64512, internal link
 Description: Nokia
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
  Last state was Idle
  Last event was AdminShutdown
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
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
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

BGP neighbor is 10.0.0.221, remote AS 65001, internal link
 Description: Ribbon-221
  BGP version 4, remote router ID 0.0.0.0, VRF default
  Inherits configuration from and member of peer-group OPTION-C-RIGHT-PEER
  Last read never, last write never
  Hold time is 0, keepalive interval is 0 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:34
  Connection interval is 148 seconds
  Failed connection attempts is 35
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Network is unreachable), Last time 00:02:20, First time 01:20:43, Repeats 34
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
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
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
Local TCP address is 10.0.0.30
Remote TCP address is 10.0.0.221, remote port is 179

BGP neighbor is 10.0.1.156, remote AS 64512, internal link
 Description: 2-23-5G-JUNIPER-156
  BGP version 4, remote router ID 0.0.0.0, VRF default
  Inherits configuration from and member of peer-group 2-23-5G-RR
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
  Last state was Idle
  Last event was AdminShutdown
  Types of communities advertised: standard extended large
  Neighbor Capabilities:
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv6 Unicast is disabled
  BGP session driven failover for IPv4 Unicast is disabled
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
10.0.0.31/32       IS-IS SR IPv4  9          65                 115            
10.0.0.32/32       IS-IS SR IPv4  6          65                 115            
10.0.0.72/32       IS-IS SR IPv4  8          65                 115            
10.0.0.84/32       IS-IS SR IPv4  1          65                 115            
10.0.0.122/32      IS-IS SR IPv4  5          65                 115            
10.0.0.175/32      IS-IS SR IPv4  2          65                 115            
10.0.0.214/32      IS-IS SR IPv4  3          65                 115            
209.209.209.202/32 IS-IS SR IPv4  4          65                 115            

   IGP Metric    Metric Type
---------------- -----------
   100           metric     
   50            metric     
   110           metric     
   110           metric     
   25            metric     
   60            metric     
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
>C    10.0.0.30/32 [0 pref/0 metric] updated 01:21:00 ago
         via Loopback0, directly connected
>C    10.0.30.30/32 [0 pref/0 metric] updated 01:21:00 ago
         via Loopback1000, directly connected
>C    20.30.31.0/24 [0 pref/0 metric] updated 01:17:34 ago
         via Ethernet1, directly connected
>C    20.30.32.0/24 [0 pref/0 metric] updated 01:07:06 ago
         via Ethernet2, directly connected
>C    20.30.72.0/24 [0 pref/0 metric] updated 00:31:57 ago
         via Ethernet9, directly connected
>C    20.30.84.0/24 [0 pref/0 metric] updated 00:31:18 ago
         via Ethernet12, directly connected
>C    20.30.122.0/24 [0 pref/0 metric] updated 00:31:05 ago
         via Ethernet14, directly connected
>C    20.30.214.0/24 [0 pref/0 metric] updated 00:27:45 ago
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
>P    0.0.0.0/8 [1 pref/0 metric] updated 01:20:59 ago
         via Null0, directly connected [NF]
>P    127.0.0.0/8 [1 pref/0 metric] updated 01:20:59 ago
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
>I    10.0.0.31/32 [115 pref/100 metric] updated 00:38:23 ago
         via 20.30.31.31, Ethernet1
>I    10.0.0.32/32 [115 pref/50 metric] updated 00:38:23 ago
         via 20.30.32.32, Ethernet2
>I    10.0.0.72/32 [115 pref/110 metric] updated 00:31:45 ago
         via 20.30.72.72, Ethernet9
>I    10.0.0.84/32 [115 pref/110 metric] updated 00:11:09 ago
         via 20.30.84.84, Ethernet12
>I    10.0.0.122/32 [115 pref/25 metric] updated 00:12:05 ago
         via 20.30.122.122, Ethernet14
>I    10.0.0.175/32 [115 pref/60 metric] updated 00:00:47 ago
         via 20.30.32.32, Ethernet2
>I    10.0.0.214/32 [115 pref/100 metric] updated 00:27:39 ago
         via 20.30.214.214, Ethernet5
>I    30.122.190.0/24 [115 pref/25 metric] updated 00:12:05 ago
         via 20.30.122.122, Ethernet14
>I    101.64.122.0/24 [115 pref/25 metric] updated 00:12:05 ago
         via 20.30.122.122, Ethernet14
>I    101.74.122.0/24 [115 pref/25 metric] updated 00:12:05 ago
         via 20.30.122.122, Ethernet14
>I    101.88.122.0/24 [115 pref/25 metric] updated 00:12:05 ago
         via 20.30.122.122, Ethernet14
>I    101.119.122.0/24 [115 pref/25 metric] updated 00:12:05 ago
         via 20.30.122.122, Ethernet14
>I    101.122.125.0/24 [115 pref/25 metric] updated 00:12:05 ago
         via 20.30.122.122, Ethernet14
>I    101.122.130.0/24 [115 pref/25 metric] updated 00:12:05 ago
         via 20.30.122.122, Ethernet14
>I    101.122.158.0/24 [115 pref/25 metric] updated 00:12:05 ago
         via 20.30.122.122, Ethernet14
>I    101.122.162.0/24 [115 pref/25 metric] updated 00:12:05 ago
         via 20.30.122.122, Ethernet14
>I    101.122.169.0/24 [115 pref/25 metric] updated 00:12:05 ago
         via 20.30.122.122, Ethernet14
>I    101.122.216.0/24 [115 pref/25 metric] updated 00:12:05 ago
         via 20.30.122.122, Ethernet14
>I    101.122.218.0/24 [115 pref/25 metric] updated 00:12:05 ago
         via 20.30.122.122, Ethernet14
>I    209.209.209.202/32 [115 pref/60 metric] updated 00:00:47 ago
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
>C    2001:0:30:31::/64 [0 pref/0 metric] updated 01:17:34 ago
         via Ethernet1, directly connected
>C    2001:0:30:32::/64 [0 pref/0 metric] updated 01:07:06 ago
         via Ethernet2, directly connected
>C    2001:0:30:72::/64 [0 pref/0 metric] updated 00:31:57 ago
         via Ethernet9, directly connected
>C    2001:0:30:84::/64 [0 pref/0 metric] updated 00:31:18 ago
         via Ethernet12, directly connected
>C    2001:0:30:214::/64 [0 pref/0 metric] updated 00:27:45 ago
         via Ethernet5, directly connected
>C    2002::30/128 [0 pref/0 metric] updated 01:21:00 ago
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
>P    ::/96 [1 pref/0 metric] updated 01:20:59 ago
         via Null0, directly connected [NF]
>P    ::ffff:127.0.0.0/104 [1 pref/0 metric] updated 01:20:59 ago
         via :: [1 pref/1 metric] type ipv6
            via , directly connected
>P    fe80::/10 [1 pref/0 metric] updated 01:20:59 ago
```

## show platform sand l3 summary

```text
Number of vrfs: 5

Ipv4:
  Routes:       84  backlog:  0  unprogrammed:  0
  Adjacencies:  83  backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       20  backlog:  0  unprogrammed:  0
  Adjacencies:  83  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       14  backlog:  0  unprogrammed:  0
  Adjacencies:  6   backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4129  ecmp fecs:  0  fec entries:  4129
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  6  ecmp fecs:  0  fec entries:  6
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   84  unprogrammed:   0   
  Routes6:  20  unprogrammed6:  0   
  Backlog:  0 

Jericho2 Lpm:
  TCAM entries used:   4   Percent free:  99  ADS2 entries used:   7  Percent free:  99
  Pivot buckets used:  6   Rows used:     2   Entries Per Bucket:  1  Percent free:  99
  Route buckets used:  20  Rows used:     4   Entries Per Bucket:  5  Percent free:  99

Lem:
  IPv4  Host in Lem:            disabled
  IPv4  Prefix-lengths in Lem:  None    
  IPv6  Host in Lem:            disabled
  IPv6  Prefix-lengths in Lem:  None    
  Number of downloads:        1
  Number of overflow events:  0

Egress Arp rewrite entries in use (in each fap):
  FixedSystem: 6
Egress Arp remote rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Ip tunnel rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Mpls (for outer 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Mpls (for inner 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Sflow rewrite entries in use (in each fap):
  FixedSystem: 0

Egress rewrite chains in backlog: resource-full 0, no-interface 0

Glem entries used per fap :
  FixedSystem: 4102

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  0  allocs:  146  frees:  110  shuffles:  0  cmds:  0
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
    Non-ecmp fecs:            72  ecmp fecs:            0  
    Non-ecmp (Percent free):  99  ecmp (Percent free):  100
  ECMP FEC entries (in each bank):  2048
  ECMP FEC bank allocation:
    Unallocated Banks:      
    ECMP Bank Usage:  
      Level Bank No Reserved Entries in Use
      ----- ------- -------- --------------
          1       0      Yes              1
          1       1      Yes              0
          1       2      Yes              0
          1       3      Yes              0
          1       4      Yes              0
          1       5      Yes              0
          1       6      Yes              0
          1       7      Yes              0
          2       8      Yes              0
          2       9      Yes              0
          2      10      Yes              0
          2      11      Yes              0
          3      12      Yes              0
          3      13      Yes              0
          3      14      Yes              0
          3      15      Yes              0

Lpm Detail:
  Requests:  597  cleanses:  103  batches:  103  avg batch size:  5

Jericho Arp:
  ArpTable writes:      24988  queued      0   
  IngressTable writes:  57400  queued      0   
  Coprocessors:         1      in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  0    
  Number of uncountable MPLS tunnels:      0    
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
|0  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318768|   -   
|0  |10.0.0.30/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |10.0.0.31/32      |ROUTE| Et1                |1016 |103428  | 68:bf:6c:35:1e:31 |  -  |318838|   -   
|0  |10.0.0.32/32      |ROUTE| Et2                |1013 |103422  | d4:af:f7:2f:13:96 |  -  |318786|   -   
|0  |10.0.0.72/32      |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |  -  |318788|   -   
|0  |10.0.0.84/32      |ROUTE| Et12               |1010 |103423  | 58:70:7f:9f:c4:03 |  -  |318836|   -   
|0  |10.0.0.122/32     |ROUTE| Et14               |1014 |103424  | bc:31:e2:c1:50:b1 |  -  |318798|   -   
|0  |10.0.0.175/32     |ROUTE| Et2                |1013 |103422  | d4:af:f7:2f:13:96 |  -  |318786|   -   
|0  |10.0.0.214/32     |ROUTE| Et5                |1022 |103427  | 18:5b:00:61:ac:6f |  -  |318814|   -   
|0  |10.0.30.30/32     |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.31.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.31.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.31.31/32    |ROUTE| Et1                |1016 |103428  | 68:bf:6c:35:1e:31 |  -  |318832|   -   
|0  |20.30.31.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.31.0/24     |TRAP | CoppSystemL3DstMiss|1016 |1016    | ArpTrap           |  -  |315687|   -   
|0  |20.30.32.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.32.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.32.32/32    |ROUTE| Et2                |1013 |103422  | d4:af:f7:2f:13:96 |  -  |318794|   -   
|0  |20.30.32.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.32.0/24     |TRAP | CoppSystemL3DstMiss|1013 |1013    | ArpTrap           |  -  |315684|   -   
|0  |20.30.72.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.72.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.72.72/32    |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |  -  |318846|   -   
|0  |20.30.72.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.72.0/24     |TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |  -  |315680|   -   
|0  |20.30.84.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.84.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.84.84/32    |ROUTE| Et12               |1010 |103423  | 58:70:7f:9f:c4:03 |  -  |318834|   -   
|0  |20.30.84.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.84.0/24     |TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |  -  |315681|   -   
|0  |20.30.122.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.122.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.122.122/32  |ROUTE| Et14               |1014 |103424  | bc:31:e2:c1:50:b1 |  -  |318796|   -   
|0  |20.30.122.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.122.0/24    |TRAP | CoppSystemL3DstMiss|1014 |1014    | ArpTrap           |  -  |315685|   -   
|0  |20.30.214.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.214.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.214.214/32  |ROUTE| Et5                |1022 |103427  | 18:5b:00:61:ac:6f |  -  |318816|   -   
|0  |20.30.214.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.214.0/24    |TRAP | CoppSystemL3DstMiss|1022 |1022    | ArpTrap           |  -  |315693|   -   
|0  |30.122.190.0/24   |ROUTE| Et14               |1014 |103424  | bc:31:e2:c1:50:b1 |  -  |318798|   -   
|0  |101.64.122.0/24   |ROUTE| Et14               |1014 |103424  | bc:31:e2:c1:50:b1 |  -  |318798|   -   
|0  |101.74.122.0/24   |ROUTE| Et14               |1014 |103424  | bc:31:e2:c1:50:b1 |  -  |318798|   -   
|0  |101.88.122.0/24   |ROUTE| Et14               |1014 |103424  | bc:31:e2:c1:50:b1 |  -  |318798|   -   
|0  |101.119.122.0/24  |ROUTE| Et14               |1014 |103424  | bc:31:e2:c1:50:b1 |  -  |318798|   -   
|0  |101.122.125.0/24  |ROUTE| Et14               |1014 |103424  | bc:31:e2:c1:50:b1 |  -  |318798|   -   
|0  |101.122.130.0/24  |ROUTE| Et14               |1014 |103424  | bc:31:e2:c1:50:b1 |  -  |318798|   -   
|0  |101.122.158.0/24  |ROUTE| Et14               |1014 |103424  | bc:31:e2:c1:50:b1 |  -  |318798|   -   
|0  |101.122.162.0/24  |ROUTE| Et14               |1014 |103424  | bc:31:e2:c1:50:b1 |  -  |318798|   -   
|0  |101.122.169.0/24  |ROUTE| Et14               |1014 |103424  | bc:31:e2:c1:50:b1 |  -  |318798|   -   
|0  |101.122.216.0/24  |ROUTE| Et14               |1014 |103424  | bc:31:e2:c1:50:b1 |  -  |318798|   -   
|0  |101.122.218.0/24  |ROUTE| Et14               |1014 |103424  | bc:31:e2:c1:50:b1 |  -  |318798|   -   
|0  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|0  |209.209.209.202/32|ROUTE| Et2                |1013 |103422  | d4:af:f7:2f:13:96 |  -  |318786|   -   
|0  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|1  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318772|   -   
|1  |10.128.0.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|1  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|1  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|2  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318774|   -   
|2  |10.0.30.30/32     |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|2  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|2  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|3  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318776|   -   
|3  |10.0.0.30/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|3  |10.0.0.31/32      |DROP | DROP               |0    |  -     |                   |  -  |318842|   -   
|3  |50.10.31.0/24     |DROP | DROP               |0    |  -     |                   |  -  |318842|   -   
|3  |50.10.53.0/24     |DROP | DROP               |0    |  -     |                   |  -  |318854|   -   
|3  |50.10.72.0/24     |DROP | DROP               |0    |  -     |                   |  -  |318844|   -   
|3  |50.10.84.0/24     |DROP | DROP               |0    |  -     |                   |  -  |318784|   -   
|3  |50.10.122.0/24    |DROP | DROP               |0    |  -     |                   |  -  |318808|   -   
|3  |50.10.128.0/24    |DROP | DROP               |0    |  -     |                   |  -  |318848|   -   
|3  |50.10.179.0/24    |DROP | DROP               |0    |  -     |                   |  -  |318850|   -   
|3  |50.10.184.0/24    |DROP | DROP               |0    |  -     |                   |  -  |318856|   -   
|3  |50.10.216.0/24    |DROP | DROP               |0    |  -     |                   |  -  |318852|   -   
|3  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|3  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|4  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318780|   -   
|4  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|4  |192.168.20.0/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|4  |192.168.20.30/32  |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|4  |192.168.21.255/32 |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|4  |192.168.20.0/23   |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|4  |0.0.0.0/0         |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   

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
|  -  |315680|TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |   -   
|  -  |315681|TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |   -   
|  -  |315684|TRAP | CoppSystemL3DstMiss|1013 |1013    | ArpTrap           |   -   
|  -  |315685|TRAP | CoppSystemL3DstMiss|1014 |1014    | ArpTrap           |   -   
|  -  |315687|TRAP | CoppSystemL3DstMiss|1016 |1016    | ArpTrap           |   -   
|  -  |315693|TRAP | CoppSystemL3DstMiss|1022 |1022    | ArpTrap           |   -   
|  -  |318768|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318770|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318772|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318774|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318776|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318778|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318780|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318782|ROUTE| Et12               |1010 |103423  | 58:70:7f:9f:c4:03 |   -   
|  -  |318784|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318786|ROUTE| Et2                |1013 |103422  | d4:af:f7:2f:13:96 |   -   
|  -  |318788|ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |   -   
|  -  |318790|ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |   -   
|  -  |318792|ROUTE| Et2                |1013 |103422  | d4:af:f7:2f:13:96 |   -   
|  -  |318794|ROUTE| Et2                |1013 |103422  | d4:af:f7:2f:13:96 |   -   
|  -  |318796|ROUTE| Et14               |1014 |103424  | bc:31:e2:c1:50:b1 |   -   
|  -  |318798|ROUTE| Et14               |1014 |103424  | bc:31:e2:c1:50:b1 |   -   
|  -  |318800|ROUTE| Et14               |1014 |103424  | bc:31:e2:c1:50:b1 |   -   
|  -  |318802|ROUTE| Et12               |1010 |103423  | 58:70:7f:9f:c4:03 |   -   
|  -  |318804|ROUTE| Et2                |1013 |103422  | d4:af:f7:2f:13:96 |   -   
|  -  |318805|ROUTE| Et5                |1022 |103427  | 18:5b:00:61:ac:6f |   -   
|  -  |318808|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318814|ROUTE| Et5                |1022 |103427  | 18:5b:00:61:ac:6f |   -   
|  -  |318816|ROUTE| Et5                |1022 |103427  | 18:5b:00:61:ac:6f |   -   
|  -  |318818|ROUTE| Et5                |1022 |103427  | 18:5b:00:61:ac:6f |   -   
|  -  |318832|ROUTE| Et1                |1016 |103428  | 68:bf:6c:35:1e:31 |   -   
|  -  |318834|ROUTE| Et12               |1010 |103423  | 58:70:7f:9f:c4:03 |   -   
|  -  |318836|ROUTE| Et12               |1010 |103423  | 58:70:7f:9f:c4:03 |   -   
|  -  |318838|ROUTE| Et1                |1016 |103428  | 68:bf:6c:35:1e:31 |   -   
|  -  |318840|ROUTE| Et1                |1016 |103428  | 68:bf:6c:35:1e:31 |   -   
|  -  |318842|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318844|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318846|ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |   -   
|  -  |318848|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318850|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318852|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318854|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318856|DROP | DROP               |0    |  -     |                   |   -   

```

## show interfaces counters queue | nz

```text
Aggregate VoQ Counters
Egress                     Traffic               Pkts             Octets           DropPkts         DropOctets
Port                       Class  
--------------------------------------------------------------------------------------------------------------
Et1                        TC1                     63               6704                  0                  0
Et1                        TC6                   1213             105161                  0                  0
Et1                        TC7                   3336             606466                  0                  0
Et2                        TC1                6071173         2900538768                  0                  0
Et2                        TC6                    959              78488                  0                  0
Et2                        TC7                   3344             617773                  0                  0
Et5                        TC1                     10                640                  0                  0
Et5                        TC6                    645              55114                  0                  0
Et5                        TC7                   1408             257439                  0                  0
Et9                        TC1                     24               2588                  0                  0
Et9                        TC6                    912              87276                  0                  0
Et9                        TC7                   3036            1167658                  0                  0
Et11                       TC1                7732102         1666070874                  0                  0
Et11                       TC6                    904              75154                  0                  0
Et11                       TC7                   2381             433508                  0                  0
Et12                       TC1                4843565         2470062540                  0                  0
Et12                       TC6                   1096             101106                  0                  0
Et12                       TC7                   3324             692773                  0                  0
Et14                       TC1                6201902          620189990                  0                  0
Et14                       TC6                    764              71365                  0                  0
Et14                       TC7                   2760            1985622                  0                  0
Et31                       TC1                     36               3856                  0                  0
Et31                       TC6                    676              51972                  0                  0
Et31                       TC7                 114144            9509518                  0                  0
Et33                       TC7                     15               3750                  0                  0
Et36                       TC7                    186              46872                  0                  0
Et39                       TC7                   4671             331641                  0                  0

Egress Queue Counters
Port                 Traffic DropPrec   DestType          OutEnqPkts      OutEnqOctets       OutDropPkts     OutDropOctets
                     Class
Et1                  TC1     DP0-3      UC                        63              6704                 0                 0
Et1                  TC6     DP0-3      UC                      1213            105161                 0                 0
Et1                  TC7     DP0-3      UC                      3340            593263                 0                 0
Et2                  TC1     DP0-3      UC                   6071658        2900589208                 0                 0
Et2                  TC6     DP0-3      UC                       959             78488                 0                 0
Et2                  TC7     DP0-3      UC                      3346            604343                 0                 0
Et5                  TC1     DP0-3      UC                        10               640                 0                 0
Et5                  TC6     DP0-3      UC                       645             55114                 0                 0
Et5                  TC7     DP0-3      UC                      1410            252254                 0                 0
Et9                  TC1     DP0-3      UC                        24              2588                 0                 0
Et9                  TC6     DP0-3      UC                       912             87276                 0                 0
Et9                  TC7     DP0-3      UC                      3036           1152733                 2               373
Et11                 TC1     DP0-3      UC                   7732102        1666070874                 0                 0
Et11                 TC6     DP0-3      UC                       904             75154                 0                 0
Et11                 TC7     DP0-3      UC                      2381            424569                 0                 0
Et12                 TC1     DP0-3      UC                   4843565        2470062540                 0                 0
Et12                 TC6     DP0-3      UC                      1096            101106                 0                 0
Et12                 TC7     DP0-3      UC                      3324            675191                 0                 0
Et14                 TC1     DP0-3      UC                   6201186         620118390                 0                 0
Et14                 TC6     DP0-3      UC                       764             71365                 0                 0
Et14                 TC7     DP0-3      UC                      2760           1972364                 0                 0
Et31                 TC1     DP0-3      UC                        36              3856                 0                 0
Et31                 TC6     DP0-3      UC                       676             51972                 0                 0
Et31                 TC7     DP0-3      UC                    112235           8161560              1909            122234
Et33                 TC7     DP0-3      UC                        15              3645                 0                 0
Et36                 TC7     DP0-3      UC                       186             45570                 0                 0
Et39                 TC7     DP0-3      UC                      4669            298816                 2               128

```

## show sync-e esmc detail

```text
Interface Ethernet31
Last received quality level: n/a, SSM: n/a, Type: n/a
Last received source MAC: n/a
Last received valid message time: never
Last received extended QL TLV: not received
Last received invalid message time: never
Received valid message count: 0
Received invalid message count: 0
Last sent quality level: QL-EEC1, SSM: 0b1011/0xff, Type: Information
Last sent source MAC: c4ca.2b45.a234
Last sent message time: 2025-02-27 16:24:36
Sent message count: 4675
ESMC messages sent by type
Information: 4675
ESMC messages sent by QL (SSM code)
QL-EEC1 (0b1011): 4675

Interface Ethernet39
Last received quality level: n/a, SSM: n/a, Type: n/a
Last received source MAC: n/a
Last received valid message time: never
Last received extended QL TLV: not received
Last received invalid message time: never
Received valid message count: 0
Received invalid message count: 0
Last sent quality level: QL-EEC1, SSM: 0b1011/0xff, Type: Information
Last sent source MAC: c4ca.2b45.a23c
Last sent message time: 2025-02-27 16:24:36
Sent message count: 4675
ESMC messages sent by type
Information: 4675
ESMC messages sent by QL (SSM code)
QL-EEC1 (0b1011): 4675

```

## show sync-e selection

```text
Input      QL        Priority Status     
---------- --------- -------- -----------
Ethernet31 QL-DNU         127 disabled   
Ethernet39 QL-FAILED      127 signal fail

```

## show ptp

```text
PTP Mode: Boundary Clock
PTP Profile: G8275.1
Clock Identity: c4:ca:2b:ff:ff:45:a2:15
Grandmaster Clock Identity: c4:ca:2b:ff:ff:45:a2:15
Number of slave ports: 0
Number of master ports: 0
Offset From Master (nanoseconds): 0
Mean Path Delay (nanoseconds): 0
Steps Removed: 0
Skew (estimated local-to-master clock frequency ratio): 1.0
   Interface       State          Transport    Delay    
                                               Mechanism
--------------- -------------- --------------- ---------
   Et31            Disabled       layer2       e2e      
   Et39            Disabled       layer2       e2e      

```

## show ptp interface

```text
Interface Ethernet1
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet2
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet3
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet4
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet5
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet6
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet7
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet8
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet9
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet10
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet11
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet12
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet13
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet14
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet15
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet16
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet17
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet18
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet19
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet20
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet21
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet22
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet23
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet24
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet25
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet26
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet27
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet28
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet29
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet30
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet31
PTP: Enabled
Management message forwarding: Enabled
Port state: Disabled 
Sync interval: 0.0625 seconds
Announce interval: 0.125 seconds
Announce interval timeout multiplier: 3
Delay mechanism: end to end
Delay request message interval: 0.0625 seconds
Local Priority: 128
Transport mode: layer 2
Destination MAC address: 01:80:c2:00:00:0e

Interface Ethernet32
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet33
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet34
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet35
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet36
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet37
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet38
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet39
PTP: Enabled
Management message forwarding: Enabled
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
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet41/1
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet42/1
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet43/1
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet44/1
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet45/1
PTP: Disabled
Management message forwarding: Enabled
Port state: Initializing 
Sync interval: 1.0 seconds
Announce interval: 1.0 seconds
Delay mechanism: end to end
Delay request message interval: 1.0 seconds
Local Priority: 128
Transport mode: layer 2

Interface Ethernet46/1
PTP: Disabled
Management message forwarding: Enabled
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
```

## show patch panel detail

```text
PW Fault Legend:
   ET-IN - Ethernet receive fault
   ET-OUT - Ethernet transmit fault
   TUN-IN - Tunnel receive fault
   TUN-OUT - Tunnel transmit fault
   NF - Pseudowire not forwarding (other reason)

Patch: 2-23-5G-H3C-120-PATCH_PANEL, Status: Down, Last change: 1:21:11 ago
   Connector 1: Ethernet46/1.1120
      Status: Awaiting internal VLAN
      Error disable triggers: none
   Connector 2: BGP VPWS 2-23-5G-EVI-H3C Pseudowire H3C-120-PW
      Status: Interface unavailable
      Local MPLS label: 362146
      EVPN VPWS type: VLAN-based
      Flow label used: no
Patch: 2-23-5G-JUNIPER-179-PATCH_PANEL, Status: Down, Last change: 1:21:11 ago
   Connector 1: Ethernet46/1.1179
      Status: Awaiting internal VLAN
      Error disable triggers: none
   Connector 2: BGP VPWS 2-23-5G-EVI-JUNIPER Pseudowire JUNIPER-179-PW
      Status: Interface unavailable
      Local MPLS label: 362144
      EVPN VPWS type: VLAN-based
      Flow label used: no
Patch: 2-23-5G-NOKIA-214-PATCH_PANEL, Status: Down, Last change: 1:21:11 ago
   Connector 1: Ethernet46/1.1214
      Status: Awaiting internal VLAN
      Error disable triggers: none
   Connector 2: BGP VPWS 2-23-5G-EVI-NOKIA Pseudowire NOKIA-214-PW
      Status: Interface unavailable
      Local MPLS label: 362145
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
Et1                        TC1                     63               6704                  0                  0
Et1                        TC6                   1213             105161                  0                  0
Et1                        TC7                   3336             606466                  0                  0
Et2                        TC1                6071173         2900538768                  0                  0
Et2                        TC6                    959              78488                  0                  0
Et2                        TC7                   3344             617773                  0                  0
Et5                        TC1                     10                640                  0                  0
Et5                        TC6                    645              55114                  0                  0
Et5                        TC7                   1408             257439                  0                  0
Et9                        TC1                     24               2588                  0                  0
Et9                        TC6                    912              87276                  0                  0
Et9                        TC7                   3036            1167658                  0                  0
Et11                       TC1                7732102         1666070874                  0                  0
Et11                       TC6                    904              75154                  0                  0
Et11                       TC7                   2381             433508                  0                  0
Et12                       TC1                4843565         2470062540                  0                  0
Et12                       TC6                   1096             101106                  0                  0
Et12                       TC7                   3324             692773                  0                  0
Et14                       TC1                6201902          620189990                  0                  0
Et14                       TC6                    764              71365                  0                  0
Et14                       TC7                   2760            1985622                  0                  0
Et31                       TC1                     36               3856                  0                  0
Et31                       TC6                    676              51972                  0                  0
Et31                       TC7                 114144            9509518                  0                  0
Et33                       TC7                     15               3750                  0                  0
Et36                       TC7                    186              46872                  0                  0
Et39                       TC7                   4671             331641                  0                  0

Egress Queue Counters
Port                 Traffic DropPrec   DestType          OutEnqPkts      OutEnqOctets       OutDropPkts     OutDropOctets
                     Class
Et1                  TC1     DP0-3      UC                        63              6704                 0                 0
Et1                  TC6     DP0-3      UC                      1213            105161                 0                 0
Et1                  TC7     DP0-3      UC                      3340            593263                 0                 0
Et2                  TC1     DP0-3      UC                   6071658        2900589208                 0                 0
Et2                  TC6     DP0-3      UC                       959             78488                 0                 0
Et2                  TC7     DP0-3      UC                      3346            604343                 0                 0
Et5                  TC1     DP0-3      UC                        10               640                 0                 0
Et5                  TC6     DP0-3      UC                       645             55114                 0                 0
Et5                  TC7     DP0-3      UC                      1410            252254                 0                 0
Et9                  TC1     DP0-3      UC                        24              2588                 0                 0
Et9                  TC6     DP0-3      UC                       912             87276                 0                 0
Et9                  TC7     DP0-3      UC                      3036           1152733                 2               373
Et11                 TC1     DP0-3      UC                   7732102        1666070874                 0                 0
Et11                 TC6     DP0-3      UC                       904             75154                 0                 0
Et11                 TC7     DP0-3      UC                      2381            424569                 0                 0
Et12                 TC1     DP0-3      UC                   4843565        2470062540                 0                 0
Et12                 TC6     DP0-3      UC                      1096            101106                 0                 0
Et12                 TC7     DP0-3      UC                      3324            675191                 0                 0
Et14                 TC1     DP0-3      UC                   6201186         620118390                 0                 0
Et14                 TC6     DP0-3      UC                       764             71365                 0                 0
Et14                 TC7     DP0-3      UC                      2760           1972364                 0                 0
Et31                 TC1     DP0-3      UC                        36              3856                 0                 0
Et31                 TC6     DP0-3      UC                       676             51972                 0                 0
Et31                 TC7     DP0-3      UC                    112235           8161560              1909            122234
Et33                 TC7     DP0-3      UC                        15              3645                 0                 0
Et36                 TC7     DP0-3      UC                       186             45570                 0                 0
Et39                 TC7     DP0-3      UC                      4669            298816                 2               128

```

