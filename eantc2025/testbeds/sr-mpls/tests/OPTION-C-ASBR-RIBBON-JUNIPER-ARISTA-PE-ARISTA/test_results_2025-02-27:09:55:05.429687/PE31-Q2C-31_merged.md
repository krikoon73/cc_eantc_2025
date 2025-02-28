# Test results for PE31-Q2C-31

## show version

```text
Arista DCS-7280SR3-48YC8-F
Hardware version: 12.12
Serial number: HBG243203DT
Hardware MAC address: 68bf.6c35.1e31
System MAC address: 68bf.6c35.1e31

Software image version: 4.33.1.1F
Architecture: x86_64
Internal build version: 4.33.1.1F-40155285.43311F
Internal build ID: 2170da2c-90c5-421e-adc1-86266708cffc
Image format version: 3.0
Image optimization: Default

Uptime: 1 week, 3 days, 3 hours and 2 minutes
Total memory: 8099700 kB
Free memory: 4965724 kB

```

## show interfaces counters rates | nz

```text
Port      Name                Intvl  In Mbps      %  In Kpps Out Mbps      %
Et1       Arista_Spine30_Eth2  0:05      3.9   0.0%        5      4.2   0.0%
Et40                           0:05      3.9   0.0%        5      3.9   0.0%
Ma1                            0:05      0.0   0.0%        0     10.0   1.0%

Port      Out Kpps
Et1              5
Et40             5
```

## show ip interface brief | exclude una

```text
                                                                        Address
Interface       IP Address          Status        Protocol        MTU   Owner  
--------------- ------------------- ------------- ----------- --------- -------
Ethernet1       20.30.31.31/24      up            up             1500          
Ethernet5       20.31.175.31/24     admin down    down           1500          
Ethernet40.4    50.10.31.1/24       up            up             1500          
Loopback0       10.0.0.31/32        up            up            65535          
Loopback1000    10.0.0.31/32        up            up            65535          
Management1     192.168.20.31/23    up            up             1500          

```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
IGP       default  Arista-Spine3-Q2A-30 L2   Ethernet1          P2P               UP    24          44                  
```

## show isis database detail

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00      7332  39141  1090    988 L2  0000.0000.0030.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
    Arista-Spine3-Q2A-30.00-01        98  38964   807    305 L2  0000.0000.0030.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 857 s
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
 U  Juniper-156-PTX10002-36QDD.00-00      2465  48498   414    316 L2  0000.0000.0156.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
    Nokia-SXR-214.00-00       34879  28493   609    349 L2  0000.0000.0214.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
      Hostname: 221
 U  221.00-02                   124  28431   475    205 L2  0221.0221.0221.00-02  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00      7332  39141  1090    988 L2  0000.0000.0030.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
            Administrative group (Color): 2
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Nokia-SXR-214.00    Metric: 100
        IPv4 Neighbor Address: 20.30.214.214
        IPv4 Interface Address: 20.30.214.30
        Adj-sid: 378660 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 2
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Ciena-8140-66.00    Metric: 100
        IPv4 Neighbor Address: 20.30.66.66
        IPv4 Interface Address: 20.30.66.30
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 2
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 100
        IPv4 Neighbor Address: 20.30.84.84
        IPv4 Interface Address: 20.30.84.30
        Adj-sid: 378648 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 2
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Ciena-5134-72.00    Metric: 100
        IPv4 Neighbor Address: 20.30.72.72
        IPv4 Interface Address: 20.30.72.30
        Adj-sid: 378684 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 2
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor (MT-IPv6): Arista-PE32-Q2C-32.00 Metric: 10
        Adj-sid: 378651 flags: [L V F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 2
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor (MT-IPv6): Ericsson_84_R6678.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:84::175
        Global IPv6 Interface Address: 2001:0:30:84::30
        Adj-sid: 378649 flags: [L V F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 2
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
    Arista-Spine3-Q2A-30.00-01        98  38964   807    305 L2  0000.0000.0030.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      Interface address: 2001:0:30:31::30
      IS Neighbor          : 0000.0000.0120.00   Metric: 100
        IPv4 Neighbor Address: 20.30.120.120
        IPv4 Interface Address: 20.30.120.30
        Adj-sid: 378652 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 2
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : 0000.0000.0122.00   Metric: 100
        IPv4 Neighbor Address: 20.30.122.122
        IPv4 Interface Address: 20.30.122.30
        Adj-sid: 378700 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 2
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Arista-PE31-Q2C-31.00 Metric: 75
        IPv4 Neighbor Address: 20.30.31.31
        IPv4 Interface Address: 20.30.31.30
        Adj-sid: 378688 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 2
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor (MT-IPv6): Arista-PE31-Q2C-31.00 Metric: 10
        Adj-sid: 378689 flags: [L V F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 2
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      Reachability (MT-IPv6): 2001:0:30:31::/64 Metric: 10 Type: 1 Up
    Arista-PE31-Q2C-31.00-00      1013   2713  1157    266 L2  0000.0000.0031.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 857 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
    Nokia-SXR-214.00-00       34879  28493   609    349 L2  0000.0000.0214.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
      Hostname: 221
 U  221.00-02                   124  28431   475    205 L2  0221.0221.0221.00-02  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      Interface address: 20.30.221.221
      Interface address: 10.0.0.221
      Interface address: 209.209.209.202
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 100
        IPv4 Neighbor Address: 20.30.221.30
        IPv4 Interface Address: 20.30.221.221
        Adj-sid: 756648 flags: [L V B] weight: 0x0
        Adj-sid: 756647 flags: [L V] weight: 0x0
        Administrative group (Color): 2
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
```

## show isis flex-algo path detail

```text
```

## show isis segment-routing tunnel

```text
 Index   Endpoint             Next Hop/Tunnel Index       Interface   Labels   
------- -------------------- --------------------------- ------------ ---------
 1       10.0.0.175/32        20.30.31.30                 Ethernet1   [ 20175 ]
 2       10.0.0.84/32         20.30.31.30                 Ethernet1   [ 20084 ]
 4       10.0.0.30/32         20.30.31.30                 Ethernet1   [ 3 ]    
 7       10.0.0.120/32        20.30.31.30                 Ethernet1   [ 20120 ]
 8       10.0.0.72/32         20.30.31.30                 Ethernet1   [ 20072 ]
 9       10.0.0.32/32         20.30.31.30                 Ethernet1   [ 20032 ]
 10      10.0.0.214/32        20.30.31.30                 Ethernet1   [ 20214 ]
 20      209.209.209.202/32   20.30.31.30                 Ethernet1   [ 20202 ]
 23      2002::30/128         fe80::c6ca:2bff:fe45:a215   Ethernet1   [ 3 ]    
 25      10.0.0.122/32        20.30.31.30                 Ethernet1   [ 20122 ]

```

## show isis segment-routing prefix-segments

```text

System ID: Arista-PE31-Q2C-31			Instance: 'IGP'
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.31

Node: 15     Proxy-Node: 0      Prefix: 2       Total Segments: 17

Flag Descriptions: R: Re-advertised, N: Node Segment, P: no-PHP
                   E: Explicit-NULL, V: Value, L: Local
Segment status codes: * - Self originated Prefix, L1 - level 1, L2 - level 2, ! - SR-unreachable,
                      # - Some IS-IS next-hops are SR-unreachable
   Prefix                      SID   Label Type       Flags                        System ID       Level Protection  Algorithm   
   ------------------------- ----- ------- ---------- ---------------------------- --------------- ----- ----------- -------------
   10.0.0.30/32                 30   20030 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node        SPF         
   10.0.0.30/32                158   20158 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected 128         
   10.0.0.30/32                159   20159 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected 129         
   10.0.0.30/32                160   20160 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected 130         
*  10.0.0.31/32                 31   20031 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE31-Q2C-31 L2    unprotected SPF         
   10.0.0.32/32                 32   20032 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node        SPF         
   10.0.0.72/32                 72   20072 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    node        SPF         
   10.0.0.84/32                 84   20084 Node       R:0 N:1 P:1 E:0 V:0 L:0      Ericsson_84_R6678 L2    node        SPF         
   10.0.0.120/32               120   20120 Prefix     R:1 N:0 P:1 E:0 V:0 L:0      0000.0000.0120  L2    node        SPF         
   10.0.0.122/32               122   20122 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0122  L2    node        SPF         
   10.0.0.175/32               175   20175 Node       R:1 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node        SPF         
   10.0.0.175/32               175   20175 Node       R:1 N:1 P:1 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node        SPF         
   10.0.0.214/32               214   20214 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node        SPF         
   209.209.209.202/32          202   20202 Prefix     R:0 N:0 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node        SPF         
   209.209.209.202/32          202   20202 Prefix     R:0 N:0 P:1 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node        SPF         
   209.209.209.202/32          202   20202 Prefix     R:0 N:0 P:1 E:0 V:0 L:0      0000.0000.0120  L2    node        SPF         
   2002::30/128                430   20430 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node        SPF         
   2002::30/128                558   20558 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected 128         
   2002::30/128                559   20559 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected 129         
   2002::30/128                560   20560 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected 130         
```

## show ip ospf segment-routing

```text
OSPF Instance ID: 1
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.31
SR Global Block( SRGB ): Base: 20000           	Size: 2000            

OSPF Reachability Algorithm : SPF (0)

Number of OSPF segment routing capable nodes excluding self: 0

Self-Originated Segment Statistics:
Node-Segments       : 1
Prefix-Segments     : 0
Proxy-Node-Segments : 0
Adjacency Segments  : 0

```

## show ip ospf segment-routing global-blocks

```text
OSPF Instance ID: 1
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.31
Number of OSPF segment routing capable nodes excluding self: 0

   Router ID        Base    Size
--------------- ----------- ----
   10.0.0.31       20000    2000

```

## show ip ospf segment-routing bindings

```text
10.0.0.31/32
   Local binding:  Label: imp-null
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

 I L2     10.0.0.30/32 [115/10]
           via 20.30.31.30, Ethernet1
 C        10.0.0.31/32
           directly connected, Loopback0
 I L2     10.0.0.32/32 [115/60]
           via 20.30.31.30, Ethernet1
 I L2     10.0.0.66/32 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     10.0.0.72/32 [115/120]
           via 20.30.31.30, Ethernet1
 I L2     10.0.0.84/32 [115/120]
           via 20.30.31.30, Ethernet1
 I L2     10.0.0.120/32 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     10.0.0.122/32 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     10.0.0.175/32 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     10.0.0.214/32 [115/110]
           via 20.30.31.30, Ethernet1
 C        20.30.31.0/24
           directly connected, Ethernet1
 I L2     20.30.32.0/24 [115/60]
           via 20.30.31.30, Ethernet1
 I L2     20.30.66.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     20.30.72.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     20.30.84.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     20.30.120.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     20.30.122.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     20.30.214.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     30.122.190.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     101.64.122.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     101.74.122.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     101.88.122.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     101.119.122.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     101.122.125.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     101.122.130.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     101.122.158.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     101.122.162.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     101.122.169.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     101.122.216.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     101.122.218.0/24 [115/110]
           via 20.30.31.30, Ethernet1
 I L2     209.209.209.202/32 [115/70]
           via 20.30.31.30, Ethernet1


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

 C        10.0.0.31/32
           directly connected, Loopback1000
 C        50.10.31.0/24
           directly connected, Ethernet40.4
 B I      50.10.53.0/24 [200/0]
           via 10.0.0.53/32, BGP LU tunnel index 228, label 970002
              via IS-IS SR tunnel index 20, label 20053
                 via ::, NextLevelFecId2493952.27, label 20202
 B I      50.10.72.0/24 [200/0]
           via 10.0.0.72/32, IS-IS SR tunnel index 8, label 62000
              via 20.30.31.30, Ethernet1, label 20072
 B I      50.10.84.0/24 [200/0]
           via 10.0.0.84/32, IS-IS SR tunnel index 2, label 720896
              via 20.30.31.30, Ethernet1, label 20084
 B I      50.10.122.0/24 [200/0]
           via 10.0.0.122/32, IS-IS SR tunnel index 25, label 1279
              via 20.30.31.30, Ethernet1, label 20122
 B I      50.10.128.0/24 [200/0]
           via 10.0.0.128/32, BGP LU tunnel index 231, label 48080
              via IS-IS SR tunnel index 20, label 20128
                 via ::, NextLevelFecId2493952.27, label 20202
 B I      50.10.179.0/24 [200/0]
           via 10.0.0.179/32, BGP LU tunnel index 236, label 16
              via IS-IS SR tunnel index 20, label 20179
                 via ::, NextLevelFecId2493952.27, label 20202
 B I      50.10.184.0/24 [200/0]
           via 10.0.0.184/32, BGP LU tunnel index 239, label 16
              via IS-IS SR tunnel index 20, label 20184
                 via ::, NextLevelFecId2493952.27, label 20202
 B I      50.10.216.0/24 [200/0]
           via 10.0.0.216/32, BGP LU tunnel index 221, label 1048571
              via IS-IS SR tunnel index 20, label 20216
                 via ::, NextLevelFecId2493952.27, label 20202


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
Displaying 10 of 14 IPv6 routing table entries
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
 I L2     2001:0:30:32::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:66::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:72::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:84::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:120::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:214::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2002::30/128 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 C        2002::31/128 [0/0]
           via Loopback0, directly connected
 I L2     2002::32/128 [115/30]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1

```

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 20 routes 
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

 20030   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.31.30 Ethernet1
 20032   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.31.30 Ethernet1
 20053   A[1]
                via M, ::, swap 20053
                    EgressACL: bypass
                  via IS-IS SR tunnel index 20
                    via 20.30.31.30, Ethernet1, label 20202
 20066   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via IS-IS SR tunnel index 20
                    via 20.30.31.30, Ethernet1, label 20202
 20072   A[1]
                via M, ::, swap 20072
                    EgressACL: bypass
                  via IS-IS SR tunnel index 20
                    via 20.30.31.30, Ethernet1, label 20202
 20084   A[1]
                via M, ::, swap 20084
                    EgressACL: bypass
                  via IS-IS SR tunnel index 20
                    via 20.30.31.30, Ethernet1, label 20202
 20120   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.31.30 Ethernet1
 20122   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.31.30 Ethernet1
 20128   A[1]
                via M, ::, swap 20128
                    EgressACL: bypass
                  via IS-IS SR tunnel index 20
                    via 20.30.31.30, Ethernet1, label 20202
 20175   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.31.30 Ethernet1
 20179   A[1]
                via M, ::, swap 20179
                    EgressACL: bypass
                  via IS-IS SR tunnel index 20
                    via 20.30.31.30, Ethernet1, label 20202
 20184   A[1]
                via M, ::, swap 20184
                    EgressACL: bypass
                  via IS-IS SR tunnel index 20
                    via 20.30.31.30, Ethernet1, label 20202
 20202   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.31.30 Ethernet1
 20214   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.31.30 Ethernet1
 20216   A[1]
                via M, ::, swap 20216
                    EgressACL: bypass
                  via IS-IS SR tunnel index 20
                    via 20.30.31.30, Ethernet1, label 20202
 20430   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::c6ca:2bff:fe45:a215 Ethernet1
 362144   [0]
                via I, ipv6, vrf RED
 362145   [0]
                via I, ipv4, vrf RED
 394917  A[1]
                via M, 20.30.31.30, pop
                    EgressACL: apply
                    directly connected, Ethernet1
                    c4:ca:2b:45:a2:15, vlan 1006
 394918  A[1]
                via M, fe80::c6ca:2bff:fe45:a215, pop
                    EgressACL: apply
                    directly connected, Ethernet1
                    c4:ca:2b:45:a2:15, vlan 1006
```

## show mpls lfib route

```text
MPLS forwarding table (Label [metric] Vias) - 20 routes 
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

 IP    20030    [1], 10.0.0.30/32
                via M, 20.30.31.30, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    20032    [1], 10.0.0.32/32
                via M, 20.30.31.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 BL    20053    [1], 10.0.0.53/32
                via IS-IS SR tunnel index 20, swap 20053
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.31.30, Ethernet1, label 20202
 BL    20066    [1], 10.0.0.66/32
                via IS-IS SR tunnel index 20, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.31.30, Ethernet1, label 20202
 I>BL  20072    [1], 10.0.0.72/32
                via IS-IS SR tunnel index 20, swap 20072
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.31.30, Ethernet1, label 20202
 I>BL  20084    [1], 10.0.0.84/32
                via IS-IS SR tunnel index 20, swap 20084
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.31.30, Ethernet1, label 20202
 IP    20120    [1], 10.0.0.120/32
                via M, 20.30.31.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    20122    [1], 10.0.0.122/32
                via M, 20.30.31.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 BL    20128    [1], 10.0.0.128/32
                via IS-IS SR tunnel index 20, swap 20128
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.31.30, Ethernet1, label 20202
 IP    20175    [1], 10.0.0.175/32
                via M, 20.30.31.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 BL    20179    [1], 10.0.0.179/32
                via IS-IS SR tunnel index 20, swap 20179
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.31.30, Ethernet1, label 20202
 BL    20184    [1], 10.0.0.184/32
                via IS-IS SR tunnel index 20, swap 20184
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.31.30, Ethernet1, label 20202
 IP    20202    [1], 209.209.209.202/32
                via M, 20.30.31.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    20214    [1], 10.0.0.214/32
                via M, 20.30.31.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 BL    20216    [1], 10.0.0.216/32
                via IS-IS SR tunnel index 20, swap 20216
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.31.30, Ethernet1, label 20202
 IP    20430    [1], 2002::30/128
                via M, fe80::c6ca:2bff:fe45:a215, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 B3    362144   [0]
                via I, ipv6, vrf RED
 B3    362145   [0]
                via I, ipv4, vrf RED
 IA    394917   [1]
                via M, 20.30.31.30, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
 IA    394918   [1]
                via M, fe80::c6ca:2bff:fe45:a215, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
```

## show bgp evpn

```text
BGP routing table information for VRF default
Router identifier 10.0.0.31, local AS number 64512
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
```

## show bgp vpn-ipv4

```text
BGP routing table information for VRF default
Router identifier 10.0.0.31, local AS number 64512
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 10.0.0.31:5001 IPv4 prefix 10.0.0.31/32
                                 -                     -       -       0       i
 * >      RD: 10.0.0.31:5001 IPv4 prefix 50.10.31.0/24
                                 -                     -       -       0       i
 * >      RD: 53:5001 IPv4 prefix 50.10.53.0/24
                                 10.0.0.53             -       100     0       65000 ?
 * >      RD: 72:5001 IPv4 prefix 50.10.72.0/24
                                 10.0.0.72             -       100     0       ? Or-ID: 10.0.0.72 C-LST: 10.0.0.30 
 * >      RD: 84:5001 IPv4 prefix 50.10.84.0/24
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.30 
 * >      RD: 122:5001 IPv4 prefix 50.10.122.0/24
                                 10.0.0.122            0       100     0       ? Or-ID: 10.0.0.122 C-LST: 10.0.0.30 
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
Router identifier 10.0.0.31, local AS number 64512
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 10.0.0.31:5001 IPv6 prefix 2600:50:10:31::/64
                                 -                     -       -       0       i
```

## show bgp ipv4 labeled-unicast

```text
BGP routing table information for VRF default
Router identifier 10.0.0.31, local AS number 64512
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
 * >  L   10.0.0.31/32           -                     -       -          -       0       i
 *    L   10.0.0.31/32           10.0.0.120            85      -          100     0       ?
 * >  L   10.0.0.53/32           209.209.209.202       110     -          100     0       i
 *    L   10.0.0.53/32           209.209.209.202       0       -          100     0       ? Or-ID: 10.0.0.53 C-LST: 32.32.32.201 
 *    L   10.0.0.53/32           209.209.209.202       0       -          100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.66 
 * >  L   10.0.0.66/32           209.209.209.202       0       -          100     0       i
 * >  L   10.0.0.72/32           209.209.209.202       0       -          100     0       i Or-ID: 10.0.0.72 C-LST: 32.32.32.201 
 *    L   10.0.0.72/32           10.0.0.120            120     -          100     0       ?
 * >  L   10.0.0.84/32           209.209.209.202       0       -          100     0       i Or-ID: 10.0.0.84 C-LST: 32.32.32.201 
 * >EcL   10.0.0.128/32          209.209.209.202       0       -          100     0       i Or-ID: 10.0.0.128 C-LST: 32.32.32.201 
 *  ecL   10.0.0.128/32          209.209.209.202       0       -          100     0       i Or-ID: 10.0.0.128 C-LST: 10.0.0.66 
 *    L   10.0.0.128/32          10.0.0.120            110     -          100     0       ?
 *    L   10.0.0.128/32          209.209.209.202       110     -          100     0       i
 * >  L   10.0.0.179/32          209.209.209.202       0       -          125     0       i Or-ID: 10.0.0.179 C-LST: 32.32.32.201 
 *    L   10.0.0.179/32          10.0.0.120            110     -          100     0       ?
 *    L   10.0.0.179/32          209.209.209.202       110     -          100     0       i
 *    L   10.0.0.179/32          209.209.209.202       0       -          100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.66 
 * >  L   10.0.0.184/32          209.209.209.202       120     -          100     0       i
 *    L   10.0.0.184/32          10.0.0.120            120     -          100     0       ?
 *    L   10.0.0.184/32          209.209.209.202       0       -          0       0       i Or-ID: 192.0.0.1 C-LST: 10.0.0.66 
 *    L   10.0.0.184/32          209.209.209.202       0       -          0       0       i Or-ID: 192.0.0.1 C-LST: 32.32.32.201 
 * >EcL   10.0.0.216/32          209.209.209.202       0       -          100     0       i Or-ID: 10.0.0.216 C-LST: 32.32.32.201 
 *  ecL   10.0.0.216/32          209.209.209.202       0       -          100     0       i Or-ID: 10.0.0.216 C-LST: 10.0.0.66 
 *    L   10.0.0.216/32          10.0.0.120            110     -          100     0       ?
 *    L   10.0.0.216/32          209.209.209.202       110     -          100     0       i
```

## show bgp neighbors

```text
BGP neighbor is 10.0.0.30, remote AS 65001, internal link
 Description: Arista-Spine30
  BGP version 4, remote router ID 10.0.0.30, VRF default
  Inherits configuration from and member of peer-group OPTION-C-RIGHT-PEER
  Last read 00:00:11, last write 00:00:44
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:49
  Keepalive timer is active, time left: 00:00:06
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:39:07
  Number of transitions to established: 7
  Last state was OpenConfirm
  Last event was ReapplyInboundPolicy
  Last sent notification:Cease/administrative reset, Last time 00:39:08, First time 12:37:35, Repeats 1
  Last rcvd notification:Cease/connection rejected, Last time 16:35:51, First time 16:36:05, Repeats 3
  Last sent socket-error:Connect (Network is unreachable), Last time 18:02:04, First time 9d01h, Repeats 4232
  Types of communities advertised: standard extended large
  Enhanced route refresh stale path removal disabled
  Outbound enhanced route refresh enabled
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised and received and negotiated
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
      VPN-IPv4: received
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: yes
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 00:39:06
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 7
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
    Opens:                          11         7
    Notifications:                   3         7
    Updates:                        27       517
    Keepalives:                   2582      2536
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:               2623      3067
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         2         9              9                   0
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
Local AS is 65001, local router ID 10.0.0.31
TTL is 255
Local TCP address is 10.0.0.31, local port is 179
Remote TCP address is 10.0.0.30, remote port is 37667
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.31
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
    TCP Throughput: 472.82 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.32, remote AS 65001, internal link
 Description: Arista-ASBR-32
  BGP version 4, remote router ID 10.0.0.32, VRF default
  Inherits configuration from and member of peer-group OPTION-C-RIGHT-LU
  Last read 00:00:25, last write 00:00:59
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:35
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:39:07
  Number of transitions to established: 3
  Last state was OpenConfirm
  Last event was RecvKeepAlive
  Last sent notification:Cease/administrative reset, Last time 00:39:08, First time 12:37:35, Repeats 1
  Types of communities advertised: standard extended large
  Enhanced route refresh stale path removal disabled
  Outbound enhanced route refresh enabled
  Neighbor Capabilities:
    Multiprotocol IPv4 with MPLS Labels: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised and received and negotiated
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      IPv4 with MPLS Labels: advertised
    Additional-paths send capability:
      IPv4 with MPLS Labels: received
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: yes
      Graceful notification: yes
      IPv4 with MPLS Labels is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      IPv4 with MPLS Labels is enabled, Forwarding State is not preserved
    Multiple labels capability:
      IPv4 with MPLS Labels: advertised with count 13
      IPv4 with MPLS Labels: received with count 13
  Restart timer is inactive
  End of rib timer is inactive
    IPv4 with MPLS Labels End-of-RIB received: Yes
      Received 00:39:06
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 7
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
    Opens:                           3         3
    Notifications:                   2         0
    Updates:                        14        60
    Keepalives:                   1229      1210
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:               1248      1273
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv4 with MPLS Labels:            1         7              5                   2
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
    IPv4 labeled-unicast NLRIs dropped due to maximum route limit violation: 0
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
  Outbound route map is CHRIS-LP-125
Local AS is 65001, local router ID 10.0.0.31
TTL is 255
Local TCP address is 10.0.0.31, local port is 179
Remote TCP address is 10.0.0.32, remote port is 34073
Local next hop for next hop self:
  IPv4 with MPLS Labels: 10.0.0.31
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
    TCP Throughput: 470.89 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.66, remote AS 65001, internal link
  BGP version 4, remote router ID 10.0.0.66, VRF default
  Inherits configuration from and member of peer-group OPTION-C-RIGHT-LU
  Last read 00:00:13, last write 00:00:35
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:47
  Keepalive timer is active, time left: 00:00:18
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:25:13
  Number of transitions to established: 4
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Cease/administrative reset, Last time 00:39:08
  Last rcvd notification:Cease/other configuration change, Last time 00:25:18, First time 00:51:16, Repeats 1
  Last sent socket-error:Connect (Connection refused), Last time 01:16:42, First time 01:21:24, Repeats 14
  Last rcvd socket-error:Connection reset by peer, Last time 00:25:17, First time 01:13:49, Repeats 4
  Types of communities advertised: standard extended large
  Neighbor Capabilities:
    Multiprotocol IPv4 with MPLS Labels: advertised and received and negotiated
    Four Octet ASN: advertised
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      IPv4 with MPLS Labels: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      IPv4 with MPLS Labels is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 0
      Restart-State bit: no
      Graceful notification: no
      IPv4 with MPLS Labels is enabled, Forwarding State is not preserved
    Multiple labels capability:
      IPv4 with MPLS Labels: advertised with count 13
  Restart timer is inactive
  End of rib timer is inactive
    IPv4 with MPLS Labels End-of-RIB received: Yes
      Received 00:25:11
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 5
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
    Opens:                  9         4
    Notifications:          1         2
    Updates:               16        29
    Keepalives:            85        73
    Route Refresh:          0         0
    Total messages:       111       108
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv4 with MPLS Labels:            1         6              3                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 256000, warning limit is 204800
  Inbound updates dropped by reason:
    AS path loop detection: 5
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 1
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
    IPv4 labeled-unicast NLRIs dropped due to maximum route limit violation: 0
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
Local AS is 65001, local router ID 10.0.0.31
TTL is 255
Local TCP address is 10.0.0.31, local port is 179
Remote TCP address is 10.0.0.66, remote port is 34769
Local next hop for next hop self:
  IPv4 with MPLS Labels: 10.0.0.31
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
    Round-trip Time (rtt/rtvar): 0.5ms/0.2ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 233.13 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.120, remote AS 65001, internal link
  BGP version 4, remote router ID 10.0.0.120, VRF default
  Inherits configuration from and member of peer-group OPTION-C-RIGHT-LU
  Last read 00:00:33, last write 00:00:08
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:27
  Keepalive timer is active, time left: 00:00:48
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:39:06
  Number of transitions to established: 5
  Last state was OpenConfirm
  Last event was ReapplyInboundPolicy
  Last sent notification:Cease/administrative reset, Last time 00:39:08, First time 12:37:35, Repeats 1
  Last sent socket-error:Connect (Connection refused), Last time 00:39:07
  Last rcvd socket-error:Connection reset by peer, Last time 00:39:08, First time 16:19:39, Repeats 13
  Types of communities advertised: standard extended large
  Neighbor Capabilities:
    Multiprotocol IPv4 with MPLS Labels: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised
    Additional-paths recv capability:
      IPv4 with MPLS Labels: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: yes
      Graceful notification: yes
      IPv4 with MPLS Labels is enabled, Forwarding State is not preserved
    Multiple labels capability:
      IPv4 with MPLS Labels: advertised with count 13
  Restart timer is inactive
  End of rib timer is inactive
    IPv4 with MPLS Labels End-of-RIB received: No
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
    Opens:                 16         5
    Notifications:          2         0
    Updates:               12        54
    Keepalives:          1145      1076
    Route Refresh:          0         0
    Total messages:      1175      1135
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv4 with MPLS Labels:            1         6              0                   0
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
    IPv4 labeled-unicast NLRIs dropped due to maximum route limit violation: 0
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
Local AS is 65001, local router ID 10.0.0.31
TTL is 255
Local TCP address is 10.0.0.31, local port is 179
Remote TCP address is 10.0.0.120, remote port is 3800
Local next hop for next hop self:
  IPv4 with MPLS Labels: 10.0.0.31
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
    Round-trip Time (rtt/rtvar): 0.3ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 377.88 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.156, remote AS 65001, internal link
 Description: Juniper_156
  BGP version 4, remote router ID 10.0.0.156, VRF default
  Inherits configuration from and member of peer-group OPTION-C-RIGHT-LU
  Last read 00:02:10, last write 00:00:40
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:46
  Connection interval is 64 seconds
  Failed connection attempts is 6
  Idle-restart timer is inactive
  BGP state is Active
  Peering failure hint: Hold Timer Expired Error/None
  Number of transitions to established: 4
  Last state was Connect
  Last event was TransportError
  Last sent notification:Hold Timer Expired Error/None, Last time 00:00:40
  Last rcvd notification:Cease/peer de-configured, Last time 02:44:13
  Last sent socket-error:Connect (Network is unreachable), Last time 00:00:18, First time 00:00:39, Repeats 5
  Types of communities advertised: standard extended large
  Neighbor Capabilities:
    Multiprotocol IPv4 with MPLS Labels: advertised and received
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received
    Additional-paths recv capability:
      IPv4 with MPLS Labels: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: yes
      Graceful notification: yes
      IPv4 with MPLS Labels is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
    Long Lived Graceful Restart received:
      Helper only
    Multiple labels capability:
      IPv4 with MPLS Labels: advertised with count 13
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
    Opens:                  4         4
    Notifications:          3         1
    Updates:               16       157
    Keepalives:          2461      2239
    Route Refresh:          0         0
    Total messages:      2484      2401
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
  Outbound route map is CHRIS-LP-150
Local AS is 65001, local router ID 10.0.0.31
TTL is 255
Local TCP address is 10.0.0.31
Remote TCP address is 10.0.0.156, remote port is 179

BGP neighbor is 10.0.0.175, remote AS 64512, internal link
 Description: Juniper_175
  BGP version 4, remote router ID 10.0.0.175, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 8d23h, last write 8d23h
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
  Number of transitions to established: 10
  Last state was Active
  Last event was AdminShutdown
  Last sent notification:Hold Timer Expired Error/None, Last time 8d23h, First time 9d13h, Repeats 9
  Last sent socket-error:Connect (Network is unreachable), Last time 19:54:09, First time 9d13h, Repeats 4163
  Types of communities advertised: standard extended large
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
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
    Opens:                 10        10
    Notifications:         10         0
    Updates:               42       440
    Keepalives:          2704      2419
    Route Refresh:          0         0
    Total messages:      2766      2869
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
Local AS is 64512, local router ID 10.0.0.31
TTL is 255
Remote TCP address is 10.0.0.175

BGP neighbor is 10.0.0.214, remote AS 65001, internal link
  BGP version 4, remote router ID 10.0.0.214, VRF default
  Inherits configuration from and member of peer-group OPTION-C-RIGHT-LU
  Last read 00:00:08, last write 00:00:23
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:22
  Keepalive timer is active, time left: 00:00:01
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:39:08
  Number of transitions to established: 4
  Last state was OpenConfirm
  Last event was RecvRtRefresh
  Last sent notification:Cease/administrative reset, Last time 00:39:08, First time 12:37:35, Repeats 1
  Last rcvd notification:Cease/administrative shutdown, Last time 16:22:12
  Last sent socket-error:Connect (Connection refused), Last time 16:21:57, First time 16:22:11, Repeats 3
  Types of communities advertised: standard extended large
  Neighbor Capabilities:
    Multiprotocol IPv4 with MPLS Labels: advertised and received and negotiated
    Multiprotocol VPN-IPv4: received
    Multiprotocol VPN-IPv6: received
    Multiprotocol L2VPN EVPN: received
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      IPv4 with MPLS Labels: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: yes
      Graceful notification: yes
      IPv4 with MPLS Labels is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 300
      Restart-State bit: no
      Graceful notification: no
    Multiple labels capability:
      IPv4 with MPLS Labels: advertised with count 13
  Restart timer is inactive
  End of rib timer is inactive
    IPv4 with MPLS Labels End-of-RIB received: Yes
      Received 00:39:03
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 7
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
    Opens:                  4         4
    Notifications:          2         1
    Updates:               21       133
    Keepalives:          2449      2091
    Route Refresh:          0         2
    Total messages:      2476      2231
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv4 with MPLS Labels:            1         5              2                   0
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
    IPv4 labeled-unicast NLRIs dropped due to maximum route limit violation: 0
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
Local AS is 65001, local router ID 10.0.0.31
TTL is 255
Local TCP address is 10.0.0.31, local port is 179
Remote TCP address is 10.0.0.214, remote port is 36283
Local next hop for next hop self:
  IPv4 with MPLS Labels: 10.0.0.31
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1012
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.4ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 224.27 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.221, remote AS 65001, internal link
  BGP version 4, remote router ID 10.0.0.221, VRF default
  Inherits configuration from and member of peer-group OPTION-C-RIGHT-LU
  Last read 00:06:11, last write 00:03:11
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:43
  Connection interval is 64 seconds
  Failed connection attempts is 8
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 6
  Last state was Connect
  Last event was TransportError
  Last sent notification:Hold Timer Expired Error/None, Last time 00:03:11
  Last rcvd notification:Cease/administrative shutdown, Last time 01:52:18, First time 15:49:12, Repeats 2
  Last sent socket-error:Connect (Network is unreachable), Last time 00:00:35, First time 00:03:10, Repeats 7
  Last rcvd socket-error:Connection reset by peer, Last time 00:38:41, First time 15:49:11, Repeats 20
  Types of communities advertised: standard extended large
  Neighbor Capabilities:
    Multiprotocol IPv4 with MPLS Labels: advertised and received
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
    Enhanced route refresh: advertised and received
    Send End-of-RIB messages: advertised
    Additional-paths recv capability:
      IPv4 with MPLS Labels: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: yes
      Graceful notification: yes
      IPv4 with MPLS Labels is enabled, Forwarding State is not preserved
    Multiple labels capability:
      IPv4 with MPLS Labels: advertised with count 13
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
    Opens:                 33        12
    Notifications:          9         3
    Updates:               13        69
    Keepalives:          1229      2840
    Route Refresh:          0         0
    Total messages:      1284      2924
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
  Outbound route map is CHRIS-LP-175
Local AS is 65001, local router ID 10.0.0.31
TTL is 255
Local TCP address is 10.0.0.31
Remote TCP address is 10.0.0.221, remote port is 179

```

## show bgp labeled-unicast tunnel

```text
Index  Endpoint       Nexthop/Tunnel Index  Interface  Labels     Contributing 
------ -------------- --------------------- ---------- ---------- -------------
221    10.0.0.216/32  IS-IS SR IPv4 (20)    -          [ 20216 ]  Yes          
228    10.0.0.53/32   IS-IS SR IPv4 (20)    -          [ 20053 ]  Yes          
231    10.0.0.128/32  IS-IS SR IPv4 (20)    -          [ 20128 ]  Yes          
236    10.0.0.179/32  IS-IS SR IPv4 (20)    -          [ 20179 ]  Yes          
239    10.0.0.184/32  IS-IS SR IPv4 (20)    -          [ 20184 ]  Yes          
240    10.0.0.72/32   IS-IS SR IPv4 (20)    -          [ 20072 ]  Yes          
250    10.0.0.66/32   IS-IS SR IPv4 (20)    -          [ 3 ]      Yes          
251    10.0.0.84/32   IS-IS SR IPv4 (20)    -          [ 20084 ]  Yes          

   Metric/Type       Metric 2       Pref    Pref 2
----------------- -------------- ---------- ------
      0 MED          0              200     0     
    110 MED          0              200     0     
      0 MED          0              200     0     
      0 MED          0              200     0     
    120 MED          0              200     0     
      0 MED          0              200     0     
      0 MED          0              200     0     
      0 MED          0              200     0     

```

## show bgp labeled-unicast forwarding

```text
   Index        Nexthop                  Interface    Labels   
------------ ------------------------ --------------- ---------
   194265       IS-IS SR IPv4 (20)       -            [ 20216 ]
   194269       IS-IS SR IPv4 (20)       -            [ 20128 ]
   194272       IS-IS SR IPv4 (20)       -            [ 20216 ]
   207255       IS-IS SR IPv4 (20)       -            [ 20053 ]
   207257       IS-IS SR IPv4 (20)       -            [ 20053 ]
   207258       IS-IS SR IPv4 (20)       -            [ 3 ]    
   207259       IS-IS SR IPv4 (20)       -            [ 3 ]    
   207267       IS-IS SR IPv4 (20)       -            [ 20179 ]
   207268       IS-IS SR IPv4 (20)       -            [ 20179 ]
   207269       IS-IS SR IPv4 (20)       -            [ 20184 ]
   207270       IS-IS SR IPv4 (20)       -            [ 20184 ]
   207271       IS-IS SR IPv4 (20)       -            [ 20128 ]
   207274       IS-IS SR IPv4 (20)       -            [ 20072 ]
   207275       IS-IS SR IPv4 (20)       -            [ 20072 ]
   207276       IS-IS SR IPv4 (20)       -            [ 20084 ]
   207277       IS-IS SR IPv4 (20)       -            [ 20084 ]

```

## show tunnel rib system-tunnel-rib brief

```text
Tunnel RIB: system-tunnel-rib
Endpoint           Tunnel Type    Index(es)  Tunnel Preference  IGP Preference 
------------------ -------------- ---------- ------------------ ---------------
10.0.0.30/32       IS-IS SR IPv4  4          65                 115            
10.0.0.32/32       IS-IS SR IPv4  9          65                 115            
10.0.0.53/32       BGP LU         228        85                 200            
10.0.0.66/32       BGP LU         250        85                 200            
10.0.0.72/32       IS-IS SR IPv4  8          65                 115            
10.0.0.84/32       IS-IS SR IPv4  2          65                 115            
10.0.0.120/32      IS-IS SR IPv4  7          65                 115            
10.0.0.122/32      IS-IS SR IPv4  25         65                 115            
10.0.0.128/32      BGP LU         231        85                 200            
10.0.0.175/32      IS-IS SR IPv4  1          65                 115            
10.0.0.179/32      BGP LU         236        85                 200            
10.0.0.184/32      BGP LU         239        85                 200            
10.0.0.214/32      IS-IS SR IPv4  10         65                 115            
10.0.0.216/32      BGP LU         221        85                 200            
209.209.209.202/32 IS-IS SR IPv4  20         65                 115            
2002::30/128       IS-IS SR IPv6  23         65                 115            

   IGP Metric    Metric Type
---------------- -----------
   10            metric     
   60            metric     
   110           MED        
   0             MED        
   120           metric     
   120           metric     
   110           metric     
   110           metric     
   0             MED        
   110           metric     
   0             MED        
   120           MED        
   110           metric     
   0             MED        
   70            metric     
   20            metric     

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
>C    10.0.0.31/32 [0 pref/0 metric] updated 9d20h ago
         via Loopback0, directly connected
>C    20.30.31.0/24 [0 pref/0 metric] updated 18:02:16 ago
         via Ethernet1, directly connected
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
>P    0.0.0.0/8 [1 pref/0 metric] updated 10d03h ago
         via Null0, directly connected [NF]
>P    127.0.0.0/8 [1 pref/0 metric] updated 10d03h ago
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
>I    10.0.0.30/32 [115 pref/10 metric] updated 18:02:05 ago
         via 20.30.31.30, Ethernet1
>I    10.0.0.32/32 [115 pref/60 metric] updated 00:59:06 ago
         via 20.30.31.30, Ethernet1
>I    10.0.0.66/32 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    10.0.0.72/32 [115 pref/120 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    10.0.0.84/32 [115 pref/120 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    10.0.0.120/32 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    10.0.0.122/32 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    10.0.0.175/32 [115 pref/110 metric] updated 00:01:51 ago
         via 20.30.31.30, Ethernet1
>I    10.0.0.214/32 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    20.30.32.0/24 [115 pref/60 metric] updated 00:59:06 ago
         via 20.30.31.30, Ethernet1
>I    20.30.66.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    20.30.72.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    20.30.84.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    20.30.120.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    20.30.122.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    20.30.214.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    30.122.190.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    101.64.122.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    101.74.122.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    101.88.122.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    101.119.122.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    101.122.125.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    101.122.130.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    101.122.158.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    101.122.162.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    101.122.169.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    101.122.216.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    101.122.218.0/24 [115 pref/110 metric] updated 01:12:24 ago
         via 20.30.31.30, Ethernet1
>I    209.209.209.202/32 [115 pref/70 metric] updated 00:01:51 ago
         via 20.30.31.30, Ethernet1
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
>C    2001:0:30:31::/64 [0 pref/0 metric] updated 18:02:16 ago
         via Ethernet1, directly connected
>C    2002::31/128 [0 pref/0 metric] updated 17:24:40 ago
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
>P    ::/96 [1 pref/0 metric] updated 18:02:16 ago
         via Null0, directly connected [NF]
>P    ::ffff:127.0.0.0/104 [1 pref/0 metric] updated 18:02:16 ago
         via :: [1 pref/1 metric] type ipv6
            via , directly connected
>P    fe80::/10 [1 pref/0 metric] updated 18:02:16 ago
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
>I    2001:0:30:32::/64 [115 pref/20 metric] updated 17:47:12 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:66::/64 [115 pref/20 metric] updated 18:02:05 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:72::/64 [115 pref/20 metric] updated 18:02:05 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:84::/64 [115 pref/20 metric] updated 18:02:05 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:120::/64 [115 pref/20 metric] updated 17:17:52 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:214::/64 [115 pref/20 metric] updated 18:02:05 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2002::30/128 [115 pref/20 metric] updated 18:02:05 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2002::32/128 [115 pref/30 metric] updated 17:44:04 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
```

## show platform sand l3 summary

```text
Number of vrfs: 3

Ipv4:
  Routes:       62  backlog:  0  unprogrammed:  0
  Adjacencies:  61  backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       21  backlog:  0  unprogrammed:  0
  Adjacencies:  61  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       18  backlog:  0  unprogrammed:  0
  Adjacencies:  9   backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4118  ecmp fecs:  0  fec entries:  4118
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  9  ecmp fecs:  0  fec entries:  9
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   62  unprogrammed:   0   
  Routes6:  21  unprogrammed6:  0   
  Backlog:  0 

Jericho2 Lpm:
  TCAM entries used:   4   Percent free:  99  ADS2 entries used:   7  Percent free:  99
  Pivot buckets used:  5   Rows used:     2   Entries Per Bucket:  1  Percent free:  99
  Route buckets used:  17  Rows used:     4   Entries Per Bucket:  4  Percent free:  99

Lem:
  IPv4  Host in Lem:            disabled
  IPv4  Prefix-lengths in Lem:  None    
  IPv6  Host in Lem:            disabled
  IPv6  Prefix-lengths in Lem:  None    
  Number of downloads:        0
  Number of overflow events:  0

Egress Arp rewrite entries in use (in each fap):
  FixedSystem: 2
Egress Arp remote rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Ip tunnel rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Mpls (for outer 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 12
Egress Mpls (for inner 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 9
Egress Sflow rewrite entries in use (in each fap):
  FixedSystem: 0

Egress rewrite chains in backlog: resource-full 0, no-interface 0

Glem entries used per fap :
  FixedSystem: 4114

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  81  allocs:  54139  frees:  54111  shuffles:  0  cmds:  0
  Zombies:     0    purges:    0
  Quarantine:  0/0  shuffles:  0  deletes:  0   
  Preserved FECs: 0
    First FEC preserved: never
    Last FEC preserved: never
  Fec insertion failures:  0
  Level1  Fecs:
    Non-ecmp fecs:            19  ecmp fecs:            4 
    Non-ecmp (Percent free):  99  ecmp (Percent free):  99
  Level2  Fecs:
    Non-ecmp fecs:            12  ecmp fecs:            0  
    Non-ecmp (Percent free):  99  ecmp (Percent free):  100
  Level3  Fecs:
    Non-ecmp fecs:            0    ecmp fecs:            0  
    Non-ecmp (Percent free):  100  ecmp (Percent free):  100

Lpm Detail:
  Requests:  4183  cleanses:  1207  batches:  1207  avg batch size:  3

Jericho Arp:
  ArpTable writes:      413724  queued      0   
  IngressTable writes:  207140  queued      0   
  Coprocessors:         1       in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  16   
  Number of uncountable MPLS tunnels:      16   
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
|0  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |288360|   -   
|0  |10.0.0.30/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |10.0.0.31/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |10.0.0.32/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |10.0.0.66/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |10.0.0.72/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |10.0.0.84/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |10.0.0.120/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |10.0.0.122/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |10.0.0.175/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |10.0.0.214/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |20.30.31.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.30.31.30/32    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288363|   -   
|0  |20.30.31.31/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |20.30.31.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.30.31.0/24     |TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |  -  |525301|   -   
|0  |20.30.32.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |20.30.66.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |20.30.72.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |20.30.84.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |20.30.120.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |20.30.122.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |20.30.214.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |30.122.190.0/24   |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |101.64.122.0/24   |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |101.74.122.0/24   |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |101.88.122.0/24   |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |101.119.122.0/24  |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |101.122.125.0/24  |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |101.122.130.0/24  |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |101.122.158.0/24  |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |101.122.162.0/24  |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |101.122.169.0/24  |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |101.122.216.0/24  |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |101.122.218.0/24  |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|0  |209.209.209.202/32|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288366|   -   
|0  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |524293|   -   
|1  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |288361|   -   
|1  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|1  |192.168.20.0/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|1  |192.168.20.31/32  |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|1  |192.168.21.255/32 |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|1  |192.168.20.0/23   |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|1  |0.0.0.0/0         |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|2  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |288365|   -   
|2  |10.0.0.31/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|2  |50.10.31.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|2  |50.10.31.1/32     |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|2  |50.10.31.2/32     |ROUTE| Et40               |1008 |107518  | 00:14:01:00:00:01 |  -  |288370|   -   
|2  |50.10.31.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|2  |50.10.31.0/24     |TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |  -  |525303|   -   
|2  |50.10.53.0/24     |ROUTE| FEC 288369         |0    |2097133 | 00:00:00:00:00:00 |  -  |91774 |M 20202 20053 970002
|2  |50.10.72.0/24     |ROUTE| FEC 288369         |0    |2097142 | 00:00:00:00:00:00 |  -  |91811 |M 20072 62000
|2  |50.10.84.0/24     |ROUTE| FEC 288369         |0    |2097136 | 00:00:00:00:00:00 |  -  |91814 |M 20084 720896
|2  |50.10.122.0/24    |ROUTE| FEC 288369         |0    |2097149 | 00:00:00:00:00:00 |  -  |91760 |M 20122 1279
|2  |50.10.128.0/24    |ROUTE| FEC 288369         |0    |2097151 | 00:00:00:00:00:00 |  -  |91758 |M 20202 20128 48080
|2  |50.10.179.0/24    |ROUTE| FEC 288369         |0    |2097137 | 00:00:00:00:00:00 |  -  |91813 |M 20202 20179 16
|2  |50.10.184.0/24    |ROUTE| FEC 288369         |0    |2097141 | 00:00:00:00:00:00 |  -  |91759 |M 20202 20184 16
|2  |50.10.216.0/24    |ROUTE| FEC 288369         |0    |2097132 | 00:00:00:00:00:00 |  -  |91799 |M 20202 20216 1048571
|2  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|2  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |524293|   -   

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
|11   |91785 |ROUTE| FEC 288369         |   - |2097150 |                 - |Mswap 20202 20179
|12   |91772 |ROUTE| FEC 288369         |   - |2097145 |                 - |Mswap 20202 20128
|13   |91825 |ROUTE| FEC 288369         |   - |2097144 |                 - |Mswap 20202 20216
|  -  |91752 |ROUTE| FEC 288369         |   - |2097148 |                 - |Mswap 20202 20072
|  -  |91753 |ROUTE| FEC 288369         |   - |2097147 |                 - |Mswap 20202 20084
|  -  |91754 |ROUTE| FEC 288369         |   - |2097143 |                 - |Mpush 20202
|  -  |91757 |ROUTE| FEC 288369         |   - |2096990 |                 - |Mswap 20202 20053
|  -  |91758 |ROUTE| FEC 288369         |   - |2097151 |                 - |Mpush 20202 20128 48080
|  -  |91759 |ROUTE| FEC 288369         |   - |2097141 |                 - |Mpush 20202 20184 16
|  -  |91760 |ROUTE| FEC 288369         |   - |2097149 |                 - |Mpush 20122 1279
|  -  |91774 |ROUTE| FEC 288369         |   - |2097133 |                 - |Mpush 20202 20053 970002
|  -  |91799 |ROUTE| FEC 288369         |   - |2097132 |                 - |Mpush 20202 20216 1048571
|  -  |91811 |ROUTE| FEC 288369         |   - |2097142 |                 - |Mpush 20072 62000
|  -  |91812 |ROUTE| FEC 288369         |   - |2097140 |                 - |Mswap 20202 20184
|  -  |91813 |ROUTE| FEC 288369         |   - |2097137 |                 - |Mpush 20202 20179 16
|  -  |91814 |ROUTE| FEC 288369         |   - |2097136 |                 - |Mpush 20084 720896
|  -  |288360|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288361|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288362|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288363|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288364|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288365|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288366|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288367|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288368|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288369|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288370|ROUTE| Et40               |1008 |107518  | 00:14:01:00:00:01 |   -   
|  -  |288371|DROP | DROP               |0    |  -     |                   |   -   
|  -  |524290|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |524291|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |524293|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |524295|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |525301|TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |   -   
|  -  |525303|TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |   -   
|  -  |525304|TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |   -   

```

## show interfaces counters queue | nz

```text
Aggregate VoQ Counters
Egress                     Traffic               Pkts             Octets           DropPkts         DropOctets
Port                       Class  
--------------------------------------------------------------------------------------------------------------
Et1                        TC1              516408465        38693672390                  0                  0
Et1                        TC6                   3377             277694                  0                  0
Et1                        TC7                 140121           28025630                  0                  0
Et5                        TC1             1648163461       125638274699                  0                  0
Et5                        TC6                   7910             799865                  0                  0
Et5                        TC7                  56394           10792382                  0                  0
Et40                       TC1             2314962035       178652170856                  0                  0
Et40                       TC6                      5                430                  0                  0
Et40                       TC7                1335210          194291299                  0                  0
OlpFap0                    TC7                    184              12512                  0                  0

Egress Queue Counters
Port                 Traffic DropPrec   DestType          OutEnqPkts      OutEnqOctets       OutDropPkts     OutDropOctets
                     Class
Et1                  TC1     DP0-3      UC                 516408832       38693706762                 0                 0
Et1                  TC6     DP0-3      UC                      3377            277584                 0                 0
Et1                  TC7     DP0-3      UC                    140120          27398667                 4               447
Et5                  TC1     DP0-3      UC                1648163461      125638266191                 0                 0
Et5                  TC6     DP0-3      UC                      7910            799751                 0                 0
Et5                  TC7     DP0-3      UC                     56392          10521019                 2               128
Et40                 TC1     DP0-3      UC                2314961803      178652148584                 0                 0
Et40                 TC6     DP0-3      UC                         5               430                 0                 0
Et40                 TC7     DP0-3      UC                   1335210         184950965                 0                 0
OlpFap0              TC3,7   DP0-3      UC                       184             11224                 0                 0

```

## show sync-e esmc detail

```text
! Agent 'Synce' is not enabled
```

## show sync-e selection

```text
! Agent 'Synce' is not enabled
```

## show ptp

```text
PTP is not configured
```

## show ptp interface

```text
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
Et1                        TC1              516408465        38693672390                  0                  0
Et1                        TC6                   3377             277694                  0                  0
Et1                        TC7                 140121           28025630                  0                  0
Et5                        TC1             1648163461       125638274699                  0                  0
Et5                        TC6                   7910             799865                  0                  0
Et5                        TC7                  56394           10792382                  0                  0
Et40                       TC1             2314962035       178652170856                  0                  0
Et40                       TC6                      5                430                  0                  0
Et40                       TC7                1335210          194291299                  0                  0
OlpFap0                    TC7                    184              12512                  0                  0

Egress Queue Counters
Port                 Traffic DropPrec   DestType          OutEnqPkts      OutEnqOctets       OutDropPkts     OutDropOctets
                     Class
Et1                  TC1     DP0-3      UC                 516408832       38693706762                 0                 0
Et1                  TC6     DP0-3      UC                      3377            277584                 0                 0
Et1                  TC7     DP0-3      UC                    140120          27398667                 4               447
Et5                  TC1     DP0-3      UC                1648163461      125638266191                 0                 0
Et5                  TC6     DP0-3      UC                      7910            799751                 0                 0
Et5                  TC7     DP0-3      UC                     56392          10521019                 2               128
Et40                 TC1     DP0-3      UC                2314961803      178652148584                 0                 0
Et40                 TC6     DP0-3      UC                         5               430                 0                 0
Et40                 TC7     DP0-3      UC                   1335210         184950965                 0                 0
OlpFap0              TC3,7   DP0-3      UC                       184             11224                 0                 0

```

