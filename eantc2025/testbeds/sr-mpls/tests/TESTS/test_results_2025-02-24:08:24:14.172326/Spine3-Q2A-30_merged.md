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

Uptime: 3 days, 17 hours and 46 minutes
Total memory: 8099700 kB
Free memory: 5002552 kB

```

## show interfaces counters rates | nz

```text
Port      Name                 Intvl  In Mbps      %  In Kpps Out Mbps      %
Et9       Ciena-5134-72 port 2  0:01      0.0   0.0%        0      0.0   0.0%
Et11      Juniper-156 port 590  0:01      0.0   0.0%        0      0.0   0.0%
Et21      Juniper-156 port 592  0:01      0.0   0.0%        0      0.0   0.0%
Et31      Ciena-8140-66 port 2  0:01      0.0   0.0%        0      0.0   0.0%
Et35      Juniper-131-JCNR 42   0:01      0.0   0.0%        0      0.0   0.0%

Port      Out Kpps
```

## show ip interface brief | exclude una

```text
                                                                        Address
Interface       IP Address          Status        Protocol        MTU   Owner  
--------------- ------------------- ------------- ----------- --------- -------
Ethernet1       20.30.31.30/24      down          down           1500          
Ethernet2       20.30.32.30/24      up            up             1500          
Ethernet3       20.30.120.30/24     up            up             1500          
Ethernet4       20.30.217.30/24     up            up             1500          
Ethernet5       20.30.214.30/24     up            up             1500          
Ethernet6       21.30.214.30/24     down          down           1500          
Ethernet7       20.30.184.30/24     up            up             1500          
Ethernet8       21.30.217.30/24     up            up             1500          
Ethernet9       20.30.72.30/24      up            up             1500          
Ethernet10      21.30.120.30/24     down          down           1500          
Ethernet11      20.30.156.30/24     up            up             1500          
Ethernet12      20.30.84.30/24      up            up             1500          
Ethernet13      20.30.53.30/24      down          down           1500          
Ethernet15      20.30.221.30/24     up            up             1500          
Ethernet16      21.30.84.30/24      admin down    down           1500          
Ethernet17      20.30.124.30/24     up            up             1500          
Ethernet18      21.30.124.30/24     up            up             1500          
Ethernet19      20.30.128.30/24     up            up             1500          
Ethernet20      21.30.128.30/24     up            up             1500          
Ethernet21      21.30.156.30/24     up            up             1500          
Ethernet29      21.30.32.30/24      down          down           1500          
Ethernet31      20.30.66.30/24      up            up             1500          
Ethernet35      20.30.131.30/24     up            up             1500          
Ethernet40      20.30.179.30/24     up            up             1500          
Loopback0       10.0.0.30/32        up            up            65535          
Loopback5001    10.0.0.30/32        up            up            65535          
Loopback5128    10.128.0.30/32      up            up            65535          
Management1     192.168.20.30/23    up            up             1500          

```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
IGP       default  Arista-PE32-Q2C-32 L2   Ethernet2          P2P               UP    21          44                  
IGP       default  Ciena-8140-66    L2   Ethernet31         P2P               UP    23          02                  
IGP       default  Ciena-5134-72    L2   Ethernet9          P2P               UP    30          02                  
IGP       default  Ericsson_84_R6678 L2   Ethernet12         P2P               UP    24          02                  
IGP       default  H3C_M1A_120      L2   Ethernet3          P2P               UP    29          01                  
IGP       default  0000.0000.0124   L2   Ethernet18         P2P               UP    30          0A                  
IGP       default  0000.0000.0124   L2   Ethernet17         P2P               UP    29          09                  
IGP       default  0000.0000.0128   L2   Ethernet20         P2P               UP    28          0E                  
IGP       default  0000.0000.0128   L2   Ethernet19         P2P               UP    30          09                  
IGP       default  Juniper-131-JCNR L2   Ethernet35         P2P               UP    19          01                  
IGP       default  Juniper-156-PTX10002-36QDD L2   Ethernet11         P2P               UP    26          01                  
IGP       default  Juniper-156-PTX10002-36QDD L2   Ethernet21         P2P               UP    25          01                  
IGP       default  Juniper-179-ACX7024 L2   Ethernet40         P2P               UP    27          01                  
IGP       default  Nokia-SXR-214    L2   Ethernet5          P2P               UP    23          00                  
IGP       default  Nokia-SR1-217    L2   Ethernet4          P2P               UP    24          00                  
IGP       default  221              L2   Ethernet15         P2P               UP    90          00                  
```

## show isis database detail

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00      1527   2347   843   1092 L2  0000.0000.0030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 543 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-Spine3-Q2A-30
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.30.128.30
      Interface address: 20.30.214.30
      Interface address: 20.30.120.30
      Interface address: 20.30.72.30
      Interface address: 20.30.84.30
      Interface address: 20.30.66.30
      Interface address: 20.30.221.30
      Interface address: 20.30.124.30
      Interface address: 20.30.32.30
      Interface address: 20.30.217.30
      Interface address: 21.30.124.30
      Interface address: 21.30.128.30
      Interface address: 21.30.156.30
      Interface address: 20.30.156.30
      Interface address: 20.30.179.30
      Interface address: 21.30.217.30
      Interface address: 20.30.184.30
      Interface address: 20.30.131.30
      Interface address: 10.0.0.30
      Interface address: 2001:0:30:128::30
      Interface address: 2001:0:30:214::30
      Interface address: 2001:0:30:120::30
      Interface address: 2001:0:30:72::30
      Interface address: 2001:0:30:84::30
      Interface address: 2001:0:30:66::30
      Interface address: 2001:0:30:221::30
      Interface address: 2001:0:30:124::30
      Interface address: 2001:0:30:32::30
      Interface address: 2001:0:30:217::30
      Interface address: 2001:0:30:156::30
      Interface address: 2001:0:30:179::30
      Interface address: 2001:0:30:184::30
      Interface address: 2001:0:30:131::30
      Interface address: 2002::30
      IS Neighbor          : 221.00              Metric: 1
        IPv4 Neighbor Address: 20.30.221.221
        IPv4 Interface Address: 20.30.221.30
        Adj-sid: 378542 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 1
        IPv4 Neighbor Address: 20.30.32.32
        IPv4 Interface Address: 20.30.32.30
        Adj-sid: 378588 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SR1-217.00    Metric: 1
        IPv4 Neighbor Address: 20.30.217.217
        IPv4 Interface Address: 20.30.217.30
        Adj-sid: 378582 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 1
        IPv4 Neighbor Address: 20.30.214.214
        IPv4 Interface Address: 20.30.214.30
        Adj-sid: 378553 flags: [L V] weight: 0x0
      IS Neighbor          : H3C_M1A_120.00      Metric: 1
        IPv4 Neighbor Address: 20.30.120.120
        IPv4 Interface Address: 20.30.120.30
        Adj-sid: 378597 flags: [L V] weight: 0x0
      Reachability         : 20.30.128.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.214.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.120.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.84.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.66.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.221.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.124.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.32.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.217.0/24 Metric: 1 Type: 1 Up
      Reachability         : 21.30.124.0/24 Metric: 1 Type: 1 Up
      Reachability         : 21.30.128.0/24 Metric: 1 Type: 1 Up
      Reachability         : 21.30.156.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.156.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.179.0/24 Metric: 1 Type: 1 Up
      Reachability         : 21.30.217.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.184.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.131.0/24 Metric: 1 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:72::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:66::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:221::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:32::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:156::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:179::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:131::/64 Metric: 10 Type: 1 Up
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
    Arista-Spine3-Q2A-30.00-01       909   7244   979   1086 L2  0000.0000.0030.00-01  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 679 s
      IS Neighbor          : Ciena-5134-72.00    Metric: 1
        IPv4 Neighbor Address: 20.30.72.72
        IPv4 Interface Address: 20.30.72.30
        Adj-sid: 378577 flags: [L V] weight: 0x0
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 1
        IPv4 Neighbor Address: 20.30.84.84
        IPv4 Interface Address: 20.30.84.30
        Adj-sid: 378586 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-8140-66.00    Metric: 1
        IPv4 Neighbor Address: 20.30.66.66
        IPv4 Interface Address: 20.30.66.30
        Adj-sid: 378578 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0124.00   Metric: 1
        IPv4 Neighbor Address: 20.30.124.124
        IPv4 Interface Address: 20.30.124.30
      IS Neighbor          : 0000.0000.0128.00   Metric: 1
        IPv4 Neighbor Address: 20.30.128.128
        IPv4 Interface Address: 20.30.128.30
      IS Neighbor          : 0000.0000.0124.00   Metric: 1
        IPv4 Neighbor Address: 21.30.124.124
        IPv4 Interface Address: 21.30.124.30
      IS Neighbor          : 0000.0000.0128.00   Metric: 1
        IPv4 Neighbor Address: 21.30.128.128
        IPv4 Interface Address: 21.30.128.30
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 1
        IPv4 Neighbor Address: 20.30.156.156
        IPv4 Interface Address: 20.30.156.30
        Adj-sid: 378540 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 1
        IPv4 Neighbor Address: 21.30.156.156
        IPv4 Interface Address: 21.30.156.30
        Adj-sid: 378574 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 1
        IPv4 Neighbor Address: 20.30.179.179
        IPv4 Interface Address: 20.30.179.30
        Adj-sid: 378538 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-131-JCNR.00 Metric: 1
        IPv4 Neighbor Address: 20.30.131.131
        IPv4 Interface Address: 20.30.131.30
        Adj-sid: 378533 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-PE32-Q2C-32.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:32::32
        Global IPv6 Interface Address: 2001:0:30:32::30
        Adj-sid: 378589 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:156::156
        Global IPv6 Interface Address: 2001:0:30:156::30
        Adj-sid: 378541 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Nokia-SR1-217.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:30:217::217
        Global IPv6 Interface Address: 2001:0:30:217::30
        Adj-sid: 378583 flags: [L V F] weight: 0x0
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
        SR Prefix-SID: 158 Flags: [N] Algorithm: 128
        SR Prefix-SID: 159 Flags: [N] Algorithm: 129
        SR Prefix-SID: 160 Flags: [N] Algorithm: 130
      Reachability (MT-IPv6): 2001:0:30:128::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:124::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::30/128 Metric: 10 Type: 1 Up
        SR Prefix-SID: 430 Flags: [N] Algorithm: 0
        SR Prefix-SID: 558 Flags: [N] Algorithm: 128
        SR Prefix-SID: 559 Flags: [N] Algorithm: 129
        SR Prefix-SID: 560 Flags: [N] Algorithm: 130
    Arista-Spine3-Q2A-30.00-02       326  59861   667    203 L2  0000.0000.0030.00-02  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 367 s
      IS Neighbor (MT-IPv6): H3C_M1A_120.00      Metric: 10
        IPv6 Neighbor Address: 2001:0:30:120::120
        Global IPv6 Interface Address: 2001:0:30:120::30
        Adj-sid: 378598 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Ericsson_84_R6678.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:84::175
        Global IPv6 Interface Address: 2001:0:30:84::30
        Adj-sid: 378587 flags: [L V F] weight: 0x0
    Arista-PE32-Q2C-32.00-00       780  32665   851    592 L2  0000.0000.0032.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE32-Q2C-32
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.30.32.32
      Interface address: 20.32.175.32
      Interface address: 10.0.0.32
      Interface address: 2001:0:30:32::32
      Interface address: 2001:0:32:175::32
      Interface address: 2002::32
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.32.30
        IPv4 Interface Address: 20.30.32.32
        Adj-sid: 362168 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.32.175.175
        IPv4 Interface Address: 20.32.175.32
        Adj-sid: 362170 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:32::30
        Global IPv6 Interface Address: 2001:0:30:32::32
        Adj-sid: 362169 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:32:175::175
        Global IPv6 Interface Address: 2001:0:32:175::32
        Adj-sid: 362171 flags: [L V F] weight: 0x0
      Reachability         : 20.30.32.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.32.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.32/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 32 Flags: [N] Algorithm: 0
        SR Prefix-SID: 161 Flags: [N] Algorithm: 128
        SR Prefix-SID: 162 Flags: [N] Algorithm: 129
        SR Prefix-SID: 163 Flags: [N] Algorithm: 130
      Reachability (MT-IPv6): 2001:0:30:32::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:32:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::32/128 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.32 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
    Arrcus-53.00-00            1221  34308   844    444 L2  0000.0000.0053.00-00  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arrcus-53
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.53
      Interface address: 2002::53
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.53.175.175
        IPv4 Interface Address: 20.53.175.53
        Global IPv6 Interface Address: 2001:0:53:175::53
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Interface Address: 20.53.175.53
        Global IPv6 Interface Address: 2001:0:53:175::53
      Reachability         : 20.53.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.53/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 53 Flags: [N P E] Algorithm: 0
        SR Prefix-SID: 1181 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1182 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1183 Flags: [N] Algorithm: 130
      Reachability (MT-IPv6): 2001:0:53:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::53/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 453 Flags: [N P E] Algorithm: 0
        SR Prefix-SID: 1581 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1582 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1583 Flags: [N] Algorithm: 130
      Router Capabilities: Router Id: 10.0.0.53 Flags: []
        SR Local Block:
          SRLB Base: 16000 Range: 3001
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 780001
        Algorithms:  0, 128, 129, 130
    Ciena-8140-66.00-00         314  39033   310    336 L2  0000.0000.0066.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-8140-66
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.66
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.66.175.175
        IPv4 Interface Address: 20.66.175.66
        Adj-sid: 16004 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.66.30
        IPv4 Interface Address: 20.30.66.66
        Adj-sid: 16005 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.66/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 66 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1195 Flags: [N] Algorithm: 129
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.175.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.66 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ciena-5134-72.00-00         315  30789   353    336 L2  0000.0000.0072.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-5134-72
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.72
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.72.30
        IPv4 Interface Address: 20.30.72.72
        Adj-sid: 16001 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.72.175.175
        IPv4 Interface Address: 20.72.175.72
        Adj-sid: 16000 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.72/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 72 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1201 Flags: [N] Algorithm: 129
      Reachability         : 20.72.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.72 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ericsson_84_R6678.00-00       828  16588  1050    324 L2  0000.0000.0084.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Ericsson_84_R6678
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.84
      Interface address: 2001:0:30:84::175
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 30
        IPv4 Interface Address: 20.84.175.84
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Interface Address: 20.30.84.84
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:84:175::175
        Global IPv6 Interface Address: 2001:0:84:175::175
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:84::30
        Global IPv6 Interface Address: 2001:0:30:84::175
      Reachability         : 10.0.0.84/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 84 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:84:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.84 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    H3C_M1A_120.00-00          4124  14887   844   1436 L2  0000.0000.0120.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: H3C_M1A_120
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.120
      Interface address: 20.30.120.120
      Interface address: 20.120.175.120
      Interface address: 20.120.214.120
      Interface address: 2001:0:30:120::120
      Interface address: 2001:0:120:175::120
      Interface address: 2001:0:120:214::120
      Interface address: 2002::120
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.120.30
        IPv4 Interface Address: 20.30.120.120
        Adj-sid: 1150 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.120.30
        IPv4 Interface Address: 20.30.120.120
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.120.175.175
        IPv4 Interface Address: 20.120.175.120
        Adj-sid: 1151 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.120.175.175
        IPv4 Interface Address: 20.120.175.120
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:120::30
        Global IPv6 Interface Address: 2001:0:30:120::120
        Adj-sid: 1149 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:120::30
        Global IPv6 Interface Address: 2001:0:30:120::120
      Reachability         : 10.0.0.120/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 120 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1248 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1249 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1250 Flags: [N] Algorithm: 130
      Reachability         : 20.30.120.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.217.0/24 Metric: 0 Type: 1 Up
      Reachability         : 192.168.20.0/23 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:217::/64 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2002::120/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 520 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1648 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1649 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1650 Flags: [N] Algorithm: 130
      Router Capabilities: Router Id: 10.0.0.120 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  13
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 128
          Exclude admin groups: 1
          Flags: [M] 0x80
    H3C_M1A_120.00-01           370  31719   842    357 L2  0000.0000.0120.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:120:175::175
        Global IPv6 Interface Address: 2001:0:120:175::120
        Adj-sid: 1148 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:120:175::175
        Global IPv6 Interface Address: 2001:0:120:175::120
    0000.0000.0124.00-00       1866  11642   766    401 L2  0000.0000.0124.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 20.124.175.124
      Interface address: 10.0.0.124
      Interface address: 21.30.124.124
      Interface address: 20.30.124.124
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 15
        IPv4 Neighbor Address: 21.30.124.30
        IPv4 Interface Address: 21.30.124.124
        Adj-sid: 403 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.124.175.175
        IPv4 Interface Address: 20.124.175.124
        Adj-sid: 404 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.124.30
        IPv4 Interface Address: 20.30.124.124
        Adj-sid: 402 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.124/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 124 Flags: [N P] Algorithm: 0
        SR Prefix-SID: 1252 Flags: [N P] Algorithm: 128
      Reachability         : 20.124.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 21.30.124.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.30.124.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.124 Flags: []
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
      Router Capabilities: Router Id: 10.0.0.124 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 2000 Range: 2001
        Algorithms:  0, 128
    0000.0000.0128.00-00       1917  42612   769    401 L2  0000.0000.0128.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.128
      Interface address: 20.128.175.128
      Interface address: 21.30.128.128
      Interface address: 20.30.128.128
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.128.175.175
        IPv4 Interface Address: 20.128.175.128
        Adj-sid: 48134 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 15
        IPv4 Neighbor Address: 21.30.128.30
        IPv4 Interface Address: 21.30.128.128
        Adj-sid: 48136 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.128.30
        IPv4 Interface Address: 20.30.128.128
        Adj-sid: 48137 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.128/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 128 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1256 Flags: [N] Algorithm: 128
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 21.30.128.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.30.128.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128
    Juniper-131-JCNR.00-00       551   5367   630    447 L2  0000.0000.0131.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-131-JCNR
      Area addresses: 49.0001
      Interface address: 10.0.0.131
      Interface address: ::af4:0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.131.175.175
        IPv4 Interface Address: 20.131.175.131
        IPv6 Neighbor Address: 2001:0:131:175::175
        Global IPv6 Interface Address: 2001:0:131:175::131
        Adj-sid: 21 flags: [L V F] weight: 0x0
        Adj-sid: 20 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.131.30
        IPv4 Interface Address: 20.30.131.131
        IPv6 Neighbor Address: 2001:0:30:131::30
        Global IPv6 Interface Address: 2001:0:30:131::131
        Adj-sid: 25 flags: [L V F] weight: 0x0
        Adj-sid: 24 flags: [L V] weight: 0x0
      Reachability         : 20.131.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.131/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 131 Flags: [N] Algorithm: 0
      Reachability         : 20.30.131.0/24 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:131:175::/64 Metric: 10 Type: 1 Up
      Reachability          : fe80::ec97:fbff:fe06:5964/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:30:131::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.131 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    Juniper-156-PTX10002-36QDD.00-00       612  53877  1132   1014 L2  0000.0000.0156.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-156-PTX10002-36QDD
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.156
      Interface address: 2002::156
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.156.30
        IPv4 Interface Address: 20.30.156.156
        IPv6 Neighbor Address: 2001:0:30:156::30
        Global IPv6 Interface Address: 2001:0:30:156::156
        Adj-sid: 22 flags: [L V B] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.156.175.175
        IPv4 Interface Address: 20.156.175.156
        IPv6 Neighbor Address: 2001:0:156:175::175
        Global IPv6 Interface Address: 2001:0:156:175::156
        Adj-sid: 18 flags: [L V B] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 15
        IPv4 Neighbor Address: 21.30.156.30
        IPv4 Interface Address: 21.30.156.156
        Adj-sid: 24 flags: [L V B] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Interface Address: 20.30.156.156
        IPv6 Neighbor Address: 2001:0:30:156::30
        Global IPv6 Interface Address: 2001:0:30:156::156
        Adj-sid: 23 flags: [L V B F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Interface Address: 20.156.175.156
        IPv6 Neighbor Address: 2001:0:156:175::175
        Global IPv6 Interface Address: 2001:0:156:175::156
        Adj-sid: 19 flags: [L V B F] weight: 0x0
      Reachability         : 10.0.0.156/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 156 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1286 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1285 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1284 Flags: [N] Algorithm: 128
      Reachability         : 20.30.156.0/24 Metric: 10 Type: 1 Up
      Reachability         : 21.30.156.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.156.175.0/24 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::156/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 556 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1686 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1685 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1684 Flags: [N] Algorithm: 128
      Reachability (MT-IPv6): 2001:0:156:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:156::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.156 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-00       972  38906   961   1178 L2  0000.0000.0175.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-175-ACX7100-48L
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.175
      Interface address: 127.0.0.1
      Interface address: 2002::175
      IS Neighbor          : Juniper-131-JCNR.00 Metric: 10
        IPv4 Neighbor Address: 20.131.175.131
        IPv4 Interface Address: 20.131.175.175
        IPv6 Neighbor Address: 2001:0:131:175::131
        Global IPv6 Interface Address: 2001:0:131:175::175
        Adj-sid: 116 flags: [L V F] weight: 0x0
        Adj-sid: 115 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 10
        IPv4 Neighbor Address: 20.175.179.179
        IPv4 Interface Address: 20.175.179.175
        IPv6 Neighbor Address: 2001:0:175::179:179
        Global IPv6 Interface Address: 2001:0:175::179:175
        Adj-sid: 106 flags: [L V F] weight: 0x0
        Adj-sid: 105 flags: [L V] weight: 0x0
      IS Neighbor          : H3C_M1A_120.00      Metric: 10
        IPv4 Neighbor Address: 20.120.175.120
        IPv4 Interface Address: 20.120.175.175
        IPv6 Neighbor Address: 2001:0:120:175::120
        Global IPv6 Interface Address: 2001:0:120:175::175
        Adj-sid: 173 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Nokia-SR1-217.00    Metric: 10
        IPv4 Interface Address: 20.175.217.175
        IPv6 Neighbor Address: 2001:0:175:217::217
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 98 flags: [L V F] weight: 0x0
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability         : 10.0.0.175/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 175 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1305 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1304 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1303 Flags: [N] Algorithm: 128
      Reachability         : 20.156.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.72.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.84.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.131.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.32.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.124.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::175/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 575 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1705 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1704 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1703 Flags: [N] Algorithm: 128
      Reachability (MT-IPv6): 2001:0:156:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:84:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:53:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:66:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:72:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:32:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:128:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:221::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.175 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  3
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 0
          Exclude admin groups: 1
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 238
          Flags: [M] 0x80
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 0
          Flags: [M] 0x80
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-01       843  37080  1175   1107 L2  0000.0000.0175.00-01  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 10
        IPv4 Neighbor Address: 20.84.175.84
        IPv4 Interface Address: 20.84.175.175
        IPv6 Neighbor Address: 2001:0:84:175::175
        Global IPv6 Interface Address: 2001:0:84:175::175
        Adj-sid: 132 flags: [L V F] weight: 0x0
        Adj-sid: 131 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 10
        IPv4 Neighbor Address: 20.175.214.214
        IPv4 Interface Address: 20.175.214.175
        IPv6 Neighbor Address: 2001:0:175:214::214
        Global IPv6 Interface Address: 2001:0:175:214::175
        Adj-sid: 151 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.156.175.156
        IPv4 Interface Address: 20.156.175.175
        IPv6 Neighbor Address: 2001:0:156:175::156
        Global IPv6 Interface Address: 2001:0:156:175::175
        Adj-sid: 130 flags: [L V F] weight: 0x0
        Adj-sid: 129 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.175.217.217
        IPv4 Interface Address: 20.175.217.175
        IPv6 Neighbor Address: 2001:0:175:217::217
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 140 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 10
        IPv4 Neighbor Address: 20.32.175.32
        IPv4 Interface Address: 20.32.175.175
        IPv6 Neighbor Address: 2001:0:32:175::32
        Global IPv6 Interface Address: 2001:0:32:175::175
        Adj-sid: 147 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.128.175.128
        IPv4 Interface Address: 20.128.175.175
        Global IPv6 Interface Address: 2001:0:128:175::175
        Adj-sid: 96 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Nokia-SXR-214.00    Metric: 10
        IPv4 Interface Address: 20.175.214.175
        IPv6 Neighbor Address: 2001:0:175:214::214
        Global IPv6 Interface Address: 2001:0:175:214::175
        Adj-sid: 108 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-PE32-Q2C-32.00 Metric: 10
        IPv4 Interface Address: 20.32.175.175
        IPv6 Neighbor Address: 2001:0:32:175::32
        Global IPv6 Interface Address: 2001:0:32:175::175
        Adj-sid: 148 flags: [L V F] weight: 0x0
    Juniper-175-ACX7100-48L.00-02       479  26376  1175   1174 L2  0000.0000.0175.00-02  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      IS Neighbor          : Ciena-5134-72.00    Metric: 10
        IPv4 Neighbor Address: 20.72.175.72
        IPv4 Interface Address: 20.72.175.175
        Global IPv6 Interface Address: 2001:0:72:175::175
        Adj-sid: 167 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.175.53
        IPv4 Interface Address: 20.53.175.175
        IPv6 Neighbor Address: 2001:0:53:175::53
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 99 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0124.00   Metric: 10
        IPv4 Neighbor Address: 20.124.175.124
        IPv4 Interface Address: 20.124.175.175
        Adj-sid: 170 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.66.175.66
        IPv4 Interface Address: 20.66.175.175
        Global IPv6 Interface Address: 2001:0:66:175::175
        Adj-sid: 163 flags: [L V] weight: 0x0
      IS Neighbor          : 221.00              Metric: 10
        IPv4 Neighbor Address: 20.175.221.221
        IPv4 Interface Address: 20.175.221.175
        Global IPv6 Interface Address: 2001:0:175:221::175
        Adj-sid: 171 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Ericsson_84_R6678.00 Metric: 10
        IPv4 Interface Address: 20.84.175.175
        IPv6 Neighbor Address: 2001:0:84:175::175
        Global IPv6 Interface Address: 2001:0:84:175::175
        Adj-sid: 132 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Interface Address: 20.156.175.175
        IPv6 Neighbor Address: 2001:0:156:175::156
        Global IPv6 Interface Address: 2001:0:156:175::175
        Adj-sid: 130 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Arrcus-53.00        Metric: 10
        IPv4 Interface Address: 20.53.175.175
        IPv6 Neighbor Address: 2001:0:53:175::53
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 133 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): H3C_M1A_120.00      Metric: 10
        IPv4 Interface Address: 20.120.175.175
        IPv6 Neighbor Address: 2001:0:120:175::120
        Global IPv6 Interface Address: 2001:0:120:175::175
        Adj-sid: 174 flags: [L V F] weight: 0x0
      Reachability (MT-IPv6): 2001:0:131:175::/64 Metric: 10 Type: 1 Up
    Juniper-179-ACX7024.00-00       720  31209   830    543 L2  0000.0000.0179.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-179-ACX7024
      Area addresses: 49.0001
      Interface address: 10.0.0.179
      Interface address: 127.0.0.1
      Interface address: 10.0.1.179
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.179.175
        IPv4 Interface Address: 20.175.179.179
        IPv6 Neighbor Address: 2001:0:175::179:175
        Global IPv6 Interface Address: 2001:0:175::179:179
        Adj-sid: 20 flags: [L V F] weight: 0x0
        Adj-sid: 19 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 4000
        IPv4 Neighbor Address: 20.30.179.30
        IPv4 Interface Address: 20.30.179.179
        IPv6 Neighbor Address: 2001:0:30:179::30
        Global IPv6 Interface Address: 2001:0:30:179::179
        Adj-sid: 24 flags: [L V F] weight: 0x0
        Adj-sid: 23 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.179/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 179 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1309 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1308 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1307 Flags: [N] Algorithm: 128
      Reachability         : 20.175.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability         : 10.0.1.179/32 Metric: 0 Type: 1 Up
      Reachability         : 20.30.179.0/24 Metric: 4000 Type: 1 Up
      Reachability          : 2001:0:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:179::/64 Metric: 4000 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.179 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    Nokia-SXR-214.00-00       17980  12329   577    620 L2  0000.0000.0214.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SXR-214
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.214
      Interface address: 20.30.214.214
      Interface address: 20.175.214.214
      Interface address: 20.214.216.214
      Interface address: 2000::214
      Interface address: 2001:0:175:214::214
      Interface address: 2001:0:214:216::214
      IS Neighbor          : Nokia-IXRe2-216.00  Metric: 10
        IPv4 Neighbor Address: 20.214.216.216
        IPv4 Interface Address: 20.214.216.214
        Adj-sid: 30031 flags: [L V B] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 100
        IPv4 Neighbor Address: 20.175.214.175
        IPv4 Interface Address: 20.175.214.214
        Adj-sid: 30033 flags: [L V B] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 1
        IPv4 Neighbor Address: 20.30.214.30
        IPv4 Interface Address: 20.30.214.214
        Adj-sid: 30042 flags: [L V B] weight: 0x0
      IS Neighbor (MT-IPv6): Nokia-IXRe2-216.00  Metric: 10
        IPv6 Neighbor Address: 2001:0:214:216::216
        Global IPv6 Interface Address: 2001:0:214:216::214
        Adj-sid: 30032 flags: [L V B F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:175:214::175
        Global IPv6 Interface Address: 2001:0:175:214::214
        Adj-sid: 30034 flags: [L V B F] weight: 0x0
      Reachability         : 20.30.214.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.214.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.214/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 214 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2000::214/128 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:214:216::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.214 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  15
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-IXRe2-216.00-00      1685  26085   660    486 L2  0100.0000.0216.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-IXRe2-216
      Area addresses: 49.0001.0000.0000.0216.00
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.216
      Interface address: 20.214.216.216
      Interface address: 2001:0:214:216::216
      Interface address: 2002::216
      IS Neighbor          : Nokia-SXR-214.00    Metric: 10
        IPv4 Neighbor Address: 20.214.216.214
        IPv4 Interface Address: 20.214.216.216
        IPv6 Neighbor Address: 2001:0:214:216::214
        Global IPv6 Interface Address: 2001:0:214:216::216
        Adj-sid: 1048575 flags: [L V B] weight: 0x0
        Adj-sid: 1048573 flags: [L V B F] weight: 0x0
      IS Neighbor (MT-IPv6): Nokia-SXR-214.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:214:216::214
        Global IPv6 Interface Address: 2001:0:214:216::216
      Reachability         : 20.214.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.216/32 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:214:216::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::216/128 Metric: 0 Type: 1 Up
      Reachability          : 5f00:0:2216::/48 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:214:216::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::216/128 Metric: 0 Type: 1 Up
      SRv6 Locator: 5f00:0:2216::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : 5f00:0:2216::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.0.216 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  11
        SRv6 Capability: Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-SR1-217.00-00        1105  16143   930    594 L2  0100.0000.0217.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SR1-217
      Area addresses: 49.0001.0000.0000.0217.00
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.217
      Interface address: 20.30.217.217
      Interface address: 20.175.217.217
      Interface address: 2001:0:30:217::217
      Interface address: 2001:0:175:217::217
      Interface address: 2002::217
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.217.175
        IPv4 Interface Address: 20.175.217.217
        Adj-sid: 524283 flags: [L V B] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.217.30
        IPv4 Interface Address: 20.30.217.217
        Adj-sid: 524285 flags: [L V B] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
      Reachability         : 10.0.0.217/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 217 Flags: [N P] Algorithm: 0
        SR Prefix-SID: 1345 Flags: [N P] Algorithm: 128
        SR Prefix-SID: 1346 Flags: [N P] Algorithm: 129
        SR Prefix-SID: 1347 Flags: [N P] Algorithm: 130
      Reachability         : 20.30.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.217.0/24 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::217/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.217 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 100
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 100
          Flags: [M] 0x80
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 100
          Exclude admin groups: 1
          Flags: [M] 0x80
    221.00-00                   720  65427   681     85 L2  0221.0221.0221.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Router Capabilities: Router Id: 10.0.0.221 Flags: []
        SR Local Block:
          SRLB Base: 626688 Range: 14336
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 720000 Range: 2000
        Algorithms:  0, 128, 129
      Unsupported TLV: Type: 14 Length: 2
    221.00-01                   652  49185   846     32 L2  0221.0221.0221.00-01  <>
      Hostname: 221
    221.00-02                  9068  40768   846    483 L2  0221.0221.0221.00-02  <>
      Remaining lifetime received: 1197 s Modified to: 1200 s
      Interface address: 10.0.0.221
      Interface address: 20.175.221.221
      Interface address: 20.30.221.221
      Interface address: 1221::1
      Interface address: 2001:0:175:221::221
      Interface address: 2001:0:30:221::221
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.221.175
        IPv4 Interface Address: 20.175.221.221
        Adj-sid: 524296 flags: [L V B] weight: 0x0
        Adj-sid: 524290 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.221.30
        IPv4 Interface Address: 20.30.221.221
        Adj-sid: 524295 flags: [L V B] weight: 0x0
        Adj-sid: 524294 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.221/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 221 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1349 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1350 Flags: [N] Algorithm: 129
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.221.0/24 Metric: 10 Type: 1 Up
      Reachability          : 1221::1/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:175:221::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:221::/64 Metric: 10 Type: 1 Up

```

## show isis database traffic-engineering

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00      1527   2347   843   1092 L2  0000.0000.0030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 543 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-Spine3-Q2A-30
      TE IPv4 router ID: 10.0.0.30
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.30.128.30
      Interface address: 20.30.214.30
      Interface address: 20.30.120.30
      Interface address: 20.30.72.30
      Interface address: 20.30.84.30
      Interface address: 20.30.66.30
      Interface address: 20.30.221.30
      Interface address: 20.30.124.30
      Interface address: 20.30.32.30
      Interface address: 20.30.217.30
      Interface address: 21.30.124.30
      Interface address: 21.30.128.30
      Interface address: 21.30.156.30
      Interface address: 20.30.156.30
      Interface address: 20.30.179.30
      Interface address: 21.30.217.30
      Interface address: 20.30.184.30
      Interface address: 20.30.131.30
      Interface address: 10.0.0.30
      Interface address: 2001:0:30:128::30
      Interface address: 2001:0:30:214::30
      Interface address: 2001:0:30:120::30
      Interface address: 2001:0:30:72::30
      Interface address: 2001:0:30:84::30
      Interface address: 2001:0:30:66::30
      Interface address: 2001:0:30:221::30
      Interface address: 2001:0:30:124::30
      Interface address: 2001:0:30:32::30
      Interface address: 2001:0:30:217::30
      Interface address: 2001:0:30:156::30
      Interface address: 2001:0:30:179::30
      Interface address: 2001:0:30:184::30
      Interface address: 2001:0:30:131::30
      Interface address: 2002::30
      IS Neighbor          : 221.00              Metric: 1
        IPv4 Neighbor Address: 20.30.221.221
        IPv4 Interface Address: 20.30.221.30
        Adj-sid: 378542 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 1
        IPv4 Neighbor Address: 20.30.32.32
        IPv4 Interface Address: 20.30.32.30
        Adj-sid: 378588 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Nokia-SR1-217.00    Metric: 1
        IPv4 Neighbor Address: 20.30.217.217
        IPv4 Interface Address: 20.30.217.30
        Adj-sid: 378582 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Nokia-SXR-214.00    Metric: 1
        IPv4 Neighbor Address: 20.30.214.214
        IPv4 Interface Address: 20.30.214.30
        Adj-sid: 378553 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : H3C_M1A_120.00      Metric: 1
        IPv4 Neighbor Address: 20.30.120.120
        IPv4 Interface Address: 20.30.120.30
        Adj-sid: 378597 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      Reachability         : 20.30.128.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.214.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.120.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.84.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.66.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.221.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.124.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.32.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.217.0/24 Metric: 1 Type: 1 Up
      Reachability         : 21.30.124.0/24 Metric: 1 Type: 1 Up
      Reachability         : 21.30.128.0/24 Metric: 1 Type: 1 Up
      Reachability         : 21.30.156.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.156.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.179.0/24 Metric: 1 Type: 1 Up
      Reachability         : 21.30.217.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.184.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.131.0/24 Metric: 1 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:72::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:66::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:221::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:32::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:156::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:179::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:131::/64 Metric: 10 Type: 1 Up
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
    Arista-Spine3-Q2A-30.00-01       909   7244   979   1086 L2  0000.0000.0030.00-01  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 679 s
      IS Neighbor          : Ciena-5134-72.00    Metric: 1
        IPv4 Neighbor Address: 20.30.72.72
        IPv4 Interface Address: 20.30.72.30
        Adj-sid: 378577 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 1
        IPv4 Neighbor Address: 20.30.84.84
        IPv4 Interface Address: 20.30.84.30
        Adj-sid: 378586 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Ciena-8140-66.00    Metric: 1
        IPv4 Neighbor Address: 20.30.66.66
        IPv4 Interface Address: 20.30.66.30
        Adj-sid: 378578 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : 0000.0000.0124.00   Metric: 1
        IPv4 Neighbor Address: 20.30.124.124
        IPv4 Interface Address: 20.30.124.30
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : 0000.0000.0128.00   Metric: 1
        IPv4 Neighbor Address: 20.30.128.128
        IPv4 Interface Address: 20.30.128.30
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : 0000.0000.0124.00   Metric: 1
        IPv4 Neighbor Address: 21.30.124.124
        IPv4 Interface Address: 21.30.124.30
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : 0000.0000.0128.00   Metric: 1
        IPv4 Neighbor Address: 21.30.128.128
        IPv4 Interface Address: 21.30.128.30
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 1
        IPv4 Neighbor Address: 20.30.156.156
        IPv4 Interface Address: 20.30.156.30
        Adj-sid: 378540 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 1
        IPv4 Neighbor Address: 21.30.156.156
        IPv4 Interface Address: 21.30.156.30
        Adj-sid: 378574 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 1
        IPv4 Neighbor Address: 20.30.179.179
        IPv4 Interface Address: 20.30.179.30
        Adj-sid: 378538 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Juniper-131-JCNR.00 Metric: 1
        IPv4 Neighbor Address: 20.30.131.131
        IPv4 Interface Address: 20.30.131.30
        Adj-sid: 378533 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor (MT-IPv6): Arista-PE32-Q2C-32.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:32::32
        Global IPv6 Interface Address: 2001:0:30:32::30
        Adj-sid: 378589 flags: [L V F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor (MT-IPv6): Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:156::156
        Global IPv6 Interface Address: 2001:0:30:156::30
        Adj-sid: 378541 flags: [L V F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor (MT-IPv6): Nokia-SR1-217.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:30:217::217
        Global IPv6 Interface Address: 2001:0:30:217::30
        Adj-sid: 378583 flags: [L V F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
        SR Prefix-SID: 158 Flags: [N] Algorithm: 128
        SR Prefix-SID: 159 Flags: [N] Algorithm: 129
        SR Prefix-SID: 160 Flags: [N] Algorithm: 130
      Reachability (MT-IPv6): 2001:0:30:128::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:124::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::30/128 Metric: 10 Type: 1 Up
        SR Prefix-SID: 430 Flags: [N] Algorithm: 0
        SR Prefix-SID: 558 Flags: [N] Algorithm: 128
        SR Prefix-SID: 559 Flags: [N] Algorithm: 129
        SR Prefix-SID: 560 Flags: [N] Algorithm: 130
    Arista-Spine3-Q2A-30.00-02       326  59861   667    203 L2  0000.0000.0030.00-02  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 367 s
      IS Neighbor (MT-IPv6): H3C_M1A_120.00      Metric: 10
        IPv6 Neighbor Address: 2001:0:30:120::120
        Global IPv6 Interface Address: 2001:0:30:120::30
        Adj-sid: 378598 flags: [L V F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor (MT-IPv6): Ericsson_84_R6678.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:84::175
        Global IPv6 Interface Address: 2001:0:30:84::30
        Adj-sid: 378587 flags: [L V F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
    Arista-PE32-Q2C-32.00-00       780  32665   851    592 L2  0000.0000.0032.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE32-Q2C-32
      TE IPv4 router ID: 10.0.0.32
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.30.32.32
      Interface address: 20.32.175.32
      Interface address: 10.0.0.32
      Interface address: 2001:0:30:32::32
      Interface address: 2001:0:32:175::32
      Interface address: 2002::32
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.32.30
        IPv4 Interface Address: 20.30.32.32
        Adj-sid: 362168 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.32.175.175
        IPv4 Interface Address: 20.32.175.32
        Adj-sid: 362170 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:32::30
        Global IPv6 Interface Address: 2001:0:30:32::32
        Adj-sid: 362169 flags: [L V F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:32:175::175
        Global IPv6 Interface Address: 2001:0:32:175::32
        Adj-sid: 362171 flags: [L V F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      Reachability         : 20.30.32.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.32.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.32/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 32 Flags: [N] Algorithm: 0
        SR Prefix-SID: 161 Flags: [N] Algorithm: 128
        SR Prefix-SID: 162 Flags: [N] Algorithm: 129
        SR Prefix-SID: 163 Flags: [N] Algorithm: 130
      Reachability (MT-IPv6): 2001:0:30:32::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:32:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::32/128 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.32 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
    Arrcus-53.00-00            1221  34308   843    444 L2  0000.0000.0053.00-00  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arrcus-53
      TE IPv4 router ID: 10.0.0.53
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.53
      Interface address: 2002::53
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.53.175.175
        IPv4 Interface Address: 20.53.175.53
        Global IPv6 Interface Address: 2001:0:53:175::53
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100/100 us
        Application Specific Link Attributes:
          Standard applications: SR-TE
            Administrative group (Color): ARISTA(2)
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Interface Address: 20.53.175.53
        Global IPv6 Interface Address: 2001:0:53:175::53
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100/100 us
        Application Specific Link Attributes:
          Standard applications: SR-TE
            Administrative group (Color): ARISTA(2)
      Reachability         : 20.53.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.53/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 53 Flags: [N P E] Algorithm: 0
        SR Prefix-SID: 1181 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1182 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1183 Flags: [N] Algorithm: 130
      Reachability (MT-IPv6): 2001:0:53:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::53/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 453 Flags: [N P E] Algorithm: 0
        SR Prefix-SID: 1581 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1582 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1583 Flags: [N] Algorithm: 130
      Router Capabilities: Router Id: 10.0.0.53 Flags: []
        SR Local Block:
          SRLB Base: 16000 Range: 3001
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 780001
        Algorithms:  0, 128, 129, 130
    Ciena-8140-66.00-00         314  39033   309    336 L2  0000.0000.0066.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-8140-66
      TE IPv4 router ID: 10.0.0.66
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.66
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.66.175.175
        IPv4 Interface Address: 20.66.175.66
        Adj-sid: 16004 flags: [L V] weight: 0x0
        TE default metric: 100
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 8.50 Gbps
        Unreserved BW:
            TE class 0: 8.50 Gbps	TE class 1: 8.50 Gbps	TE class 2: 8.50 Gbps
            TE class 3: 8.50 Gbps	TE class 4: 8.50 Gbps	TE class 5: 8.50 Gbps
            TE class 6: 8.50 Gbps	TE class 7: 8.50 Gbps
        Local link ID: 1073731826
        Remote link ID: 1016
        Application Specific Link Attributes:
          Standard applications: RSVP-TE SR-TE LFA Flex-Algo
            TE default metric: 100
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.66.30
        IPv4 Interface Address: 20.30.66.66
        Adj-sid: 16005 flags: [L V] weight: 0x0
        TE default metric: 10
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 8.50 Gbps
        Unreserved BW:
            TE class 0: 8.50 Gbps	TE class 1: 8.50 Gbps	TE class 2: 8.50 Gbps
            TE class 3: 8.50 Gbps	TE class 4: 8.50 Gbps	TE class 5: 8.50 Gbps
            TE class 6: 8.50 Gbps	TE class 7: 8.50 Gbps
        Local link ID: 1073731827
        Remote link ID: 110
        Application Specific Link Attributes:
          Standard applications: RSVP-TE SR-TE LFA Flex-Algo
            TE default metric: 10
      Reachability         : 10.0.0.66/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 66 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1195 Flags: [N] Algorithm: 129
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.175.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.66 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ciena-5134-72.00-00         315  30789   353    336 L2  0000.0000.0072.00-00  <>
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
        Adj-sid: 16001 flags: [L V] weight: 0x0
        TE default metric: 10
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 8.50 Gbps
        Unreserved BW:
            TE class 0: 8.50 Gbps	TE class 1: 8.50 Gbps	TE class 2: 8.50 Gbps
            TE class 3: 8.50 Gbps	TE class 4: 8.50 Gbps	TE class 5: 8.50 Gbps
            TE class 6: 8.50 Gbps	TE class 7: 8.50 Gbps
        Local link ID: 1073731827
        Remote link ID: 109
        Application Specific Link Attributes:
          Standard applications: RSVP-TE SR-TE LFA Flex-Algo
            TE default metric: 10
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.72.175.175
        IPv4 Interface Address: 20.72.175.72
        Adj-sid: 16000 flags: [L V] weight: 0x0
        TE default metric: 100
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 8.50 Gbps
        Unreserved BW:
            TE class 0: 8.50 Gbps	TE class 1: 8.50 Gbps	TE class 2: 8.50 Gbps
            TE class 3: 8.50 Gbps	TE class 4: 8.50 Gbps	TE class 5: 8.50 Gbps
            TE class 6: 8.50 Gbps	TE class 7: 8.50 Gbps
        Local link ID: 1073731826
        Remote link ID: 1015
        Application Specific Link Attributes:
          Standard applications: RSVP-TE SR-TE LFA Flex-Algo
            TE default metric: 100
      Reachability         : 10.0.0.72/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 72 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1201 Flags: [N] Algorithm: 129
      Reachability         : 20.72.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.72 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ericsson_84_R6678.00-00       828  16588  1050    324 L2  0000.0000.0084.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Ericsson_84_R6678
      TE IPv4 router ID: 10.0.0.84
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.84
      Interface address: 2001:0:30:84::175
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 30
        IPv4 Interface Address: 20.84.175.84
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Interface Address: 20.30.84.84
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:84:175::175
        Global IPv6 Interface Address: 2001:0:84:175::175
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:84::30
        Global IPv6 Interface Address: 2001:0:30:84::175
      Reachability         : 10.0.0.84/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 84 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:84:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.84 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    H3C_M1A_120.00-00          4124  14887   844   1436 L2  0000.0000.0120.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: H3C_M1A_120
      TE IPv4 router ID: 10.0.0.120
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.120
      Interface address: 20.30.120.120
      Interface address: 20.120.175.120
      Interface address: 20.120.214.120
      Interface address: 2001:0:30:120::120
      Interface address: 2001:0:120:175::120
      Interface address: 2001:0:120:214::120
      Interface address: 2002::120
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.120.30
        IPv4 Interface Address: 20.30.120.120
        Adj-sid: 1150 flags: [L V] weight: 0x0
        TE default metric: 10
        Maximum link BW: 0.00 bps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
        Local link ID: 3
        Remote link ID: 135
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.120.30
        IPv4 Interface Address: 20.30.120.120
        Local link ID: 3
        Remote link ID: 135
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
          User-defined applications: APP3
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Maximum link BW: 0.00 bps
            Maximum reservable link BW: 0.00 bps
            Unreserved BW:
                TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
                TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
                TE class 6: 0.00 bps	TE class 7: 0.00 bps
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.120.175.175
        IPv4 Interface Address: 20.120.175.120
        Adj-sid: 1151 flags: [L V] weight: 0x0
        TE default metric: 10
        Maximum link BW: 0.00 bps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
        Local link ID: 4
        Remote link ID: 1007
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.120.175.175
        IPv4 Interface Address: 20.120.175.120
        Local link ID: 4
        Remote link ID: 1007
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
          User-defined applications: APP3
            Administrative group (Color): 1
            TE default metric: 10
            Maximum link BW: 0.00 bps
            Maximum reservable link BW: 0.00 bps
            Unreserved BW:
                TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
                TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
                TE class 6: 0.00 bps	TE class 7: 0.00 bps
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:120::30
        Global IPv6 Interface Address: 2001:0:30:120::120
        Adj-sid: 1149 flags: [L V F] weight: 0x0
        TE default metric: 10
        Maximum link BW: 0.00 bps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
        Local link ID: 3
        Remote link ID: 135
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:120::30
        Global IPv6 Interface Address: 2001:0:30:120::120
        Local link ID: 3
        Remote link ID: 135
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
          User-defined applications: APP3
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Maximum link BW: 0.00 bps
            Maximum reservable link BW: 0.00 bps
            Unreserved BW:
                TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
                TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
                TE class 6: 0.00 bps	TE class 7: 0.00 bps
      Reachability         : 10.0.0.120/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 120 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1248 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1249 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1250 Flags: [N] Algorithm: 130
      Reachability         : 20.30.120.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.217.0/24 Metric: 0 Type: 1 Up
      Reachability         : 192.168.20.0/23 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:217::/64 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2002::120/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 520 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1648 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1649 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1650 Flags: [N] Algorithm: 130
      Router Capabilities: Router Id: 10.0.0.120 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  13
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 128
          Exclude admin groups: 1
          Flags: [M] 0x80
      Shared Risk Link Group:  Neighbor Arista-Spine3-Q2A-30.00 (Numbered)
        Interface Address: 20.30.120.120
        Neighbor Address: 20.30.120.30
        Group ID: 1
      IPv6 Shared Risk Link Group:  Neighbor Arista-Spine3-Q2A-30.00
        Interface Address: 2001:0:30:120::120
        Neighbor Address: 2001:0:30:120::30
        Group ID: 1
      Application Specific Shared Risk Link Group:  Neighbor Arista-Spine3-Q2A-30.00
        Standard applications: Flex-Algo
        User-defined applications: APP3
        Local link identifier: 337541240
        Remote link identifier: 337541150
        IPv4 interface address: 20.30.120.120
        IPv4 neighbor address: 20.30.120.30
        IPv6 interface address: 2001:0:30:120::120
        IPv6 neighbor address: 2001:0:30:120::30
        Group ID: 1
    H3C_M1A_120.00-01           370  31719   842    357 L2  0000.0000.0120.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:120:175::175
        Global IPv6 Interface Address: 2001:0:120:175::120
        Adj-sid: 1148 flags: [L V F] weight: 0x0
        TE default metric: 10
        Maximum link BW: 0.00 bps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
        Local link ID: 4
        Remote link ID: 1007
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:120:175::175
        Global IPv6 Interface Address: 2001:0:120:175::120
        Local link ID: 4
        Remote link ID: 1007
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
          User-defined applications: APP3
            Administrative group (Color): 1
            TE default metric: 10
            Maximum link BW: 0.00 bps
            Maximum reservable link BW: 0.00 bps
            Unreserved BW:
                TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
                TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
                TE class 6: 0.00 bps	TE class 7: 0.00 bps
    0000.0000.0124.00-00       1866  11642   766    401 L2  0000.0000.0124.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      TE IPv4 router ID: 10.0.0.124
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 20.124.175.124
      Interface address: 10.0.0.124
      Interface address: 21.30.124.124
      Interface address: 20.30.124.124
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 15
        IPv4 Neighbor Address: 21.30.124.30
        IPv4 Interface Address: 21.30.124.124
        Adj-sid: 403 flags: [L V] weight: 0x0
        Local link ID: 9
        Remote link ID: 91
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.124.175.175
        IPv4 Interface Address: 20.124.175.124
        Adj-sid: 404 flags: [L V] weight: 0x0
        Local link ID: 11
        Remote link ID: 1013
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.124.30
        IPv4 Interface Address: 20.30.124.124
        Adj-sid: 402 flags: [L V] weight: 0x0
        Local link ID: 8
        Remote link ID: 138
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      Reachability         : 10.0.0.124/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 124 Flags: [N P] Algorithm: 0
        SR Prefix-SID: 1252 Flags: [N P] Algorithm: 128
      Reachability         : 20.124.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 21.30.124.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.30.124.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.124 Flags: []
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
      Router Capabilities: Router Id: 10.0.0.124 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 2000 Range: 2001
        Algorithms:  0, 128
      Application Specific Shared Risk Link Group:  Neighbor Arista-Spine3-Q2A-30.00
        Standard applications: LFA
        Local link identifier: 9
        Remote link identifier: 91
        Group ID: 124
      Application Specific Shared Risk Link Group:  Neighbor Arista-Spine3-Q2A-30.00
        Standard applications: LFA
        Local link identifier: 8
        Remote link identifier: 138
        Group ID: 124
    0000.0000.0128.00-00       1917  42612   769    401 L2  0000.0000.0128.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      TE IPv4 router ID: 10.0.0.128
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.128
      Interface address: 20.128.175.128
      Interface address: 21.30.128.128
      Interface address: 20.30.128.128
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.128.175.175
        IPv4 Interface Address: 20.128.175.128
        Adj-sid: 48134 flags: [L V] weight: 0x0
        Local link ID: 9
        Remote link ID: 1011
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 15
        IPv4 Neighbor Address: 21.30.128.30
        IPv4 Interface Address: 21.30.128.128
        Adj-sid: 48136 flags: [L V] weight: 0x0
        Local link ID: 13
        Remote link ID: 90
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.128.30
        IPv4 Interface Address: 20.30.128.128
        Adj-sid: 48137 flags: [L V] weight: 0x0
        Local link ID: 8
        Remote link ID: 139
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      Reachability         : 10.0.0.128/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 128 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1256 Flags: [N] Algorithm: 128
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 21.30.128.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.30.128.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128
      Application Specific Shared Risk Link Group:  Neighbor Arista-Spine3-Q2A-30.00
        Standard applications: LFA
        Local link identifier: 13
        Remote link identifier: 90
        Group ID: 128
      Application Specific Shared Risk Link Group:  Neighbor Arista-Spine3-Q2A-30.00
        Standard applications: LFA
        Local link identifier: 8
        Remote link identifier: 139
        Group ID: 128
    Juniper-131-JCNR.00-00       551   5367   630    447 L2  0000.0000.0131.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-131-JCNR
      TE IPv4 router ID: 10.0.0.131
      TE IPv6 router ID: ::af4:0
      Area addresses: 49.0001
      Interface address: 10.0.0.131
      Interface address: ::af4:0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.131.175.175
        IPv4 Interface Address: 20.131.175.131
        IPv6 Neighbor Address: 2001:0:131:175::175
        Global IPv6 Interface Address: 2001:0:131:175::131
        Adj-sid: 21 flags: [L V F] weight: 0x0
        Adj-sid: 20 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100/100 us
        Average unidirectional link delay: 100 us
        Local link ID: 39
        Remote link ID: 1002
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.131.30
        IPv4 Interface Address: 20.30.131.131
        IPv6 Neighbor Address: 2001:0:30:131::30
        Global IPv6 Interface Address: 2001:0:30:131::131
        Adj-sid: 25 flags: [L V F] weight: 0x0
        Adj-sid: 24 flags: [L V] weight: 0x0
        Local link ID: 42
        Remote link ID: 62
      Reachability         : 20.131.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.131/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 131 Flags: [N] Algorithm: 0
      Reachability         : 20.30.131.0/24 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:131:175::/64 Metric: 10 Type: 1 Up
      Reachability          : fe80::ec97:fbff:fe06:5964/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:30:131::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.131 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    Juniper-156-PTX10002-36QDD.00-00       612  53877  1132   1014 L2  0000.0000.0156.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-156-PTX10002-36QDD
      TE IPv4 router ID: 10.0.0.156
      TE IPv6 router ID: 2002::156
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.156
      Interface address: 2002::156
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.156.30
        IPv4 Interface Address: 20.30.156.156
        IPv6 Neighbor Address: 2001:0:30:156::30
        Global IPv6 Interface Address: 2001:0:30:156::156
        Adj-sid: 22 flags: [L V B] weight: 0x0
        TE default metric: 100
        Min/Max unidirectional link delay: 10000/10000 us
        Average unidirectional link delay: 10000 us
        Local link ID: 1009
        Remote link ID: 56
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.156.175.175
        IPv4 Interface Address: 20.156.175.156
        IPv6 Neighbor Address: 2001:0:156:175::175
        Global IPv6 Interface Address: 2001:0:156:175::156
        Adj-sid: 18 flags: [L V B] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1010
        Remote link ID: 1056
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 15
        IPv4 Neighbor Address: 21.30.156.30
        IPv4 Interface Address: 21.30.156.156
        Adj-sid: 24 flags: [L V B] weight: 0x0
        TE default metric: 100
        Min/Max unidirectional link delay: 10000/10000 us
        Average unidirectional link delay: 10000 us
        Local link ID: 1045
        Remote link ID: 104
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Interface Address: 20.30.156.156
        IPv6 Neighbor Address: 2001:0:30:156::30
        Global IPv6 Interface Address: 2001:0:30:156::156
        Adj-sid: 23 flags: [L V B F] weight: 0x0
        TE default metric: 100
        Min/Max unidirectional link delay: 10000/10000 us
        Average unidirectional link delay: 10000 us
        Local link ID: 1009
        Remote link ID: 56
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Interface Address: 20.156.175.156
        IPv6 Neighbor Address: 2001:0:156:175::175
        Global IPv6 Interface Address: 2001:0:156:175::156
        Adj-sid: 19 flags: [L V B F] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1010
        Remote link ID: 1056
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      Reachability         : 10.0.0.156/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 156 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1286 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1285 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1284 Flags: [N] Algorithm: 128
      Reachability         : 20.30.156.0/24 Metric: 10 Type: 1 Up
      Reachability         : 21.30.156.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.156.175.0/24 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::156/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 556 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1686 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1685 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1684 Flags: [N] Algorithm: 128
      Reachability (MT-IPv6): 2001:0:156:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:156::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.156 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
      Shared Risk Link Group:  Neighbor Arista-Spine3-Q2A-30.00 (Numbered)
        Interface Address: 20.30.156.156
        Neighbor Address: 20.30.156.30
        Group ID: 2
      Shared Risk Link Group:  Neighbor Arista-Spine3-Q2A-30.00 (Numbered)
        Interface Address: 21.30.156.156
        Neighbor Address: 21.30.156.30
        Group ID: 2
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-00       972  38906   961   1178 L2  0000.0000.0175.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-175-ACX7100-48L
      TE IPv4 router ID: 10.0.0.175
      TE IPv6 router ID: 2002::175
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.175
      Interface address: 127.0.0.1
      Interface address: 2002::175
      IS Neighbor          : Juniper-131-JCNR.00 Metric: 10
        IPv4 Neighbor Address: 20.131.175.131
        IPv4 Interface Address: 20.131.175.175
        IPv6 Neighbor Address: 2001:0:131:175::131
        Global IPv6 Interface Address: 2001:0:131:175::175
        Adj-sid: 116 flags: [L V F] weight: 0x0
        Adj-sid: 115 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1002
        Remote link ID: 39
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 10
        IPv4 Neighbor Address: 20.175.179.179
        IPv4 Interface Address: 20.175.179.175
        IPv6 Neighbor Address: 2001:0:175::179:179
        Global IPv6 Interface Address: 2001:0:175::179:175
        Adj-sid: 106 flags: [L V F] weight: 0x0
        Adj-sid: 105 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1005
        Remote link ID: 1010
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : H3C_M1A_120.00      Metric: 10
        IPv4 Neighbor Address: 20.120.175.120
        IPv4 Interface Address: 20.120.175.175
        IPv6 Neighbor Address: 2001:0:120:175::120
        Global IPv6 Interface Address: 2001:0:120:175::175
        Adj-sid: 173 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1007
        Remote link ID: 4
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor (MT-IPv6): Nokia-SR1-217.00    Metric: 10
        IPv4 Interface Address: 20.175.217.175
        IPv6 Neighbor Address: 2001:0:175:217::217
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 98 flags: [L V F] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1003
        Remote link ID: 10
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability         : 10.0.0.175/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 175 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1305 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1304 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1303 Flags: [N] Algorithm: 128
      Reachability         : 20.156.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.72.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.84.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.131.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.32.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.124.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::175/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 575 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1705 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1704 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1703 Flags: [N] Algorithm: 128
      Reachability (MT-IPv6): 2001:0:156:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:84:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:53:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:66:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:72:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:32:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:128:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:221::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.175 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  3
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 0
          Exclude admin groups: 1
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 238
          Flags: [M] 0x80
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 0
          Flags: [M] 0x80
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-01       843  37080  1174   1107 L2  0000.0000.0175.00-01  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 10
        IPv4 Neighbor Address: 20.84.175.84
        IPv4 Interface Address: 20.84.175.175
        IPv6 Neighbor Address: 2001:0:84:175::175
        Global IPv6 Interface Address: 2001:0:84:175::175
        Adj-sid: 132 flags: [L V F] weight: 0x0
        Adj-sid: 131 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1010
        Remote link ID: 528
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : Nokia-SXR-214.00    Metric: 10
        IPv4 Neighbor Address: 20.175.214.214
        IPv4 Interface Address: 20.175.214.175
        IPv6 Neighbor Address: 2001:0:175:214::214
        Global IPv6 Interface Address: 2001:0:175:214::175
        Adj-sid: 151 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1014
        Remote link ID: 11
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.156.175.156
        IPv4 Interface Address: 20.156.175.175
        IPv6 Neighbor Address: 2001:0:156:175::156
        Global IPv6 Interface Address: 2001:0:156:175::175
        Adj-sid: 130 flags: [L V F] weight: 0x0
        Adj-sid: 129 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1056
        Remote link ID: 1010
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.175.217.217
        IPv4 Interface Address: 20.175.217.175
        IPv6 Neighbor Address: 2001:0:175:217::217
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 140 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1003
        Remote link ID: 10
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 10
        IPv4 Neighbor Address: 20.32.175.32
        IPv4 Interface Address: 20.32.175.175
        IPv6 Neighbor Address: 2001:0:32:175::32
        Global IPv6 Interface Address: 2001:0:32:175::175
        Adj-sid: 147 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1004
        Remote link ID: 88
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.128.175.128
        IPv4 Interface Address: 20.128.175.175
        Global IPv6 Interface Address: 2001:0:128:175::175
        Adj-sid: 96 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1011
        Remote link ID: 9
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor (MT-IPv6): Nokia-SXR-214.00    Metric: 10
        IPv4 Interface Address: 20.175.214.175
        IPv6 Neighbor Address: 2001:0:175:214::214
        Global IPv6 Interface Address: 2001:0:175:214::175
        Adj-sid: 108 flags: [L V F] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1014
        Remote link ID: 11
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor (MT-IPv6): Arista-PE32-Q2C-32.00 Metric: 10
        IPv4 Interface Address: 20.32.175.175
        IPv6 Neighbor Address: 2001:0:32:175::32
        Global IPv6 Interface Address: 2001:0:32:175::175
        Adj-sid: 148 flags: [L V F] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1004
        Remote link ID: 88
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
    Juniper-175-ACX7100-48L.00-02       479  26376  1174   1174 L2  0000.0000.0175.00-02  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      IS Neighbor          : Ciena-5134-72.00    Metric: 10
        IPv4 Neighbor Address: 20.72.175.72
        IPv4 Interface Address: 20.72.175.175
        Global IPv6 Interface Address: 2001:0:72:175::175
        Adj-sid: 167 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1015
        Remote link ID: 1073731826
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.175.53
        IPv4 Interface Address: 20.53.175.175
        IPv6 Neighbor Address: 2001:0:53:175::53
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 99 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1008
        Remote link ID: 1002
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : 0000.0000.0124.00   Metric: 10
        IPv4 Neighbor Address: 20.124.175.124
        IPv4 Interface Address: 20.124.175.175
        Adj-sid: 170 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1013
        Remote link ID: 11
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.66.175.66
        IPv4 Interface Address: 20.66.175.175
        Global IPv6 Interface Address: 2001:0:66:175::175
        Adj-sid: 163 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1016
        Remote link ID: 1073731826
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : 221.00              Metric: 10
        IPv4 Neighbor Address: 20.175.221.221
        IPv4 Interface Address: 20.175.221.175
        Global IPv6 Interface Address: 2001:0:175:221::175
        Adj-sid: 171 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1009
        Remote link ID: 8388613
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor (MT-IPv6): Ericsson_84_R6678.00 Metric: 10
        IPv4 Interface Address: 20.84.175.175
        IPv6 Neighbor Address: 2001:0:84:175::175
        Global IPv6 Interface Address: 2001:0:84:175::175
        Adj-sid: 132 flags: [L V F] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1010
        Remote link ID: 528
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor (MT-IPv6): Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Interface Address: 20.156.175.175
        IPv6 Neighbor Address: 2001:0:156:175::156
        Global IPv6 Interface Address: 2001:0:156:175::175
        Adj-sid: 130 flags: [L V F] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1056
        Remote link ID: 1010
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor (MT-IPv6): Arrcus-53.00        Metric: 10
        IPv4 Interface Address: 20.53.175.175
        IPv6 Neighbor Address: 2001:0:53:175::53
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 133 flags: [L V F] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1008
        Remote link ID: 1002
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor (MT-IPv6): H3C_M1A_120.00      Metric: 10
        IPv4 Interface Address: 20.120.175.175
        IPv6 Neighbor Address: 2001:0:120:175::120
        Global IPv6 Interface Address: 2001:0:120:175::175
        Adj-sid: 174 flags: [L V F] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1007
        Remote link ID: 4
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      Reachability (MT-IPv6): 2001:0:131:175::/64 Metric: 10 Type: 1 Up
    Juniper-179-ACX7024.00-00       720  31209   830    543 L2  0000.0000.0179.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-179-ACX7024
      TE IPv4 router ID: 10.0.0.179
      TE IPv6 router ID: 2001:0:30:179::179
      Area addresses: 49.0001
      Interface address: 10.0.0.179
      Interface address: 127.0.0.1
      Interface address: 10.0.1.179
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.179.175
        IPv4 Interface Address: 20.175.179.179
        IPv6 Neighbor Address: 2001:0:175::179:175
        Global IPv6 Interface Address: 2001:0:175::179:179
        Adj-sid: 20 flags: [L V F] weight: 0x0
        Adj-sid: 19 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1010
        Remote link ID: 1005
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 4000
        IPv4 Neighbor Address: 20.30.179.30
        IPv4 Interface Address: 20.30.179.179
        IPv6 Neighbor Address: 2001:0:30:179::30
        Global IPv6 Interface Address: 2001:0:30:179::179
        Adj-sid: 24 flags: [L V F] weight: 0x0
        Adj-sid: 23 flags: [L V] weight: 0x0
        TE default metric: 100
        Min/Max unidirectional link delay: 10000/10000 us
        Average unidirectional link delay: 10000 us
        Local link ID: 1014
        Remote link ID: 44
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      Reachability         : 10.0.0.179/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 179 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1309 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1308 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1307 Flags: [N] Algorithm: 128
      Reachability         : 20.175.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability         : 10.0.1.179/32 Metric: 0 Type: 1 Up
      Reachability         : 20.30.179.0/24 Metric: 4000 Type: 1 Up
      Reachability          : 2001:0:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:179::/64 Metric: 4000 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.179 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    Nokia-SXR-214.00-00       17980  12329   577    620 L2  0000.0000.0214.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SXR-214
      TE IPv4 router ID: 10.0.0.214
      TE IPv6 router ID: 2000::214
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.214
      Interface address: 20.30.214.214
      Interface address: 20.175.214.214
      Interface address: 20.214.216.214
      Interface address: 2000::214
      Interface address: 2001:0:175:214::214
      Interface address: 2001:0:214:216::214
      IS Neighbor          : Nokia-IXRe2-216.00  Metric: 10
        IPv4 Neighbor Address: 20.214.216.216
        IPv4 Interface Address: 20.214.216.214
        Adj-sid: 30031 flags: [L V B] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 100
        IPv4 Neighbor Address: 20.175.214.175
        IPv4 Interface Address: 20.175.214.214
        Adj-sid: 30033 flags: [L V B] weight: 0x0
        TE default metric: 100
        Maximum link BW: 80.00 Mbps
        Application Specific Link Attributes:
          Standard applications: [L] SR-TE
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 1
        IPv4 Neighbor Address: 20.30.214.30
        IPv4 Interface Address: 20.30.214.214
        Adj-sid: 30042 flags: [L V B] weight: 0x0
        TE default metric: 1
        Maximum link BW: 80.00 Mbps
        Application Specific Link Attributes:
          Standard applications: [L] SR-TE
      IS Neighbor (MT-IPv6): Nokia-IXRe2-216.00  Metric: 10
        IPv6 Neighbor Address: 2001:0:214:216::216
        Global IPv6 Interface Address: 2001:0:214:216::214
        Adj-sid: 30032 flags: [L V B F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:175:214::175
        Global IPv6 Interface Address: 2001:0:175:214::214
        Adj-sid: 30034 flags: [L V B F] weight: 0x0
        TE default metric: 10
        Maximum link BW: 80.00 Mbps
        Application Specific Link Attributes:
          Standard applications: [L] SR-TE
      Reachability         : 20.30.214.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.214.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.214/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 214 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2000::214/128 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:214:216::/64 Metric: 10 Type: 1 Up
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
    Nokia-IXRe2-216.00-00      1685  26085   660    486 L2  0100.0000.0216.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-IXRe2-216
      TE IPv4 router ID: 10.0.0.216
      TE IPv6 router ID: 2002::216
      Area addresses: 49.0001.0000.0000.0216.00
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.216
      Interface address: 20.214.216.216
      Interface address: 2001:0:214:216::216
      Interface address: 2002::216
      IS Neighbor          : Nokia-SXR-214.00    Metric: 10
        IPv4 Neighbor Address: 20.214.216.214
        IPv4 Interface Address: 20.214.216.216
        IPv6 Neighbor Address: 2001:0:214:216::214
        Global IPv6 Interface Address: 2001:0:214:216::216
        Adj-sid: 1048575 flags: [L V B] weight: 0x0
        Adj-sid: 1048573 flags: [L V B F] weight: 0x0
      IS Neighbor (MT-IPv6): Nokia-SXR-214.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:214:216::214
        Global IPv6 Interface Address: 2001:0:214:216::216
      Reachability         : 20.214.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.216/32 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:214:216::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::216/128 Metric: 0 Type: 1 Up
      Reachability          : 5f00:0:2216::/48 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:214:216::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::216/128 Metric: 0 Type: 1 Up
      SRv6 Locator: 5f00:0:2216::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : 5f00:0:2216::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.0.216 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  11
        SRv6 Capability: Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-SR1-217.00-00        1105  16143   930    594 L2  0100.0000.0217.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SR1-217
      TE IPv4 router ID: 10.0.0.217
      TE IPv6 router ID: 2002::217
      Area addresses: 49.0001.0000.0000.0217.00
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.217
      Interface address: 20.30.217.217
      Interface address: 20.175.217.217
      Interface address: 2001:0:30:217::217
      Interface address: 2001:0:175:217::217
      Interface address: 2002::217
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.217.175
        IPv4 Interface Address: 20.175.217.217
        Adj-sid: 524283 flags: [L V B] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: SR-TE
            Administrative group (Color): 1
            TE default metric: 10
            Maximum link BW: 10.00 Gbps
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.217.30
        IPv4 Interface Address: 20.30.217.217
        Adj-sid: 524285 flags: [L V B] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: SR-TE
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Maximum link BW: 10.00 Gbps
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 100
            Min/Max unidirectional link delay: 10000/10000 us
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
      Reachability         : 10.0.0.217/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 217 Flags: [N P] Algorithm: 0
        SR Prefix-SID: 1345 Flags: [N P] Algorithm: 128
        SR Prefix-SID: 1346 Flags: [N P] Algorithm: 129
        SR Prefix-SID: 1347 Flags: [N P] Algorithm: 130
      Reachability         : 20.30.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.217.0/24 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::217/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.217 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 100
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 100
          Flags: [M] 0x80
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 100
          Exclude admin groups: 1
          Flags: [M] 0x80
      Application Specific Shared Risk Link Group:  Neighbor Arista-Spine3-Q2A-30.00
        Standard applications: SR-TE
        IPv4 interface address: 20.30.217.217
        IPv4 neighbor address: 20.30.217.30
        IPv6 interface address: 2001:0:30:217::217
        IPv6 neighbor address: 2001:0:30:217::30
        Group ID: 1
    221.00-00                   720  65427   680     85 L2  0221.0221.0221.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      TE IPv4 router ID: 10.0.0.221
      Area addresses: 49.0001
      Router Capabilities: Router Id: 10.0.0.221 Flags: []
        SR Local Block:
          SRLB Base: 626688 Range: 14336
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 720000 Range: 2000
        Algorithms:  0, 128, 129
      Unsupported TLV: Type: 14 Length: 2
    221.00-01                   652  49185   846     32 L2  0221.0221.0221.00-01  <>
      Hostname: 221
    221.00-02                  9068  40768   846    483 L2  0221.0221.0221.00-02  <>
      Remaining lifetime received: 1197 s Modified to: 1200 s
      Interface address: 10.0.0.221
      Interface address: 20.175.221.221
      Interface address: 20.30.221.221
      Interface address: 1221::1
      Interface address: 2001:0:175:221::221
      Interface address: 2001:0:30:221::221
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.221.175
        IPv4 Interface Address: 20.175.221.221
        Adj-sid: 524296 flags: [L V B] weight: 0x0
        Adj-sid: 524290 flags: [L V] weight: 0x0
        Administrative group (Color): 1
        TE default metric: 10
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Min/Max unidirectional link delay: 10/10 us
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 10/10 us
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.221.30
        IPv4 Interface Address: 20.30.221.221
        Adj-sid: 524295 flags: [L V B] weight: 0x0
        Adj-sid: 524294 flags: [L V] weight: 0x0
        Administrative group (Color): ARISTA(2)
        TE default metric: 10
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Min/Max unidirectional link delay: 100/100 us
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): ARISTA(2)
            TE default metric: 10
            Min/Max unidirectional link delay: 100/100 us
      Reachability         : 10.0.0.221/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 221 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1349 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1350 Flags: [N] Algorithm: 129
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.221.0/24 Metric: 10 Type: 1 Up
      Reachability          : 1221::1/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:175:221::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:221::/64 Metric: 10 Type: 1 Up

```

## show isis flex-algo path

```text
Flex algo paths for IPv4 address family
Topology ID: Level-2
  Destination                     Algorithm         Next Hop         Interface 
------------------------------- ---------------- ------------------- ----------
  221                             MIN-LATENCY       20.30.221.221    Ethernet15
                                                                               
  221                             MIN-TE            20.30.221.221    Ethernet15
                                                                               
  Arista-PE32-Q2C-32              MIN-LATENCY       20.30.32.32      Ethernet2 
                                                                               
  Arista-PE32-Q2C-32              MIN-TE            20.30.32.32      Ethernet2 
                                                                               
  Arista-PE32-Q2C-32              ADMIN             20.30.32.32      Ethernet2 
                                                                               
  Arista-Spine3-Q2A-30            MIN-LATENCY                                  
                                                                               
  Arista-Spine3-Q2A-30            MIN-TE                                       
                                                                               
  Arista-Spine3-Q2A-30            ADMIN                                        
                                                                               
  Arrcus-53                       MIN-LATENCY       20.30.221.221    Ethernet15
                                                                               
  Arrcus-53                       MIN-TE            20.30.217.217    Ethernet4 
                                                    20.30.179.179    Ethernet40
                                                    20.30.221.221    Ethernet15
                                                    20.30.156.156    Ethernet11
                                                    21.30.156.156    Ethernet21
                                                    20.30.32.32      Ethernet2 
                                                                               
  Arrcus-53                       ADMIN                                        
                                                                               
  Ciena-5134-72                   MIN-TE                                       
                                                                               
  Ciena-8140-66                   MIN-TE                                       
                                                                               
  H3C_M1A_120                     MIN-LATENCY       20.30.221.221    Ethernet15
                                                                               
  H3C_M1A_120                     MIN-TE            20.30.217.217    Ethernet4 
                                                    20.30.179.179    Ethernet40
                                                    20.30.221.221    Ethernet15
                                                    20.30.156.156    Ethernet11
                                                    21.30.156.156    Ethernet21
                                                    20.30.32.32      Ethernet2 
                                                                               
  H3C_M1A_120                     ADMIN                                        
                                                                               
  Juniper-156-PTX10002-36QDD      MIN-LATENCY       20.30.156.156    Ethernet11
                                                    21.30.156.156    Ethernet21
                                                                               
  Juniper-156-PTX10002-36QDD      MIN-TE            20.30.156.156    Ethernet11
                                                    21.30.156.156    Ethernet21
                                                                               
  Juniper-156-PTX10002-36QDD      ADMIN             20.30.156.156    Ethernet11
                                                    21.30.156.156    Ethernet21
                                                                               
  Juniper-175-ACX7100-48L         MIN-LATENCY       20.30.221.221    Ethernet15
                                                                               
  Juniper-175-ACX7100-48L         MIN-TE            20.30.217.217    Ethernet4 
                                                    20.30.179.179    Ethernet40
                                                    20.30.221.221    Ethernet15
                                                    20.30.156.156    Ethernet11
                                                    21.30.156.156    Ethernet21
                                                    20.30.32.32      Ethernet2 
                                                                               
  Juniper-175-ACX7100-48L         ADMIN             20.30.131.131    Ethernet35
                                                                               
  Juniper-179-ACX7024             MIN-LATENCY       20.30.179.179    Ethernet40
                                                                               
  Juniper-179-ACX7024             MIN-TE            20.30.179.179    Ethernet40
                                                                               
  Juniper-179-ACX7024             ADMIN             20.30.179.179    Ethernet40
                                                                               
  Nokia-SR1-217                   MIN-LATENCY       20.30.217.217    Ethernet4 
                                                                               
  Nokia-SR1-217                   MIN-TE            20.30.217.217    Ethernet4 
                                                                               
  Nokia-SR1-217                   ADMIN             20.30.217.217    Ethernet4 
                                                                               

Flex algo paths for IPv6 address family
Topology ID: Level-2
Destination                 Algorithm     Next Hop                   Interface 
--------------------------- ------------ --------------------------- ----------
Arista-Spine3-Q2A-30        MIN-LATENCY                                        
                                                                               
Arista-Spine3-Q2A-30        MIN-TE                                             
                                                                               
Arista-Spine3-Q2A-30        ADMIN                                              
                                                                               
Arrcus-53                   MIN-LATENCY   fe80::d248:a1ff:feba:3c61  Ethernet11
                                          fe80::d6af:f7ff:fe2f:1396  Ethernet2 
                                                                               
Arrcus-53                   MIN-TE        fe80::d248:a1ff:feba:3c61  Ethernet11
                                          fe80::d6af:f7ff:fe2f:1396  Ethernet2 
                                                                               
Arrcus-53                   ADMIN                                              
                                                                               
H3C_M1A_120                 MIN-LATENCY                                        
                                                                               
H3C_M1A_120                 MIN-TE                                             
                                                                               
H3C_M1A_120                 ADMIN                                              
                                                                               
Juniper-156-PTX10002-36QDD  MIN-LATENCY   fe80::d248:a1ff:feba:3c61  Ethernet11
                                                                               
Juniper-156-PTX10002-36QDD  MIN-TE        fe80::d248:a1ff:feba:3c61  Ethernet11
                                                                               
Juniper-156-PTX10002-36QDD  ADMIN         fe80::d248:a1ff:feba:3c61  Ethernet11
                                                                               
Juniper-175-ACX7100-48L     MIN-LATENCY   fe80::d248:a1ff:feba:3c61  Ethernet11
                                          fe80::d6af:f7ff:fe2f:1396  Ethernet2 
                                                                               
Juniper-175-ACX7100-48L     MIN-TE        fe80::d248:a1ff:feba:3c61  Ethernet11
                                          fe80::d6af:f7ff:fe2f:1396  Ethernet2 
                                                                               
Juniper-175-ACX7100-48L     ADMIN         fe80::c214:b8ff:fe21:9790  Ethernet4 
                                                                               

```

## show isis flex-algo path detail

```text
Flex algo paths for IPv4 address family
Topology ID: Level-2
Destination: 221
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 15:05:58 ago
Metric: 10000
Next Hop      Interface 
------------- ----------
20.30.221.221 Ethernet15

Destination: 221
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 15:05:58 ago
Metric: 100
Next Hop      Interface 
------------- ----------
20.30.221.221 Ethernet15

Destination: Arista-PE32-Q2C-32
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 14
Last updated: 2 days, 15:40:12 ago
Metric: 10000
Next Hop    Interface
----------- ---------
20.30.32.32 Ethernet2

Destination: Arista-PE32-Q2C-32
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 14
Last updated: 2 days, 15:40:12 ago
Metric: 100
Next Hop    Interface
----------- ---------
20.30.32.32 Ethernet2

Destination: Arista-PE32-Q2C-32
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 12
Last updated: 2 days, 15:40:12 ago
Metric: 1
Next Hop    Interface
----------- ---------
20.30.32.32 Ethernet2

Destination: Arista-Spine3-Q2A-30
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 23:22:43 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 23:22:43 ago
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
Last updated: 2 days, 23:22:43 ago
Next Hop Interface
-------- ---------

Destination: Arrcus-53
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 34
Last updated: 0:05:56 ago
Metric: 110010
Next Hop      Interface 
------------- ----------
20.30.221.221 Ethernet15

Destination: Arrcus-53
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 34
Last updated: 0:05:56 ago
Metric: 120
Next Hop      Interface 
------------- ----------
20.30.217.217 Ethernet4 
20.30.179.179 Ethernet40
20.30.221.221 Ethernet15
20.30.156.156 Ethernet11
21.30.156.156 Ethernet21
20.30.32.32   Ethernet2 

Destination: Arrcus-53
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 26
Last updated: 0:05:56 ago
Next Hop Interface
-------- ---------

Destination: Ciena-5134-72
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 2 days, 15:27:56 ago
Next Hop Interface
-------- ---------

Destination: Ciena-8140-66
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 15:25:19 ago
Next Hop Interface
-------- ---------

Destination: H3C_M1A_120
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 14:19:03 ago
Metric: 110010
Next Hop      Interface 
------------- ----------
20.30.221.221 Ethernet15

Destination: H3C_M1A_120
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:05:56 ago
Metric: 120
Next Hop      Interface 
------------- ----------
20.30.217.217 Ethernet4 
20.30.179.179 Ethernet40
20.30.221.221 Ethernet15
20.30.156.156 Ethernet11
21.30.156.156 Ethernet21
20.30.32.32   Ethernet2 

Destination: H3C_M1A_120
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 14:19:03 ago
Next Hop Interface
-------- ---------

Destination: Juniper-156-PTX10002-36QDD
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 12
Last updated: 2 days, 18:18:40 ago
Metric: 10000
Next Hop      Interface 
------------- ----------
20.30.156.156 Ethernet11
21.30.156.156 Ethernet21

Destination: Juniper-156-PTX10002-36QDD
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 15
Last updated: 2 days, 18:18:40 ago
Metric: 100
Next Hop      Interface 
------------- ----------
20.30.156.156 Ethernet11
21.30.156.156 Ethernet21

Destination: Juniper-156-PTX10002-36QDD
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 10
Last updated: 2 days, 18:18:40 ago
Metric: 1
Next Hop      Interface 
------------- ----------
20.30.156.156 Ethernet11
21.30.156.156 Ethernet21

Destination: Juniper-175-ACX7100-48L
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 33
Last updated: 2 days, 15:05:36 ago
Metric: 10010
Next Hop      Interface 
------------- ----------
20.30.221.221 Ethernet15

Destination: Juniper-175-ACX7100-48L
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 184
Last updated: 0:05:56 ago
Metric: 110
Next Hop      Interface 
------------- ----------
20.30.217.217 Ethernet4 
20.30.179.179 Ethernet40
20.30.221.221 Ethernet15
20.30.156.156 Ethernet11
21.30.156.156 Ethernet21
20.30.32.32   Ethernet2 

Destination: Juniper-175-ACX7100-48L
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 16
Last updated: 2 days, 16:29:42 ago
Metric: 11
Next Hop      Interface 
------------- ----------
20.30.131.131 Ethernet35

Destination: Juniper-179-ACX7024
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 2 days, 18:24:13 ago
Metric: 10000
Next Hop      Interface 
------------- ----------
20.30.179.179 Ethernet40

Destination: Juniper-179-ACX7024
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 2 days, 18:24:13 ago
Metric: 100
Next Hop      Interface 
------------- ----------
20.30.179.179 Ethernet40

Destination: Juniper-179-ACX7024
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 2 days, 18:24:13 ago
Metric: 1
Next Hop      Interface 
------------- ----------
20.30.179.179 Ethernet40

Destination: Nokia-SR1-217
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 29
Last updated: 2 days, 15:50:38 ago
Metric: 10000
Next Hop      Interface
------------- ---------
20.30.217.217 Ethernet4

Destination: Nokia-SR1-217
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 29
Last updated: 2 days, 15:50:38 ago
Metric: 100
Next Hop      Interface
------------- ---------
20.30.217.217 Ethernet4

Destination: Nokia-SR1-217
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 24
Last updated: 2 days, 15:50:38 ago
Metric: 1
Next Hop      Interface
------------- ---------
20.30.217.217 Ethernet4

Flex algo paths for IPv6 address family
Topology ID: Level-2
Destination: Arista-Spine3-Q2A-30
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 17:19:23 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 17:19:23 ago
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
Last updated: 2 days, 17:19:23 ago
Next Hop Interface
-------- ---------

Destination: Arrcus-53
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 32
Last updated: 0:05:56 ago
Metric: 210000
Next Hop                  Interface 
------------------------- ----------
fe80::d248:a1ff:feba:3c61 Ethernet11
fe80::d6af:f7ff:fe2f:1396 Ethernet2 

Destination: Arrcus-53
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 29
Last updated: 0:05:56 ago
Metric: 120
Next Hop                  Interface 
------------------------- ----------
fe80::d248:a1ff:feba:3c61 Ethernet11
fe80::d6af:f7ff:fe2f:1396 Ethernet2 

Destination: Arrcus-53
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 21
Last updated: 0:05:56 ago
Next Hop Interface
-------- ---------

Destination: H3C_M1A_120
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 14:19:03 ago
Next Hop Interface
-------- ---------

Destination: H3C_M1A_120
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 14:19:03 ago
Next Hop Interface
-------- ---------

Destination: H3C_M1A_120
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 14:19:03 ago
Next Hop Interface
-------- ---------

Destination: Juniper-156-PTX10002-36QDD
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 5
Last updated: 2 days, 18:18:40 ago
Metric: 10000
Next Hop                  Interface 
------------------------- ----------
fe80::d248:a1ff:feba:3c61 Ethernet11

Destination: Juniper-156-PTX10002-36QDD
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 2 days, 18:18:40 ago
Metric: 100
Next Hop                  Interface 
------------------------- ----------
fe80::d248:a1ff:feba:3c61 Ethernet11

Destination: Juniper-156-PTX10002-36QDD
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 2 days, 18:18:40 ago
Metric: 10
Next Hop                  Interface 
------------------------- ----------
fe80::d248:a1ff:feba:3c61 Ethernet11

Destination: Juniper-175-ACX7100-48L
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 26
Last updated: 0:05:56 ago
Metric: 110000
Next Hop                  Interface 
------------------------- ----------
fe80::d248:a1ff:feba:3c61 Ethernet11
fe80::d6af:f7ff:fe2f:1396 Ethernet2 

Destination: Juniper-175-ACX7100-48L
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 39
Last updated: 0:05:56 ago
Metric: 110
Next Hop                  Interface 
------------------------- ----------
fe80::d248:a1ff:feba:3c61 Ethernet11
fe80::d6af:f7ff:fe2f:1396 Ethernet2 

Destination: Juniper-175-ACX7100-48L
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 20
Last updated: 2 days, 15:50:38 ago
Metric: 20
Next Hop                  Interface
------------------------- ---------
fe80::c214:b8ff:fe21:9790 Ethernet4

```

## show isis segment-routing tunnel

```text
 Index    Endpoint         Next Hop/Tunnel Index         Interface    Labels   
-------- ---------------- ---------------------------- -------------- ---------
 2        2002::120/128    fe80::be31:e2ff:fee1:ec2c     Ethernet3    [ 3 ]    
 3        2002::175/128    fe80::5a70:7fff:fe9f:c403     Ethernet12   [ 20575 ]
                           fe80::be31:e2ff:fee1:ec2c     Ethernet3    [ 20575 ]
                           fe80::c214:b8ff:fe21:9790     Ethernet4    [ 20575 ]
                           fe80::d248:a1ff:feba:3c61     Ethernet11   [ 20575 ]
                           fe80::d6af:f7ff:fe2f:1396     Ethernet2    [ 20575 ]
 5        2002::156/128    TI-LFA (10)                   -            [ 3 ]    
 6        2002::53/128     fe80::5a70:7fff:fe9f:c403     Ethernet12   [ 20453 ]
                           fe80::be31:e2ff:fee1:ec2c     Ethernet3    [ 20453 ]
                           fe80::c214:b8ff:fe21:9790     Ethernet4    [ 20453 ]
                           fe80::d248:a1ff:feba:3c61     Ethernet11   [ 20453 ]
                           fe80::d6af:f7ff:fe2f:1396     Ethernet2    [ 20453 ]
 7        10.0.0.175/32    20.30.32.32                   Ethernet2    [ 20175 ]
                           20.30.66.66                   Ethernet31   [ 20175 ]
                           20.30.72.72                   Ethernet9    [ 20175 ]
                           20.30.120.120                 Ethernet3    [ 20175 ]
                           20.30.131.131                 Ethernet35   [ 20175 ]
                           20.30.156.156                 Ethernet11   [ 20175 ]
 8        10.0.0.84/32     TI-LFA (8)                    -            [ 20084 ]
 9        10.0.0.131/32    TI-LFA (3)                    -            [ 3 ]    
 10       10.0.0.53/32     20.30.32.32                   Ethernet2    [ 20053 ]
                           20.30.66.66                   Ethernet31   [ 20053 ]
                           20.30.72.72                   Ethernet9    [ 20053 ]
                           20.30.120.120                 Ethernet3    [ 20053 ]
                           20.30.131.131                 Ethernet35   [ 20053 ]
                           20.30.156.156                 Ethernet11   [ 20053 ]
 11       10.0.0.156/32    20.30.156.156                 Ethernet11   [ 3 ]    
                           21.30.156.156                 Ethernet21   [ 3 ]    
 12       10.0.0.179/32    20.30.179.179                 Ethernet40   [ 3 ]    
 13       10.0.0.66/32     TI-LFA (7)                    -            [ 3 ]    
 14       10.0.0.72/32     TI-LFA (2)                    -            [ 3 ]    
 15       10.0.0.221/32    TI-LFA (6)                    -            [ 3 ]    
 16       10.0.0.217/32    TI-LFA (0)                    -            [ 20217 ]
 17       10.0.0.120/32    20.30.120.120                 Ethernet3    [ 3 ]    
 20       10.0.0.32/32     TI-LFA (11)                   -            [ 3 ]    
 21       10.0.0.214/32    TI-LFA (4)                    -            [ 20214 ]

```

## show isis segment-routing prefix-segments

```text

System ID: Arista-Spine3-Q2A-30			Instance: 'IGP'
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.30

Node: 62     Proxy-Node: 0      Prefix: 0       Total Segments: 62

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
   10.0.0.32/32                 32   20032 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node        SPF         
   10.0.0.32/32                161   20161 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node        MIN-LATENCY 
   10.0.0.32/32                162   20162 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node        MIN-TE      
   10.0.0.32/32                163   20163 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node        ADMIN       
   10.0.0.53/32                 53   20053 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    unprotected SPF         
   10.0.0.53/32               1181   21181 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        MIN-LATENCY 
   10.0.0.53/32               1182   21182 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    unprotected MIN-TE      
   10.0.0.53/32               1183   21183 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    unprotected ADMIN       
   10.0.0.66/32                 66   20066 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-8140-66   L2    node        SPF         
   10.0.0.66/32               1195   21195 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-8140-66   L2    unprotected MIN-TE      
   10.0.0.72/32                 72   20072 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    node        SPF         
   10.0.0.72/32               1201   21201 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    unprotected MIN-TE      
   10.0.0.84/32                 84   20084 Node       R:0 N:1 P:1 E:0 V:0 L:0      Ericsson_84_R6678 L2    node        SPF         
   10.0.0.120/32               120   20120 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node        SPF         
   10.0.0.120/32              1248   21248 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node        MIN-LATENCY 
   10.0.0.120/32              1249   21249 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected MIN-TE      
   10.0.0.120/32              1250   21250 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected ADMIN       
   10.0.0.131/32               131   20131 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-131-JCNR L2    node        SPF         
   10.0.0.156/32               156   20156 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    unprotected SPF         
   10.0.0.156/32              1284   21284 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    unprotected MIN-LATENCY 
   10.0.0.156/32              1285   21285 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    unprotected MIN-TE      
   10.0.0.156/32              1286   21286 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    unprotected ADMIN       
   10.0.0.175/32               175   20175 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected SPF         
   10.0.0.175/32              1303   21303 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        MIN-LATENCY 
   10.0.0.175/32              1304   21304 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected MIN-TE      
   10.0.0.175/32              1305   21305 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        ADMIN       
   10.0.0.179/32               179   20179 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        SPF         
   10.0.0.179/32              1307   21307 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        MIN-LATENCY 
   10.0.0.179/32              1308   21308 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        MIN-TE      
   10.0.0.179/32              1309   21309 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        ADMIN       
   10.0.0.214/32               214   20214 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node        SPF         
   10.0.0.217/32               217   20217 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        SPF         
   10.0.0.217/32              1345   21345 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        MIN-LATENCY 
   10.0.0.217/32              1346   21346 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        MIN-TE      
   10.0.0.217/32              1347   21347 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        ADMIN       
   10.0.0.221/32               221  720221 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node        SPF         
   10.0.0.221/32              1349  721349 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node        MIN-LATENCY 
   10.0.0.221/32              1350  721350 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node        MIN-TE      
*  2002::30/128                430   20430 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected SPF         
*  2002::30/128                558   20558 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-LATENCY 
*  2002::30/128                559   20559 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-TE      
*  2002::30/128                560   20560 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected ADMIN       
   2002::53/128                453   20453 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    unprotected SPF         
   2002::53/128               1581   21581 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    unprotected MIN-LATENCY 
   2002::53/128               1582   21582 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    unprotected MIN-TE      
   2002::53/128               1583   21583 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    unprotected ADMIN       
   2002::120/128               520   20520 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node        SPF         
   2002::120/128              1648   21648 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected MIN-LATENCY 
   2002::120/128              1649   21649 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected MIN-TE      
   2002::120/128              1650   21650 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected ADMIN       
   2002::156/128               556   20556 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        SPF         
   2002::156/128              1684   21684 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        MIN-LATENCY 
   2002::156/128              1685   21685 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        MIN-TE      
   2002::156/128              1686   21686 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        ADMIN       
   2002::175/128               575   20575 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected SPF         
   2002::175/128              1703   21703 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected MIN-LATENCY 
   2002::175/128              1704   21704 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected MIN-TE      
   2002::175/128              1705   21705 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        ADMIN       
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
 I L2     10.0.0.32/32 [115/1]
           via 20.30.32.32, Ethernet2
 I L2     10.0.0.53/32 [115/21]
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.156.156, Ethernet11
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.66.66, Ethernet31
           via 20.30.131.131, Ethernet35
 I L2     10.0.0.66/32 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.72/32 [115/11]
           via 20.30.72.72, Ethernet9
 I L2     10.0.0.84/32 [115/11]
           via 20.30.84.84, Ethernet12
 I L2     10.0.0.120/32 [115/1]
           via 20.30.120.120, Ethernet3
 I L2     10.0.0.124/32 [115/1]
           via 20.30.124.124, Ethernet17
           via 21.30.124.124, Ethernet18
 I L2     10.0.0.128/32 [115/1]
           via 20.30.128.128, Ethernet19
           via 21.30.128.128, Ethernet20
 I L2     10.0.0.131/32 [115/1]
           via 20.30.131.131, Ethernet35
 I L2     10.0.0.156/32 [115/1]
           via 20.30.156.156, Ethernet11
           via 21.30.156.156, Ethernet21
 I L2     10.0.0.175/32 [115/11]
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.156.156, Ethernet11
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.66.66, Ethernet31
           via 20.30.131.131, Ethernet35
 I L2     10.0.0.179/32 [115/1]
           via 20.30.179.179, Ethernet40
 I L2     10.0.0.214/32 [115/1]
           via 20.30.214.214, Ethernet5
 I L2     10.0.0.216/32 [115/11]
           via 20.30.214.214, Ethernet5
 I L2     10.0.0.217/32 [115/1]
           via 20.30.217.217, Ethernet4
 I L2     10.0.0.221/32 [115/1]
           via 20.30.221.221, Ethernet15
 I L2     10.0.1.179/32 [115/1]
           via 20.30.179.179, Ethernet40
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
 C        20.30.124.0/24
           directly connected, Ethernet17
 C        20.30.128.0/24
           directly connected, Ethernet19
 C        20.30.131.0/24
           directly connected, Ethernet35
 C        20.30.156.0/24
           directly connected, Ethernet11
 C        20.30.179.0/24
           directly connected, Ethernet40
 C        20.30.184.0/24
           directly connected, Ethernet7
 C        20.30.214.0/24
           directly connected, Ethernet5
 C        20.30.217.0/24
           directly connected, Ethernet4
 C        20.30.221.0/24
           directly connected, Ethernet15
 I L2     20.32.175.0/24 [115/11]
           via 20.30.32.32, Ethernet2
 I L2     20.53.175.0/24 [115/21]
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.156.156, Ethernet11
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.66.66, Ethernet31
           via 20.30.131.131, Ethernet35
 I L2     20.66.175.0/24 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     20.72.175.0/24 [115/11]
           via 20.30.72.72, Ethernet9
 I L2     20.84.175.0/24 [115/21]
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.156.156, Ethernet11
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.66.66, Ethernet31
           via 20.30.131.131, Ethernet35
 I L2     20.120.175.0/24 [115/11]
           via 20.30.120.120, Ethernet3
 I L2     20.120.214.0/24 [115/11]
           via 20.30.120.120, Ethernet3
 I L2     20.120.217.0/24 [115/1]
           via 20.30.120.120, Ethernet3
 I L2     20.124.175.0/24 [115/11]
           via 20.30.124.124, Ethernet17
           via 21.30.124.124, Ethernet18
 I L2     20.128.175.0/24 [115/11]
           via 20.30.128.128, Ethernet19
           via 21.30.128.128, Ethernet20
 I L2     20.131.175.0/24 [115/11]
           via 20.30.131.131, Ethernet35
 I L2     20.156.175.0/24 [115/11]
           via 20.30.156.156, Ethernet11
           via 21.30.156.156, Ethernet21
 I L2     20.175.179.0/24 [115/11]
           via 20.30.179.179, Ethernet40
 I L2     20.175.184.0/24 [115/21]
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.156.156, Ethernet11
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.66.66, Ethernet31
           via 20.30.131.131, Ethernet35
 I L2     20.175.214.0/24 [115/21]
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.156.156, Ethernet11
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.66.66, Ethernet31
           via 20.30.131.131, Ethernet35
 I L2     20.175.217.0/24 [115/11]
           via 20.30.217.217, Ethernet4
 I L2     20.175.221.0/24 [115/11]
           via 20.30.221.221, Ethernet15
 I L2     20.214.216.0/24 [115/11]
           via 20.30.214.214, Ethernet5
 C        21.30.124.0/24
           directly connected, Ethernet18
 C        21.30.128.0/24
           directly connected, Ethernet20
 C        21.30.156.0/24
           directly connected, Ethernet21
 C        21.30.217.0/24
           directly connected, Ethernet8
 I L2     192.168.20.0/23 [115/1]
           via 20.30.120.120, Ethernet3


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
 B I      50.128.32.0/24 [200/0]
           via 10.0.0.32/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 46, label 378530
              via TI-LFA tunnel index 22, label imp-null(3)
                 via 20.30.32.32, Ethernet2, label imp-null(3)
                 backup via 20.30.221.221, Ethernet15, label 721303 20161
 B I      50.128.53.0/24 [200/0]
           via 10.0.0.53/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 8, label 970002
              via TI-LFA tunnel index 17, label imp-null(3)
                 via 20.30.221.221, Ethernet15, label 721181
                 backup via 20.30.217.217, Ethernet4, label 524283 21181
 B I      50.128.120.0/24 [200/0]
           via 10.0.0.120/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 51, label 1278
              via TI-LFA tunnel index 14, label imp-null(3)
                 via 20.30.221.221, Ethernet15, label 721248
                 backup via 20.30.217.217, Ethernet4, label 524283 21248
 B I      50.128.156.0/24 [200/0]
           via 10.0.0.156/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 14, label 17
              via 20.30.156.156, Ethernet11, label imp-null(3)
              via 21.30.156.156, Ethernet21, label imp-null(3)
 B I      50.128.179.0/24 [200/0]
           via 10.0.0.179/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 15, label 21
              via TI-LFA tunnel index 19, label imp-null(3)
                 via 20.30.179.179, Ethernet40, label imp-null(3)
                 backup via 20.30.221.221, Ethernet15, label 721303 21307
 B I      50.128.217.0/24 [200/0]
           via 10.0.0.217/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 41, label 524284
              via TI-LFA tunnel index 15, label 21345
                 via 20.30.217.217, Ethernet4, label imp-null(3)
                 backup via 20.30.221.221, Ethernet15, label 721303
 B I      50.129.32.0/24 [200/0]
           via 10.0.0.32/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 47, label 378530
              via TI-LFA tunnel index 25, label imp-null(3)
                 via 20.30.32.32, Ethernet2, label imp-null(3)
                 backup via 20.30.217.217, Ethernet4, label 20162
 B I      50.129.53.0/24 [200/0]
           via 10.0.0.53/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 3, label 970002
              via 20.30.32.32, Ethernet2, label 21182
              via 20.30.156.156, Ethernet11, label 21182
              via 20.30.179.179, Ethernet40, label 21182
              via 20.30.217.217, Ethernet4, label 21182
              via 20.30.221.221, Ethernet15, label 721182
              via 21.30.156.156, Ethernet21, label 21182
 B I      50.129.120.0/24 [200/0]
           via 10.0.0.120/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 52, label 1277
              via 20.30.32.32, Ethernet2, label 21249
              via 20.30.156.156, Ethernet11, label 21249
              via 20.30.179.179, Ethernet40, label 21249
              via 20.30.217.217, Ethernet4, label 21249
              via 20.30.221.221, Ethernet15, label 721249
              via 21.30.156.156, Ethernet21, label 21249
 B I      50.129.156.0/24 [200/0]
           via 10.0.0.156/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 6, label 17
              via 20.30.156.156, Ethernet11, label imp-null(3)
              via 21.30.156.156, Ethernet21, label imp-null(3)
 B I      50.129.179.0/24 [200/0]
           via 10.0.0.179/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 9, label 21
              via TI-LFA tunnel index 21, label imp-null(3)
                 via 20.30.179.179, Ethernet40, label imp-null(3)
                 backup via 21.30.156.156, Ethernet21, label 21308
 B I      50.129.217.0/24 [200/0]
           via 10.0.0.217/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 39, label 524284
              via TI-LFA tunnel index 0, label 21346
                 via 20.30.217.217, Ethernet4, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label imp-null(3)
 B I      50.129.221.0/24 [200/0]
           via 10.0.0.221/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 12, label 524293
              via TI-LFA tunnel index 16, label imp-null(3)
                 via 20.30.221.221, Ethernet15, label imp-null(3)
                 backup via 20.30.217.217, Ethernet4, label 21350
 B I      50.130.32.0/24 [200/0]
           via 10.0.0.32/32, algorithm ADMIN, IS-IS FlexAlgo tunnel index 48, label 378530
              via 20.30.32.32, Ethernet2, label imp-null(3)
 B I      50.130.53.0/24 [200/0]
           via 10.0.0.53/32, IS-IS SR tunnel index 10, label 970002
              via 20.30.32.32, Ethernet2, label 20053
              via 20.30.66.66, Ethernet31, label 20053
              via 20.30.72.72, Ethernet9, label 20053
              via 20.30.120.120, Ethernet3, label 20053
              via 20.30.131.131, Ethernet35, label 20053
              via 20.30.156.156, Ethernet11, label 20053
 B I      50.130.120.0/24 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 17, label 1276
              via 20.30.120.120, Ethernet3, label imp-null(3)
 B I      50.130.156.0/24 [200/0]
           via 10.0.0.156/32, algorithm ADMIN, IS-IS FlexAlgo tunnel index 37, label 17
              via 20.30.156.156, Ethernet11, label imp-null(3)
              via 21.30.156.156, Ethernet21, label imp-null(3)
 B I      50.130.179.0/24 [200/0]
           via 10.0.0.179/32, algorithm ADMIN, IS-IS FlexAlgo tunnel index 34, label 21
              via 20.30.179.179, Ethernet40, label imp-null(3)
 B I      50.130.217.0/24 [200/0]
           via 10.0.0.217/32, algorithm ADMIN, IS-IS FlexAlgo tunnel index 40, label 524284
              via 20.30.217.217, Ethernet4, label 21347


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
 B I      50.10.32.0/24 [200/0]
           via 10.0.0.32/32, IS-IS SR tunnel index 20, label 378528
              via TI-LFA tunnel index 11, label imp-null(3)
                 via 20.30.32.32, Ethernet2, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label 20032
 B I      50.10.53.0/24 [200/0]
           via 10.0.0.53/32, IS-IS SR tunnel index 10, label 970000
              via 20.30.32.32, Ethernet2, label 20053
              via 20.30.66.66, Ethernet31, label 20053
              via 20.30.72.72, Ethernet9, label 20053
              via 20.30.120.120, Ethernet3, label 20053
              via 20.30.131.131, Ethernet35, label 20053
              via 20.30.156.156, Ethernet11, label 20053
 B I      50.10.66.0/24 [200/0]
           via 10.0.0.66/32, IS-IS SR tunnel index 13, label 62000
              via TI-LFA tunnel index 7, label imp-null(3)
                 via 20.30.66.66, Ethernet31, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label 20066
 B I      50.10.72.0/24 [200/0]
           via 10.0.0.72/32, IS-IS SR tunnel index 14, label 62000
              via TI-LFA tunnel index 2, label imp-null(3)
                 via 20.30.72.72, Ethernet9, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label 20072
 B I      50.10.84.0/24 [200/0]
           via 10.0.0.84/32, IS-IS SR tunnel index 8, label 720898
              via TI-LFA tunnel index 8, label 20084
                 via 20.30.84.84, Ethernet12, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label imp-null(3)
 B I      50.10.120.0/24 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 17, label 1279
              via 20.30.120.120, Ethernet3, label imp-null(3)
 B I      50.10.131.0/24 [200/0]
           via 10.0.0.131/32, IS-IS SR tunnel index 9, label 18
              via TI-LFA tunnel index 3, label imp-null(3)
                 via 20.30.131.131, Ethernet35, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label 20131
 B I      50.10.156.0/24 [200/0]
           via 10.0.0.156/32, IS-IS SR tunnel index 11, label 16
              via 20.30.156.156, Ethernet11, label imp-null(3)
              via 21.30.156.156, Ethernet21, label imp-null(3)
 B I      50.10.179.0/24 [200/0]
           via 10.0.0.179/32, IS-IS SR tunnel index 12, label 16
              via 20.30.179.179, Ethernet40, label imp-null(3)
 B I      50.10.214.0/24 [200/0]
           via 10.0.0.214/32, IS-IS SR tunnel index 21, label 500000
              via TI-LFA tunnel index 4, label 20214
                 via 20.30.214.214, Ethernet5, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label imp-null(3)
 B I      50.10.217.0/24 [200/0]
           via 10.0.0.217/32, IS-IS SR tunnel index 16, label 524287
              via TI-LFA tunnel index 0, label 20217
                 via 20.30.217.217, Ethernet4, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label imp-null(3)
 B I      50.10.221.0/24 [200/0]
           via 10.0.0.221/32, IS-IS SR tunnel index 15, label 524292
              via TI-LFA tunnel index 6, label imp-null(3)
                 via 20.30.221.221, Ethernet15, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label 20221
 B I      50.129.66.0/24 [200/0]
           via 10.0.0.66/32, IS-IS SR tunnel index 13, label 62000
              via TI-LFA tunnel index 7, label imp-null(3)
                 via 20.30.66.66, Ethernet31, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label 20066
 B I      50.129.72.0/24 [200/0]
           via 10.0.0.72/32, IS-IS SR tunnel index 14, label 62000
              via TI-LFA tunnel index 2, label imp-null(3)
                 via 20.30.72.72, Ethernet9, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label 20072


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
Displaying 40 of 57 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 I L2     2000::214/128 [115/30]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
           via fe80::c214:b8ff:fe21:9790, Ethernet4
           via fe80::d248:a1ff:feba:3c61, Ethernet11
           via fe80::5a70:7fff:fe9f:c403, Ethernet12
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
 C        2001:0:30:124::/64 [0/0]
           via Ethernet17, directly connected
 C        2001:0:30:128::/64 [0/0]
           via Ethernet19, directly connected
 C        2001:0:30:131::/64 [0/0]
           via Ethernet35, directly connected
 C        2001:0:30:156::/64 [0/0]
           via Ethernet11, directly connected
 C        2001:0:30:179::/64 [0/0]
           via Ethernet40, directly connected
 C        2001:0:30:184::/64 [0/0]
           via Ethernet7, directly connected
 C        2001:0:30:214::/64 [0/0]
           via Ethernet5, directly connected
 C        2001:0:30:217::/64 [0/0]
           via Ethernet4, directly connected
 C        2001:0:30:221::/64 [0/0]
           via Ethernet15, directly connected
 I L2     2001:0:32:175::/64 [115/20]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2
 I L2     2001:0:53:175::/64 [115/30]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
           via fe80::c214:b8ff:fe21:9790, Ethernet4
           via fe80::d248:a1ff:feba:3c61, Ethernet11
           via fe80::5a70:7fff:fe9f:c403, Ethernet12
 I L2     2001:0:66:175::/64 [115/30]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
           via fe80::c214:b8ff:fe21:9790, Ethernet4
           via fe80::d248:a1ff:feba:3c61, Ethernet11
           via fe80::5a70:7fff:fe9f:c403, Ethernet12
 I L2     2001:0:72:175::/64 [115/30]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
           via fe80::c214:b8ff:fe21:9790, Ethernet4
           via fe80::d248:a1ff:feba:3c61, Ethernet11
           via fe80::5a70:7fff:fe9f:c403, Ethernet12
 I L2     2001:0:84:175::/64 [115/20]
           via fe80::5a70:7fff:fe9f:c403, Ethernet12
 I L2     2001:0:120:175::/64 [115/20]
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
 I L2     2001:0:120:214::/64 [115/20]
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
 I L2     2001:0:120:217::/64 [115/10]
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
 I L2     2001:0:128:175::/64 [115/30]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
           via fe80::c214:b8ff:fe21:9790, Ethernet4
           via fe80::d248:a1ff:feba:3c61, Ethernet11
           via fe80::5a70:7fff:fe9f:c403, Ethernet12
 I L2     2001:0:131:175::/64 [115/30]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
           via fe80::c214:b8ff:fe21:9790, Ethernet4
           via fe80::d248:a1ff:feba:3c61, Ethernet11
           via fe80::5a70:7fff:fe9f:c403, Ethernet12
 I L2     2001:0:156:175::/64 [115/20]
           via fe80::d248:a1ff:feba:3c61, Ethernet11
 I L2     2001:0:175::/64 [115/30]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
           via fe80::c214:b8ff:fe21:9790, Ethernet4
           via fe80::d248:a1ff:feba:3c61, Ethernet11
           via fe80::5a70:7fff:fe9f:c403, Ethernet12
 I L2     2001:0:175:184::/64 [115/30]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
           via fe80::c214:b8ff:fe21:9790, Ethernet4
           via fe80::d248:a1ff:feba:3c61, Ethernet11
           via fe80::5a70:7fff:fe9f:c403, Ethernet12
 I L2     2001:0:175:214::/64 [115/30]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
           via fe80::c214:b8ff:fe21:9790, Ethernet4
           via fe80::d248:a1ff:feba:3c61, Ethernet11
           via fe80::5a70:7fff:fe9f:c403, Ethernet12
 I L2     2001:0:175:217::/64 [115/20]
           via fe80::c214:b8ff:fe21:9790, Ethernet4
 I L2     2001:0:175:221::/64 [115/30]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
           via fe80::c214:b8ff:fe21:9790, Ethernet4
           via fe80::d248:a1ff:feba:3c61, Ethernet11
           via fe80::5a70:7fff:fe9f:c403, Ethernet12
 I L2     2001:0:214:216::/64 [115/40]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
           via fe80::c214:b8ff:fe21:9790, Ethernet4
           via fe80::d248:a1ff:feba:3c61, Ethernet11
           via fe80::5a70:7fff:fe9f:c403, Ethernet12
 C        2002::30/128 [0/0]
           via Loopback0, directly connected
 I L2     2002::32/128 [115/20]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2
 I L2     2002::53/128 [115/30]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
           via fe80::c214:b8ff:fe21:9790, Ethernet4
           via fe80::d248:a1ff:feba:3c61, Ethernet11
           via fe80::5a70:7fff:fe9f:c403, Ethernet12
 I L2     2002::120/128 [115/10]
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
 I L2     2002::156/128 [115/10]
           via fe80::d248:a1ff:feba:3c61, Ethernet11
 I L2     2002::175/128 [115/20]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
           via fe80::c214:b8ff:fe21:9790, Ethernet4
           via fe80::d248:a1ff:feba:3c61, Ethernet11
           via fe80::5a70:7fff:fe9f:c403, Ethernet12
 I L2     2002::216/128 [115/40]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
           via fe80::c214:b8ff:fe21:9790, Ethernet4
           via fe80::d248:a1ff:feba:3c61, Ethernet11
           via fe80::5a70:7fff:fe9f:c403, Ethernet12
 I L2     2002::217/128 [115/10]
           via fe80::c214:b8ff:fe21:9790, Ethernet4

```

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 66 routes 
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

 20032   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 11
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20032
 20053   A[1]
                via M, 20.30.32.32, swap 20053
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1018
                via M, 20.30.66.66, swap 20053
                    EgressACL: apply
                    directly connected, Ethernet31
                    e4:6d:7f:e3:c8:0a, vlan 1020
                via M, 20.30.72.72, swap 20053
                    EgressACL: apply
                    directly connected, Ethernet9
                    e0:9b:27:c4:c5:84, vlan 1009
                via M, 20.30.120.120, swap 20053
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1017
                via M, 20.30.131.131, swap 20053
                    EgressACL: apply
                    directly connected, Ethernet35
                    40:a6:b7:94:34:cb, vlan 1012
                via M, 20.30.156.156, swap 20053
                    EgressACL: apply
                    directly connected, Ethernet11
                    d0:48:a1:ba:3c:61, vlan 1019
 20066   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 7
                    via 20.30.66.66, Ethernet31, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20066
 20072   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 2
                    via 20.30.72.72, Ethernet9, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20072
 20084   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 8
                    via 20.30.84.84, Ethernet12, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label imp-null(3)
 20120   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.120.120 Ethernet3
 20131   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 3
                    via 20.30.131.131, Ethernet35, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20131
 20156   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.156.156 Ethernet11
                    21.30.156.156 Ethernet21
 20161   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 22
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 20161
 20162   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 25
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.217.217, Ethernet4, label 20162
 20163   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.32.32 Ethernet2
 20175   A[1]
                via M, 20.30.32.32, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1018
                via M, 20.30.66.66, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet31
                    e4:6d:7f:e3:c8:0a, vlan 1020
                via M, 20.30.72.72, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet9
                    e0:9b:27:c4:c5:84, vlan 1009
                via M, 20.30.120.120, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1017
                via M, 20.30.131.131, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet35
                    40:a6:b7:94:34:cb, vlan 1012
                via M, 20.30.156.156, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet11
                    d0:48:a1:ba:3c:61, vlan 1019
 20179   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.179.179 Ethernet40
 20214   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 4
                    via 20.30.214.214, Ethernet5, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label imp-null(3)
 20217   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label imp-null(3)
 20221   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 6
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20221
 20453   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::d248:a1ff:feba:3c61 Ethernet11
                    fe80::c214:b8ff:fe21:9790 Ethernet4
                    fe80::5a70:7fff:fe9f:c403 Ethernet12
                    fe80::d6af:f7ff:fe2f:1396 Ethernet2
                    fe80::be31:e2ff:fee1:ec2c Ethernet3
 20520   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::be31:e2ff:fee1:ec2c Ethernet3
 20556   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 10
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::d6af:f7ff:fe2f:1396, Ethernet2, label 20575 20556
 20575   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::d248:a1ff:feba:3c61 Ethernet11
                    fe80::c214:b8ff:fe21:9790 Ethernet4
                    fe80::5a70:7fff:fe9f:c403 Ethernet12
                    fe80::d6af:f7ff:fe2f:1396 Ethernet2
                    fe80::be31:e2ff:fee1:ec2c Ethernet3
 21181   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 17
                    via 20.30.221.221, Ethernet15, label 721181
                    backup via 20.30.217.217, Ethernet4, label 524283 21181
 21182   A[1]
                via M, 20.30.32.32, swap 21182
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1018
                via M, 20.30.156.156, swap 21182
                    EgressACL: apply
                    directly connected, Ethernet11
                    d0:48:a1:ba:3c:61, vlan 1019
                via M, 20.30.179.179, swap 21182
                    EgressACL: apply
                    directly connected, Ethernet40
                    e8:24:a6:96:05:48, vlan 1015
                via M, 20.30.217.217, swap 21182
                    EgressACL: apply
                    directly connected, Ethernet4
                    c0:14:b8:21:97:90, vlan 1007
                via M, 20.30.221.221, swap 721182
                    EgressACL: apply
                    directly connected, Ethernet15
                    30:c5:07:84:3e:79, vlan 1006
                via M, 21.30.156.156, swap 21182
                    EgressACL: apply
                    directly connected, Ethernet21
                    d0:48:a1:ba:3c:63, vlan 1027
 21248   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 14
                    via 20.30.221.221, Ethernet15, label 721248
                    backup via 20.30.217.217, Ethernet4, label 524283 21248
 21249   A[1]
                via M, 20.30.32.32, swap 21249
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1018
                via M, 20.30.156.156, swap 21249
                    EgressACL: apply
                    directly connected, Ethernet11
                    d0:48:a1:ba:3c:61, vlan 1019
                via M, 20.30.179.179, swap 21249
                    EgressACL: apply
                    directly connected, Ethernet40
                    e8:24:a6:96:05:48, vlan 1015
                via M, 20.30.217.217, swap 21249
                    EgressACL: apply
                    directly connected, Ethernet4
                    c0:14:b8:21:97:90, vlan 1007
                via M, 20.30.221.221, swap 721249
                    EgressACL: apply
                    directly connected, Ethernet15
                    30:c5:07:84:3e:79, vlan 1006
                via M, 21.30.156.156, swap 21249
                    EgressACL: apply
                    directly connected, Ethernet21
                    d0:48:a1:ba:3c:63, vlan 1027
 21284   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.156.156 Ethernet11
                    21.30.156.156 Ethernet21
 21285   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.156.156 Ethernet11
                    21.30.156.156 Ethernet21
 21286   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.156.156 Ethernet11
                    21.30.156.156 Ethernet21
 21303   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 18
                    via 20.30.221.221, Ethernet15, label 721303
                    backup via 20.30.217.217, Ethernet4, label 524283
 21304   A[1]
                via M, 20.30.32.32, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1018
                via M, 20.30.156.156, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet11
                    d0:48:a1:ba:3c:61, vlan 1019
                via M, 20.30.179.179, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet40
                    e8:24:a6:96:05:48, vlan 1015
                via M, 20.30.217.217, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet4
                    c0:14:b8:21:97:90, vlan 1007
                via M, 20.30.221.221, swap 721304
                    EgressACL: apply
                    directly connected, Ethernet15
                    30:c5:07:84:3e:79, vlan 1006
                via M, 21.30.156.156, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet21
                    d0:48:a1:ba:3c:63, vlan 1027
 21305   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.131.131 Ethernet35
 21307   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 19
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 21307
 21308   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 21
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 21.30.156.156, Ethernet21, label 21308
 21309   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.179.179 Ethernet40
 21345   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 15
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303
 21346   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label imp-null(3)
 21347   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.217.217 Ethernet4
 21349   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 13
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.124.124, Ethernet17, label 404 21349
 21350   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 16
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.217.217, Ethernet4, label 21350
 21581   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::d248:a1ff:feba:3c61 Ethernet11
                    fe80::d6af:f7ff:fe2f:1396 Ethernet2
 21582   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::d248:a1ff:feba:3c61 Ethernet11
                    fe80::d6af:f7ff:fe2f:1396 Ethernet2
 21684   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 5
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::d6af:f7ff:fe2f:1396, Ethernet2, label 21703 21684
 21685   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 27
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::d6af:f7ff:fe2f:1396, Ethernet2, label 21685
 21686   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::d248:a1ff:feba:3c61 Ethernet11
 21703   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::d248:a1ff:feba:3c61 Ethernet11
                    fe80::d6af:f7ff:fe2f:1396 Ethernet2
 21704   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::d248:a1ff:feba:3c61 Ethernet11
                    fe80::d6af:f7ff:fe2f:1396 Ethernet2
 21705   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::c214:b8ff:fe21:9790 Ethernet4
 362144   [0]
                via I, ipv4, vrf FLEXALGO
 362145   [0]
                via I, ipv4, vrf RED
 362146   [0]
                via I, ipv6, vrf RED
 378533  A[1]
                via M, 20.30.131.131, pop
                    EgressACL: apply
                    directly connected, Ethernet35
                    40:a6:b7:94:34:cb, vlan 1012
 378538  A[1]
                via M, 20.30.179.179, pop
                    EgressACL: apply
                    directly connected, Ethernet40
                    e8:24:a6:96:05:48, vlan 1015
 378540  A[1]
                via M, 20.30.156.156, pop
                    EgressACL: apply
                    directly connected, Ethernet11
                    d0:48:a1:ba:3c:61, vlan 1019
 378541  A[1]
                via M, fe80::d248:a1ff:feba:3c61, pop
                    EgressACL: apply
                    directly connected, Ethernet11
                    d0:48:a1:ba:3c:61, vlan 1019
 378542  A[1]
                via M, 20.30.221.221, pop
                    EgressACL: apply
                    directly connected, Ethernet15
                    30:c5:07:84:3e:79, vlan 1006
 378553  A[1]
                via M, 20.30.214.214, pop
                    EgressACL: apply
                    directly connected, Ethernet5
                    18:5b:00:61:ac:6f, vlan 1008
 378574  A[1]
                via M, 21.30.156.156, pop
                    EgressACL: apply
                    directly connected, Ethernet21
                    d0:48:a1:ba:3c:63, vlan 1027
 378577  A[1]
                via M, 20.30.72.72, pop
                    EgressACL: apply
                    directly connected, Ethernet9
                    e0:9b:27:c4:c5:84, vlan 1009
 378578  A[1]
                via M, 20.30.66.66, pop
                    EgressACL: apply
                    directly connected, Ethernet31
                    e4:6d:7f:e3:c8:0a, vlan 1020
 378582  A[1]
                via M, 20.30.217.217, pop
                    EgressACL: apply
                    directly connected, Ethernet4
                    c0:14:b8:21:97:90, vlan 1007
 378583  A[1]
                via M, fe80::c214:b8ff:fe21:9790, pop
                    EgressACL: apply
                    directly connected, Ethernet4
                    c0:14:b8:21:97:90, vlan 1007
 378586  A[1]
                via M, 20.30.84.84, pop
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1014
 378587  A[1]
                via M, fe80::5a70:7fff:fe9f:c403, pop
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1014
 378588  A[1]
                via M, 20.30.32.32, pop
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1018
 378589  A[1]
                via M, fe80::d6af:f7ff:fe2f:1396, pop
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1018
 378597  A[1]
                via M, 20.30.120.120, pop
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1017
 378598  A[1]
                via M, fe80::be31:e2ff:fee1:ec2c, pop
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1017
```

## show mpls lfib route

```text
MPLS forwarding table (Label [metric] Vias) - 66 routes 
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

 IP    20032    [1], 10.0.0.32/32
                via TI-LFA tunnel index 11, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20032
 IP    20053    [1], 10.0.0.53/32
                via M, 20.30.32.32, swap 20053
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
                via M, 20.30.66.66, swap 20053
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet31
                via M, 20.30.72.72, swap 20053
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet9
                via M, 20.30.120.120, swap 20053
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
                via M, 20.30.131.131, swap 20053
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet35
                via M, 20.30.156.156, swap 20053
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet11
 IP    20066    [1], 10.0.0.66/32
                via TI-LFA tunnel index 7, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.66.66, Ethernet31, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20066
 IP    20072    [1], 10.0.0.72/32
                via TI-LFA tunnel index 2, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.72.72, Ethernet9, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20072
 IP    20084    [1], 10.0.0.84/32
                via TI-LFA tunnel index 8, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.84.84, Ethernet12, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label imp-null(3)
 IP    20120    [1], 10.0.0.120/32
                via M, 20.30.120.120, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet3
 IP    20131    [1], 10.0.0.131/32
                via TI-LFA tunnel index 3, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.131.131, Ethernet35, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20131
 IP    20156    [1], 10.0.0.156/32
                via M, 20.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
                via M, 21.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet21
 IP    20161    [1], 10.0.0.32/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 22, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 20161
 IP    20162    [1], 10.0.0.32/32, algorithm MIN-TE
                via TI-LFA tunnel index 25, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.217.217, Ethernet4, label 20162
 IP    20163    [1], 10.0.0.32/32, algorithm ADMIN
                via M, 20.30.32.32, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet2
 IP    20175    [1], 10.0.0.175/32
                via M, 20.30.32.32, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
                via M, 20.30.66.66, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet31
                via M, 20.30.72.72, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet9
                via M, 20.30.120.120, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
                via M, 20.30.131.131, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet35
                via M, 20.30.156.156, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet11
 IP    20179    [1], 10.0.0.179/32
                via M, 20.30.179.179, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet40
 IP    20214    [1], 10.0.0.214/32
                via TI-LFA tunnel index 4, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.214.214, Ethernet5, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label imp-null(3)
 IP    20217    [1], 10.0.0.217/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label imp-null(3)
 IP    20221    [1], 10.0.0.221/32
                via TI-LFA tunnel index 6, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20221
 IP    20453    [1], 2002::53/128
                via M, fe80::5a70:7fff:fe9f:c403, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet12
                via M, fe80::be31:e2ff:fee1:ec2c, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet3
                via M, fe80::c214:b8ff:fe21:9790, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet4
                via M, fe80::d248:a1ff:feba:3c61, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
                via M, fe80::d6af:f7ff:fe2f:1396, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet2
 IP    20520    [1], 2002::120/128
                via M, fe80::be31:e2ff:fee1:ec2c, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet3
 IP    20556    [1], 2002::156/128
                via TI-LFA tunnel index 10, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::d6af:f7ff:fe2f:1396, Ethernet2, label 20575 20556
 IP    20575    [1], 2002::175/128
                via M, fe80::5a70:7fff:fe9f:c403, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet12
                via M, fe80::be31:e2ff:fee1:ec2c, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet3
                via M, fe80::c214:b8ff:fe21:9790, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet4
                via M, fe80::d248:a1ff:feba:3c61, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
                via M, fe80::d6af:f7ff:fe2f:1396, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet2
 IP    21181    [1], 10.0.0.53/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 17, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.221.221, Ethernet15, label 721181
                    backup via 20.30.217.217, Ethernet4, label 524283 21181
 IP    21182    [1], 10.0.0.53/32, algorithm MIN-TE
                via M, 20.30.32.32, swap 21182
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
                via M, 20.30.156.156, swap 21182
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet11
                via M, 20.30.179.179, swap 21182
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet40
                via M, 20.30.217.217, swap 21182
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet4
                via M, 20.30.221.221, swap 721182
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet15
                via M, 21.30.156.156, swap 21182
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet21
 IP    21248    [1], 10.0.0.120/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 14, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.221.221, Ethernet15, label 721248
                    backup via 20.30.217.217, Ethernet4, label 524283 21248
 IP    21249    [1], 10.0.0.120/32, algorithm MIN-TE
                via M, 20.30.32.32, swap 21249
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
                via M, 20.30.156.156, swap 21249
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet11
                via M, 20.30.179.179, swap 21249
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet40
                via M, 20.30.217.217, swap 21249
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet4
                via M, 20.30.221.221, swap 721249
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet15
                via M, 21.30.156.156, swap 21249
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet21
 IP    21284    [1], 10.0.0.156/32, algorithm MIN-LATENCY
                via M, 20.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
                via M, 21.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet21
 IP    21285    [1], 10.0.0.156/32, algorithm MIN-TE
                via M, 20.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
                via M, 21.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet21
 IP    21286    [1], 10.0.0.156/32, algorithm ADMIN
                via M, 20.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
                via M, 21.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet21
 IP    21303    [1], 10.0.0.175/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 18, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.221.221, Ethernet15, label 721303
                    backup via 20.30.217.217, Ethernet4, label 524283
 IP    21304    [1], 10.0.0.175/32, algorithm MIN-TE
                via M, 20.30.32.32, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
                via M, 20.30.156.156, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet11
                via M, 20.30.179.179, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet40
                via M, 20.30.217.217, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet4
                via M, 20.30.221.221, swap 721304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet15
                via M, 21.30.156.156, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet21
 IP    21305    [1], 10.0.0.175/32, algorithm ADMIN
                via M, 20.30.131.131, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet35
 IP    21307    [1], 10.0.0.179/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 19, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 21307
 IP    21308    [1], 10.0.0.179/32, algorithm MIN-TE
                via TI-LFA tunnel index 21, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 21.30.156.156, Ethernet21, label 21308
 IP    21309    [1], 10.0.0.179/32, algorithm ADMIN
                via M, 20.30.179.179, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet40
 IP    21345    [1], 10.0.0.217/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 15, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303
 IP    21346    [1], 10.0.0.217/32, algorithm MIN-TE
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label imp-null(3)
 IP    21347    [1], 10.0.0.217/32, algorithm ADMIN
                via M, 20.30.217.217, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet4
 IP    21349    [1], 10.0.0.221/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 13, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.124.124, Ethernet17, label 404 21349
 IP    21350    [1], 10.0.0.221/32, algorithm MIN-TE
                via TI-LFA tunnel index 16, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.217.217, Ethernet4, label 21350
 IP    21581    [1], 2002::53/128, algorithm MIN-LATENCY
                via M, fe80::d248:a1ff:feba:3c61, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
                via M, fe80::d6af:f7ff:fe2f:1396, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet2
 IP    21582    [1], 2002::53/128, algorithm MIN-TE
                via M, fe80::d248:a1ff:feba:3c61, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
                via M, fe80::d6af:f7ff:fe2f:1396, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet2
 IP    21684    [1], 2002::156/128, algorithm MIN-LATENCY
                via TI-LFA tunnel index 5, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::d6af:f7ff:fe2f:1396, Ethernet2, label 21703 21684
 IP    21685    [1], 2002::156/128, algorithm MIN-TE
                via TI-LFA tunnel index 27, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::d6af:f7ff:fe2f:1396, Ethernet2, label 21685
 IP    21686    [1], 2002::156/128, algorithm ADMIN
                via M, fe80::d248:a1ff:feba:3c61, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
 IP    21703    [1], 2002::175/128, algorithm MIN-LATENCY
                via M, fe80::d248:a1ff:feba:3c61, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
                via M, fe80::d6af:f7ff:fe2f:1396, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet2
 IP    21704    [1], 2002::175/128, algorithm MIN-TE
                via M, fe80::d248:a1ff:feba:3c61, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
                via M, fe80::d6af:f7ff:fe2f:1396, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet2
 IP    21705    [1], 2002::175/128, algorithm ADMIN
                via M, fe80::c214:b8ff:fe21:9790, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet4
 B3    362144   [0]
                via I, ipv4, vrf FLEXALGO
 B3    362145   [0]
                via I, ipv4, vrf RED
 B3    362146   [0]
                via I, ipv6, vrf RED
 IA    378533   [1]
                via M, 20.30.131.131, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet35
 IA    378538   [1]
                via M, 20.30.179.179, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet40
 IA    378540   [1]
                via M, 20.30.156.156, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet11
 IA    378541   [1]
                via M, fe80::d248:a1ff:feba:3c61, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet11
 IA    378542   [1]
                via M, 20.30.221.221, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet15
 IA    378553   [1]
                via M, 20.30.214.214, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet5
 IA    378574   [1]
                via M, 21.30.156.156, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet21
 IA    378577   [1]
                via M, 20.30.72.72, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet9
 IA    378578   [1]
                via M, 20.30.66.66, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet31
 IA    378582   [1]
                via M, 20.30.217.217, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet4
 IA    378583   [1]
                via M, fe80::c214:b8ff:fe21:9790, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet4
 IA    378586   [1]
                via M, 20.30.84.84, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet12
 IA    378587   [1]
                via M, fe80::5a70:7fff:fe9f:c403, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet12
 IA    378588   [1]
                via M, 20.30.32.32, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
 IA    378589   [1]
                via M, fe80::d6af:f7ff:fe2f:1396, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
 IA    378597   [1]
                via M, 20.30.120.120, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
 IA    378598   [1]
                via M, fe80::be31:e2ff:fee1:ec2c, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
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
 * >      RD: 10.0.0.32:5001 IPv4 prefix 50.10.32.0/24
                                 10.0.0.32             -       100     0       i
 * >      RD: 53:5001 IPv4 prefix 50.10.53.0/24
                                 10.0.0.53             -       100     0       ?
 * >      RD: 66:5001 IPv4 prefix 50.10.66.0/24
                                 10.0.0.66             -       100     0       ?
 * >      RD: 72:5001 IPv4 prefix 50.10.72.0/24
                                 10.0.0.72             -       100     0       ?
 * >      RD: 84:5001 IPv4 prefix 50.10.84.0/24
                                 10.0.0.84             0       100     0       ?
 * >      RD: 120:5001 IPv4 prefix 50.10.120.0/24
                                 10.0.0.120            0       100     0       ?
 * >      RD: 131:5001 IPv4 prefix 50.10.131.0/24
                                 10.0.0.131            -       100     0       i
 * >      RD: 156:5001 IPv4 prefix 50.10.156.0/24
                                 10.0.0.156            -       100     0       i
 * >      RD: 179:5001 IPv4 prefix 50.10.179.0/24
                                 10.0.0.179            -       100     0       i
 * >      RD: 214:5001 IPv4 prefix 50.10.214.0/24
                                 10.0.0.214            -       100     0       i
 * >      RD: 217:5001 IPv4 prefix 50.10.217.0/24
                                 10.0.0.217            -       100     0       i
 * >      RD: 221:5001 IPv4 prefix 50.10.221.0/24
                                 10.0.0.221            -       100     0       i
 * >      RD: 10.0.0.30:5128 IPv4 prefix 50.128.32.0/24
                                 10.0.0.32             -       100     0       i
 * >      RD: 53:5128 IPv4 prefix 50.128.53.0/24
                                 10.0.0.53             -       100     0       ?
 * >      RD: 120:5128 IPv4 prefix 50.128.120.0/24
                                 10.0.0.120            0       100     0       ?
 * >      RD: 5128:5128 IPv4 prefix 50.128.156.0/24
                                 10.0.0.156            -       100     0       i
 * >      RD: 5128:5128 IPv4 prefix 50.128.179.0/24
                                 10.0.0.179            -       100     0       i
 * >      RD: 217:5128 IPv4 prefix 50.128.217.0/24
                                 10.0.0.217            -       100     0       i
 * >      RD: 10.0.0.30:5128 IPv4 prefix 50.129.32.0/24
                                 10.0.0.32             -       100     0       i
 * >      RD: 53:5128 IPv4 prefix 50.129.53.0/24
                                 10.0.0.53             -       100     0       ?
 * >      RD: 66:5001 IPv4 prefix 50.129.66.0/24
                                 10.0.0.66             -       100     0       ?
 * >      RD: 72:5001 IPv4 prefix 50.129.72.0/24
                                 10.0.0.72             -       100     0       ?
 * >      RD: 120:5129 IPv4 prefix 50.129.120.0/24
                                 10.0.0.120            0       100     0       ?
 * >      RD: 5128:5128 IPv4 prefix 50.129.156.0/24
                                 10.0.0.156            -       100     0       i
 * >      RD: 5128:5128 IPv4 prefix 50.129.179.0/24
                                 10.0.0.179            -       100     0       i
 * >      RD: 217:5128 IPv4 prefix 50.129.217.0/24
                                 10.0.0.217            -       100     0       i
 * >      RD: 221:5128 IPv4 prefix 50.129.221.0/24
                                 10.0.0.221            -       100     0       i
 * >      RD: 10.0.0.30:5128 IPv4 prefix 50.130.32.0/24
                                 10.0.0.32             -       100     0       i
 * >      RD: 53:5128 IPv4 prefix 50.130.53.0/24
                                 10.0.0.53             -       100     0       ?
 * >      RD: 120:5130 IPv4 prefix 50.130.120.0/24
                                 10.0.0.120            0       100     0       ?
 * >      RD: 5128:5128 IPv4 prefix 50.130.156.0/24
                                 10.0.0.156            -       100     0       i
 * >      RD: 5128:5128 IPv4 prefix 50.130.179.0/24
                                 10.0.0.179            -       100     0       i
 * >      RD: 217:5128 IPv4 prefix 50.130.217.0/24
                                 10.0.0.217            -       100     0       i
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
 * >      RD: 10.0.0.32:5001 IPv6 prefix 2600:50:10:32::/64
                                 ::ffff:10.0.0.32      -       100     0       i
 * >      RD: 84:5001 IPv6 prefix 2600:50:10:84::/64
                                 ::ffff:10.0.0.84      0       100     0       ?
 * >      RD: 131:5001 IPv6 prefix 2600:50:10:131::/64
                                 ::ffff:10.0.0.131     -       100     0       i
 * >      RD: 156:5001 IPv6 prefix 2600:50:10:156::/64
                                 ::ffff:10.0.0.156     -       100     0       i
 * >      RD: 179:5001 IPv6 prefix 2600:50:10:179::/64
                                 ::ffff:10.0.0.179     -       100     0       i
 * >      RD: 214:5001 IPv6 prefix 2600:50:10:214::/64
                                 ::ffff:10.0.0.214     -       100     0       i
 * >      RD: 217:5001 IPv6 prefix 2600:50:10:217::/64
                                 ::ffff:10.0.0.217     -       100     0       i
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
BGP neighbor is 10.0.0.31, remote AS 64512, internal link
 Description: Arista-PE31-Q2C
  BGP version 4, remote router ID 0.0.0.0, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read never, last write never
  Hold time is 0, keepalive interval is 0 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:34
  Connection interval is 148 seconds
  Failed connection attempts is 1856
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Network is unreachable), Last time 00:02:17, First time 3d15h, Repeats 1855
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
Local TCP address is 10.0.0.30
Remote TCP address is 10.0.0.31, remote port is 179

BGP neighbor is 10.0.0.32, remote AS 64512, internal link
 Description: Arista-PE32-Q2C
  BGP version 4, remote router ID 10.0.0.32, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:34, last write 00:00:57
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:26
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 3d15h
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
  Types of communities advertised: standard extended large
  Enhanced route refresh stale path removal disabled
  Outbound enhanced route refresh enabled
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised and received and negotiated
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
      VPN-IPv4: received
      VPN-IPv6: received
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
      VPN-IPv6 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 3d15h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 3d15h
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
    Opens:                           1         1
    Notifications:                   0         0
    Updates:                       134         7
    Keepalives:                   6113      6160
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:               6248      6168
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        29         4              4                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         6         1              1                   0
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
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 39975
Remote TCP address is 10.0.0.32, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
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
    TCP Throughput: 454.27 Mbps
    Recv Round-trip Time (rcv_rtt): 23178.5ms
    Advertised Recv Window (rcv_space): 64347

BGP neighbor is 10.0.0.53, remote AS 64512, internal link
 Description: Arrcus-53
  BGP version 4, remote router ID 10.0.0.53, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:01, last write 00:00:18
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:59
  Keepalive timer is active, time left: 00:00:26
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 3d15h
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvRtRefresh
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 with MPLS Labels: received
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: yes
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
    VPN-IPv4 End-of-RIB received: Yes
      Received 3d15h
      Number of stale paths removed after graceful restart: 0
    VPN-IPv6 End-of-RIB received: Yes
      Received 3d15h
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
    Updates:              171        10
    Keepalives:          6124      5237
    Route Refresh:          0         2
    Total messages:      6296      5250
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        29         4              4                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         7         0              0                   0
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
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 179
Remote TCP address is 10.0.0.53, remote port is 36759
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1436
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 14,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.4ms/0.2ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 295.32 Mbps
    Recv Round-trip Time (rcv_rtt): 459652.8ms
    Advertised Recv Window (rcv_space): 65264

BGP neighbor is 10.0.0.66, remote AS 64512, internal link
 Description: Ciena-8140-66
  BGP version 4, remote router ID 10.0.0.66, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:49, last write 00:00:23
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:11
  Keepalive timer is active, time left: 00:00:19
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 2d17h
  Number of transitions to established: 6
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Hold Timer Expired Error/None, Last time 2d18h, First time 2d22h, Repeats 1
  Last rcvd notification:Cease/other configuration change, Last time 2d17h, First time 3d15h, Repeats 2
  Last sent socket-error:Connect (Connection refused), Last time 2d17h, First time 2d18h, Repeats 8
  Last rcvd socket-error:Connection reset by peer, Last time 2d17h, First time 2d17h, Repeats 1
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised
    Four Octet ASN: advertised
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
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
      Restart-time is 0
      Restart-State bit: no
      Graceful notification: no
      IPv4 Unicast is enabled, Forwarding State is not preserved
      VPN-IPv4 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 2d17h
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
    Opens:                  8         6
    Notifications:          2         3
    Updates:              259        20
    Keepalives:          5926      5051
    Route Refresh:          0         0
    Total messages:      6195      5080
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        31         2              2                   0
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
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
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
Local TCP address is 10.0.0.30, local port is 179
Remote TCP address is 10.0.0.66, remote port is 38163
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1460
  Total Number of TCP retransmissions: 7
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 7,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.4ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 2
    Slow-start Threshold (ssthresh): 7
    TCP Throughput: 52.14 Mbps
    Recv Round-trip Time (rcv_rtt): 39675.6ms
    Advertised Recv Window (rcv_space): 64321

BGP neighbor is 10.0.0.72, remote AS 64512, internal link
 Description: Ciena-5134-72
  BGP version 4, remote router ID 10.0.0.72, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:35, last write 00:00:53
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:25
  Keepalive timer is active, time left: 00:00:04
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 2d17h
  Number of transitions to established: 7
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Hold Timer Expired Error/None, Last time 2d18h, First time 2d23h, Repeats 1
  Last rcvd notification:Cease/other configuration change, Last time 2d17h, First time 3d15h, Repeats 3
  Last sent socket-error:Connect (Connection refused), Last time 2d17h, First time 2d18h, Repeats 7
  Last rcvd socket-error:Connection reset by peer, Last time 2d17h, First time 2d19h, Repeats 4
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised
    Four Octet ASN: advertised
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
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
      Restart-time is 0
      Restart-State bit: no
      Graceful notification: no
      IPv4 Unicast is enabled, Forwarding State is not preserved
      VPN-IPv4 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 2d17h
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
    Opens:                 12         7
    Notifications:          2         4
    Updates:              277        21
    Keepalives:          5913      5048
    Route Refresh:          0         0
    Total messages:      6204      5080
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        31         2              2                   0
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
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
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
Local TCP address is 10.0.0.30, local port is 179
Remote TCP address is 10.0.0.72, remote port is 37843
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
    Round-trip Time (rtt/rtvar): 0.7ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 179.69 Mbps
    Recv Round-trip Time (rcv_rtt): 39674.3ms
    Advertised Recv Window (rcv_space): 64321

BGP neighbor is 10.0.0.84, remote AS 64512, internal link
 Description: Ericsson_84
  BGP version 4, remote router ID 10.0.0.84, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:42, last write 00:00:10
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:18
  Keepalive timer is active, time left: 00:00:41
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 3d15h
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
  Types of communities advertised: standard extended large
  Enhanced route refresh stale path removal disabled
  Outbound enhanced route refresh enabled
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol IPv6 Unicast: received
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Multiprotocol L2VPN EVPN: received
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised and received and negotiated
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: yes
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: no
      IPv4 Unicast is enabled, Forwarding State is preserved
      VPN-IPv4 is enabled, Forwarding State is preserved
      IPv6 Unicast is enabled, Forwarding State is preserved
      VPN-IPv6 is enabled, Forwarding State is preserved
      L2VPN EVPN is enabled, Forwarding State is preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 3d15h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 3d15h
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
    Opens:                           1         1
    Notifications:                   0         0
    Updates:                       145         4
    Keepalives:                   6125      5229
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:               6271      5234
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        32         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         6         1              1                   0
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
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 35281
Remote TCP address is 10.0.0.84, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
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
    Round-trip Time (rtt/rtvar): 232.0ms/0.2ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 0.49 Mbps
    Recv Round-trip Time (rcv_rtt): 519668.6ms
    Advertised Recv Window (rcv_space): 64371

BGP neighbor is 10.0.0.120, remote AS 64512, internal link
 Description: Huawei_120
  BGP version 4, remote router ID 10.0.0.120, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:44, last write 00:00:07
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:16
  Keepalive timer is active, time left: 00:00:52
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 2d14h
  Number of transitions to established: 3
  Last state was OpenConfirm
  Last event was RecvKeepAlive
  Last sent notification:Hold Timer Expired Error/None, Last time 2d14h, First time 2d16h, Repeats 1
  Last sent socket-error:Connect (Network is unreachable), Last time 2d14h, First time 2d14h, Repeats 10
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
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
    VPN-IPv4 End-of-RIB received: No
      Number of stale paths removed after graceful restart: 0
    VPN-IPv6 End-of-RIB received: No
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
    Opens:                  3         4
    Notifications:          3         0
    Updates:              176        26
    Keepalives:          4735      4743
    Route Refresh:          0         2
    Total messages:      4917      4775
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        29         4              4                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         7         0              0                   0
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
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 41969
Remote TCP address is 10.0.0.120, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
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
    TCP Throughput: 324.69 Mbps
    Recv Round-trip Time (rcv_rtt): 379291.5ms
    Advertised Recv Window (rcv_space): 64327

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
  Connect timer is active, time left: 00:01:22
  Connection interval is 148 seconds
  Failed connection attempts is 1360
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Connection refused), Last time 00:01:26, First time 2d22h, Repeats 1509
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
Local TCP address is 10.0.0.30
Remote TCP address is 10.0.0.124, remote port is 179

BGP neighbor is 10.0.0.128, remote AS 64512, internal link
 Description: Huawei_128
  BGP version 4, remote router ID 10.0.0.128, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 2d21h, last write 2d21h
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:01:36
  Connection interval is 148 seconds
  Failed connection attempts is 1369
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 1
  Last state was Connect
  Last event was TransportError
  Last sent notification:Open Message Error/unsupported capability, Last time 2d21h, First time 2d21h, Repeats 38
    Sent data: 0x010400010080010400020080
  Last rcvd notification:Cease/peer de-configured, Last time 2d21h
  Last sent socket-error:Connect (Connection refused), Last time 00:00:51, First time 2d16h, Repeats 1368
  Last rcvd socket-error:Connection reset by peer, Last time 2d21h, First time 2d21h, Repeats 5
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
Local TCP address is 10.0.0.30
Remote TCP address is 10.0.0.128, remote port is 179

BGP neighbor is 10.0.0.131, remote AS 64512, internal link
 Description: Juniper-131-JCNR
  BGP version 4, remote router ID 10.0.0.131, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:10, last write 00:00:23
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:20
  Keepalive timer is active, time left: 00:00:04
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 3d15h
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
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
    Long Lived Graceful Restart received:
      Helper only
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 3d15h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 3d15h
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
    Opens:                  1         1
    Notifications:          0         0
    Updates:              145         4
    Keepalives:         12282     11592
    Route Refresh:          0         0
    Total messages:     12428     11597
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        32         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         6         1              1                   0
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
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 34875
Remote TCP address is 10.0.0.131, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
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
    Window Scale (wscale): 1,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.5ms/0.1ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 218.57 Mbps
    Recv Round-trip Time (rcv_rtt): 506899.8ms
    Advertised Recv Window (rcv_space): 64335

BGP neighbor is 10.0.0.156, remote AS 64512, internal link
 Description: Juniper-156
  BGP version 4, remote router ID 10.0.0.156, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:12, last write 00:00:02
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:18
  Keepalive timer is active, time left: 00:00:24
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 3d15h
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
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
    Long Lived Graceful Restart received:
      Helper only
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 3d15h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 4
    VPN-IPv6 End-of-RIB received: Yes
      Received 3d15h
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
    Opens:                  1         1
    Notifications:          0         0
    Updates:              142         7
    Keepalives:         12262     11548
    Route Refresh:          0         0
    Total messages:     12405     11556
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        29         4              4                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         6         1              1                   0
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
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 43549
Remote TCP address is 10.0.0.156, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
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
    Round-trip Time (rtt/rtvar): 0.4ms/0.1ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 298.56 Mbps
    Recv Round-trip Time (rcv_rtt): 482781.9ms
    Advertised Recv Window (rcv_space): 64345

BGP neighbor is 10.0.0.179, remote AS 64512, internal link
 Description: Juniper-179
  BGP version 4, remote router ID 10.0.0.179, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:18, last write 00:00:28
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:12
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 2d23h
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Open Message Error/unsupported capability, Last time 2d23h, First time 3d15h, Repeats 333
    Sent data: 0x010400010080010400020080
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
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
    VPN-IPv4 End-of-RIB received: Yes
      Received 2d23h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 4
    VPN-IPv6 End-of-RIB received: Yes
      Received 2d23h
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
    Opens:                335       335
    Notifications:        334         0
    Updates:              111         7
    Keepalives:         10007      9453
    Route Refresh:          0         0
    Total messages:     10787      9795
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        29         4              4                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         6         1              1                   0
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
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 179
Remote TCP address is 10.0.0.179, remote port is 50428
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
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
    Round-trip Time (rtt/rtvar): 0.8ms/0.1ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 137.41 Mbps
    Recv Round-trip Time (rcv_rtt): 335825.5ms
    Advertised Recv Window (rcv_space): 65257

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
  Connect timer is active, time left: 00:00:48
  Connection interval is 148 seconds
  Failed connection attempts is 1859
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Network is unreachable), Last time 00:02:08, First time 3d15h, Repeats 1858
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
Local TCP address is 10.0.0.30
Remote TCP address is 10.0.0.184, remote port is 179

BGP neighbor is 10.0.0.214, remote AS 64512, internal link
 Description: Nokia-SXR-214
  BGP version 4, remote router ID 10.0.0.214, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:12, last write 00:00:21
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:18
  Keepalive timer is active, time left: 00:00:07
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 3d15h
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent socket-error:Connect (Network is unreachable), Last time 3d15h, First time 3d15h, Repeats 10
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
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
    VPN-IPv4 End-of-RIB received: Yes
      Received 3d15h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 3d15h
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
    Opens:                  1         1
    Notifications:          0         0
    Updates:              137         4
    Keepalives:         12254     10456
    Route Refresh:          0         0
    Total messages:     12392     10461
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        32         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         6         1              1                   0
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
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 45419
Remote TCP address is 10.0.0.214, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/332800
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
    Round-trip Time (rtt/rtvar): 0.4ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 297.79 Mbps
    Recv Round-trip Time (rcv_rtt): 78674.8ms
    Advertised Recv Window (rcv_space): 64311

BGP neighbor is 10.0.0.217, remote AS 64512, internal link
 Description: Nokia
  BGP version 4, remote router ID 10.0.0.217, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:25, last write 00:00:18
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:05
  Keepalive timer is active, time left: 00:00:09
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 3d15h
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: yes
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: no
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 3d15h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 4
    VPN-IPv6 End-of-RIB received: Yes
      Received 3d15h
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
    Opens:                  1         1
    Notifications:          0         0
    Updates:              142         7
    Keepalives:         12261     10473
    Route Refresh:          0         0
    Total messages:     12404     10481
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        29         4              4                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         6         1              1                   0
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
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 41903
Remote TCP address is 10.0.0.217, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1012
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: no
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.5ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 177.54 Mbps
    Recv Round-trip Time (rcv_rtt): 195459.6ms
    Advertised Recv Window (rcv_space): 64321

BGP neighbor is 10.0.0.221, remote AS 64512, internal link
 Description: Ribbon-221
  BGP version 4, remote router ID 10.0.0.221, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:15, last write 00:00:33
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:45
  Keepalive timer is active, time left: 00:00:16
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 2d15h
  Number of transitions to established: 8
  Last state was OpenConfirm
  Last event was RecvKeepAlive
  Last sent notification:Hold Timer Expired Error/None, Last time 2d23h
  Last sent socket-error:Connect (Network is unreachable), Last time 2d15h, First time 2d15h, Repeats 8
  Last rcvd socket-error:Connection reset by peer, Last time 2d15h, First time 3d15h, Repeats 5
  Types of communities advertised: standard extended large
  Enhanced route refresh stale path removal disabled
  Outbound enhanced route refresh enabled
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised and received and negotiated
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
    VPN-IPv4 End-of-RIB received: No
      Number of stale paths removed after graceful restart: 0
    VPN-IPv6 End-of-RIB received: No
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
    Opens:                           8         8
    Notifications:                   1         0
    Updates:                       445        24
    Keepalives:                   6071     14272
    Enhanced Route Refresh:          0        10
    Begin of Route Refresh:         10         0
    End of Route Refresh:           10         0
    Total messages:               6545     14314
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        31         2              2                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         7         0              0                   0
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
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 44007
Remote TCP address is 10.0.0.221, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1448
  Total Number of TCP retransmissions: 2
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 9,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.2ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 517.14 Mbps
    Recv Round-trip Time (rcv_rtt): 230754.9ms
    Advertised Recv Window (rcv_space): 64324

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
Endpoint        Tunnel Type     Index(es)   Tunnel Preference   IGP Preference 
-------------- --------------- ----------- ------------------- ----------------
10.0.0.32/32    IS-IS SR IPv4   20          65                  115            
10.0.0.53/32    IS-IS SR IPv4   10          65                  115            
10.0.0.66/32    IS-IS SR IPv4   13          65                  115            
10.0.0.72/32    IS-IS SR IPv4   14          65                  115            
10.0.0.84/32    IS-IS SR IPv4   8           65                  115            
10.0.0.120/32   IS-IS SR IPv4   17          65                  115            
10.0.0.131/32   IS-IS SR IPv4   9           65                  115            
10.0.0.156/32   IS-IS SR IPv4   11          65                  115            
10.0.0.175/32   IS-IS SR IPv4   7           65                  115            
10.0.0.179/32   IS-IS SR IPv4   12          65                  115            
10.0.0.214/32   IS-IS SR IPv4   21          65                  115            
10.0.0.217/32   IS-IS SR IPv4   16          65                  115            
10.0.0.221/32   IS-IS SR IPv4   15          65                  115            
2002::120/128   IS-IS SR IPv6   2           65                  115            
2002::175/128   IS-IS SR IPv6   3           65                  115            
2002::53/128    IS-IS SR IPv6   6           65                  115            
2002::156/128   IS-IS SR IPv6   5           65                  115            

   IGP Metric    Metric Type
---------------- -----------
   1             metric     
   21            metric     
   11            metric     
   11            metric     
   11            metric     
   1             metric     
   1             metric     
   1             metric     
   11            metric     
   1             metric     
   1             metric     
   1             metric     
   1             metric     
   10            metric     
   20            metric     
   30            metric     
   10            metric     

```

## show tunnel rib colored brief

```text
Tunnel RIB: system-colored-tunnel-rib
 Endpoint        Color   Tunnel Type       Index(es)    Tunnel Preference    IGP Preference    IGP Metric   Metric Type
--------------- ------- ----------------- ------------ -------------------- ----------------- ------------- -----------
 10.0.0.32/32    128     IS-IS FlexAlgo    46           65                   115               10000        metric     
 10.0.0.32/32    129     IS-IS FlexAlgo    47           65                   115               100          metric     
 10.0.0.32/32    130     IS-IS FlexAlgo    48           65                   115               1            metric     
 10.0.0.53/32    128     IS-IS FlexAlgo    8            65                   115               110010       metric     
 10.0.0.53/32    129     IS-IS FlexAlgo    3            65                   115               120          metric     
 10.0.0.120/32   128     IS-IS FlexAlgo    51           65                   115               110010       metric     
 10.0.0.120/32   129     IS-IS FlexAlgo    52           65                   115               120          metric     
 10.0.0.156/32   128     IS-IS FlexAlgo    14           65                   115               10000        metric     
 10.0.0.156/32   129     IS-IS FlexAlgo    6            65                   115               100          metric     
 10.0.0.156/32   130     IS-IS FlexAlgo    37           65                   115               1            metric     
 10.0.0.175/32   128     IS-IS FlexAlgo    7            65                   115               10010        metric     
 10.0.0.175/32   129     IS-IS FlexAlgo    2            65                   115               110          metric     
 10.0.0.175/32   130     IS-IS FlexAlgo    28           65                   115               11           metric     
 10.0.0.179/32   128     IS-IS FlexAlgo    15           65                   115               10000        metric     
 10.0.0.179/32   129     IS-IS FlexAlgo    9            65                   115               100          metric     
 10.0.0.179/32   130     IS-IS FlexAlgo    34           65                   115               1            metric     
 10.0.0.217/32   128     IS-IS FlexAlgo    41           65                   115               10000        metric     
 10.0.0.217/32   129     IS-IS FlexAlgo    39           65                   115               100          metric     
 10.0.0.217/32   130     IS-IS FlexAlgo    40           65                   115               1            metric     
 10.0.0.221/32   128     IS-IS FlexAlgo    4            65                   115               10000        metric     
 10.0.0.221/32   129     IS-IS FlexAlgo    12           65                   115               100          metric     
 2002::156/128   128     IS-IS FlexAlgo    21           65                   115               10000        metric     
 2002::156/128   129     IS-IS FlexAlgo    25           65                   115               100          metric     
 2002::156/128   130     IS-IS FlexAlgo    36           65                   115               10           metric     
 2002::53/128    128     IS-IS FlexAlgo    19           65                   115               210000       metric     
 2002::53/128    129     IS-IS FlexAlgo    17           65                   115               120          metric     
 2002::175/128   128     IS-IS FlexAlgo    26           65                   115               110000       metric     
 2002::175/128   129     IS-IS FlexAlgo    18           65                   115               110          metric     
 2002::175/128   130     IS-IS FlexAlgo    45           65                   115               20           metric     

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
>C    10.0.0.30/32 [0 pref/0 metric] updated 3d17h ago
         via Loopback0, directly connected
>C    20.30.32.0/24 [0 pref/0 metric] updated 2d15h ago
         via Ethernet2, directly connected
>C    20.30.66.0/24 [0 pref/0 metric] updated 2d15h ago
         via Ethernet31, directly connected
>C    20.30.72.0/24 [0 pref/0 metric] updated 2d14h ago
         via Ethernet9, directly connected
>C    20.30.84.0/24 [0 pref/0 metric] updated 2d14h ago
         via Ethernet12, directly connected
>C    20.30.120.0/24 [0 pref/0 metric] updated 2d14h ago
         via Ethernet3, directly connected
>C    20.30.124.0/24 [0 pref/0 metric] updated 2d15h ago
         via Ethernet17, directly connected
>C    20.30.128.0/24 [0 pref/0 metric] updated 22:08:51 ago
         via Ethernet19, directly connected
>C    20.30.131.0/24 [0 pref/0 metric] updated 3d17h ago
         via Ethernet35, directly connected
>C    20.30.156.0/24 [0 pref/0 metric] updated 2d18h ago
         via Ethernet11, directly connected
>C    20.30.179.0/24 [0 pref/0 metric] updated 2d18h ago
         via Ethernet40, directly connected
>C    20.30.184.0/24 [0 pref/0 metric] updated 3d17h ago
         via Ethernet7, directly connected
>C    20.30.214.0/24 [0 pref/0 metric] updated 1d18h ago
         via Ethernet5, directly connected
>C    20.30.217.0/24 [0 pref/0 metric] updated 2d15h ago
         via Ethernet4, directly connected
>C    20.30.221.0/24 [0 pref/0 metric] updated 2d15h ago
         via Ethernet15, directly connected
>C    21.30.124.0/24 [0 pref/0 metric] updated 2d15h ago
         via Ethernet18, directly connected
>C    21.30.128.0/24 [0 pref/0 metric] updated 2d17h ago
         via Ethernet20, directly connected
>C    21.30.156.0/24 [0 pref/0 metric] updated 2d18h ago
         via Ethernet21, directly connected
>C    21.30.217.0/24 [0 pref/0 metric] updated 2d21h ago
         via Ethernet8, directly connected
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
>P    0.0.0.0/8 [1 pref/0 metric] updated 3d17h ago
         via Null0, directly connected [NF]
>P    127.0.0.0/8 [1 pref/0 metric] updated 3d17h ago
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
>I    10.0.0.32/32 [115 pref/1 metric] updated 2d15h ago
         via 20.30.32.32, Ethernet2
>I    10.0.0.53/32 [115 pref/21 metric] updated 00:05:58 ago
         via 20.30.32.32, Ethernet2
         via 20.30.66.66, Ethernet31
         via 20.30.72.72, Ethernet9
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.131.131, Ethernet35
         via 20.30.156.156, Ethernet11
>I    10.0.0.66/32 [115 pref/11 metric] updated 2d14h ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.72/32 [115 pref/11 metric] updated 2d14h ago
         via 20.30.72.72, Ethernet9
>I    10.0.0.84/32 [115 pref/11 metric] updated 2d14h ago
         via 20.30.84.84, Ethernet12
>I    10.0.0.120/32 [115 pref/1 metric] updated 2d14h ago
         via 20.30.120.120, Ethernet3
>I    10.0.0.124/32 [115 pref/1 metric] updated 2d15h ago
         via 20.30.124.124, Ethernet17
         via 21.30.124.124, Ethernet18
>I    10.0.0.128/32 [115 pref/1 metric] updated 22:08:50 ago
         via 20.30.128.128, Ethernet19
         via 21.30.128.128, Ethernet20
>I    10.0.0.131/32 [115 pref/1 metric] updated 3d00h ago
         via 20.30.131.131, Ethernet35
>I    10.0.0.156/32 [115 pref/1 metric] updated 2d18h ago
         via 20.30.156.156, Ethernet11
         via 21.30.156.156, Ethernet21
>I    10.0.0.175/32 [115 pref/11 metric] updated 00:05:58 ago
         via 20.30.32.32, Ethernet2
         via 20.30.66.66, Ethernet31
         via 20.30.72.72, Ethernet9
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.131.131, Ethernet35
         via 20.30.156.156, Ethernet11
>I    10.0.0.179/32 [115 pref/1 metric] updated 2d18h ago
         via 20.30.179.179, Ethernet40
>I    10.0.0.214/32 [115 pref/1 metric] updated 1d18h ago
         via 20.30.214.214, Ethernet5
>I    10.0.0.216/32 [115 pref/11 metric] updated 1d18h ago
         via 20.30.214.214, Ethernet5
>I    10.0.0.217/32 [115 pref/1 metric] updated 2d15h ago
         via 20.30.217.217, Ethernet4
>I    10.0.0.221/32 [115 pref/1 metric] updated 2d15h ago
         via 20.30.221.221, Ethernet15
>I    10.0.1.179/32 [115 pref/1 metric] updated 2d18h ago
         via 20.30.179.179, Ethernet40
>I    20.32.175.0/24 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.32, Ethernet2
>I    20.53.175.0/24 [115 pref/21 metric] updated 00:05:58 ago
         via 20.30.32.32, Ethernet2
         via 20.30.66.66, Ethernet31
         via 20.30.72.72, Ethernet9
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.131.131, Ethernet35
         via 20.30.156.156, Ethernet11
>I    20.66.175.0/24 [115 pref/11 metric] updated 2d14h ago
         via 20.30.66.66, Ethernet31
>I    20.72.175.0/24 [115 pref/11 metric] updated 2d14h ago
         via 20.30.72.72, Ethernet9
>I    20.84.175.0/24 [115 pref/21 metric] updated 00:05:58 ago
         via 20.30.32.32, Ethernet2
         via 20.30.66.66, Ethernet31
         via 20.30.72.72, Ethernet9
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.131.131, Ethernet35
         via 20.30.156.156, Ethernet11
>I    20.120.175.0/24 [115 pref/11 metric] updated 2d14h ago
         via 20.30.120.120, Ethernet3
>I    20.120.214.0/24 [115 pref/11 metric] updated 2d14h ago
         via 20.30.120.120, Ethernet3
>I    20.120.217.0/24 [115 pref/1 metric] updated 2d14h ago
         via 20.30.120.120, Ethernet3
>I    20.124.175.0/24 [115 pref/11 metric] updated 2d15h ago
         via 20.30.124.124, Ethernet17
         via 21.30.124.124, Ethernet18
>I    20.128.175.0/24 [115 pref/11 metric] updated 22:08:50 ago
         via 20.30.128.128, Ethernet19
         via 21.30.128.128, Ethernet20
>I    20.131.175.0/24 [115 pref/11 metric] updated 3d00h ago
         via 20.30.131.131, Ethernet35
>I    20.156.175.0/24 [115 pref/11 metric] updated 2d18h ago
         via 20.30.156.156, Ethernet11
         via 21.30.156.156, Ethernet21
>I    20.175.179.0/24 [115 pref/11 metric] updated 2d18h ago
         via 20.30.179.179, Ethernet40
>I    20.175.184.0/24 [115 pref/21 metric] updated 00:05:58 ago
         via 20.30.32.32, Ethernet2
         via 20.30.66.66, Ethernet31
         via 20.30.72.72, Ethernet9
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.131.131, Ethernet35
         via 20.30.156.156, Ethernet11
>I    20.175.214.0/24 [115 pref/21 metric] updated 00:05:58 ago
         via 20.30.32.32, Ethernet2
         via 20.30.66.66, Ethernet31
         via 20.30.72.72, Ethernet9
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.131.131, Ethernet35
         via 20.30.156.156, Ethernet11
>I    20.175.217.0/24 [115 pref/11 metric] updated 2d15h ago
         via 20.30.217.217, Ethernet4
>I    20.175.221.0/24 [115 pref/11 metric] updated 2d15h ago
         via 20.30.221.221, Ethernet15
>I    20.214.216.0/24 [115 pref/11 metric] updated 1d18h ago
         via 20.30.214.214, Ethernet5
>I    192.168.20.0/23 [115 pref/1 metric] updated 2d14h ago
         via 20.30.120.120, Ethernet3
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
>C    2001:0:30:32::/64 [0 pref/0 metric] updated 2d15h ago
         via Ethernet2, directly connected
>C    2001:0:30:66::/64 [0 pref/0 metric] updated 2d15h ago
         via Ethernet31, directly connected
>C    2001:0:30:72::/64 [0 pref/0 metric] updated 2d14h ago
         via Ethernet9, directly connected
>C    2001:0:30:84::/64 [0 pref/0 metric] updated 2d14h ago
         via Ethernet12, directly connected
>C    2001:0:30:120::/64 [0 pref/0 metric] updated 2d14h ago
         via Ethernet3, directly connected
>C    2001:0:30:124::/64 [0 pref/0 metric] updated 2d15h ago
         via Ethernet17, directly connected
>C    2001:0:30:128::/64 [0 pref/0 metric] updated 22:08:51 ago
         via Ethernet19, directly connected
>C    2001:0:30:131::/64 [0 pref/0 metric] updated 3d17h ago
         via Ethernet35, directly connected
>C    2001:0:30:156::/64 [0 pref/0 metric] updated 2d18h ago
         via Ethernet11, directly connected
>C    2001:0:30:179::/64 [0 pref/0 metric] updated 2d18h ago
         via Ethernet40, directly connected
>C    2001:0:30:184::/64 [0 pref/0 metric] updated 3d17h ago
         via Ethernet7, directly connected
>C    2001:0:30:214::/64 [0 pref/0 metric] updated 1d18h ago
         via Ethernet5, directly connected
>C    2001:0:30:217::/64 [0 pref/0 metric] updated 2d15h ago
         via Ethernet4, directly connected
>C    2001:0:30:221::/64 [0 pref/0 metric] updated 2d15h ago
         via Ethernet15, directly connected
>C    2002::30/128 [0 pref/0 metric] updated 3d17h ago
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
>P    ::/96 [1 pref/0 metric] updated 3d17h ago
         via Null0, directly connected [NF]
>P    ::ffff:127.0.0.0/104 [1 pref/0 metric] updated 3d17h ago
         via :: [1 pref/1 metric] type ipv6
            via , directly connected
>P    fe80::/10 [1 pref/0 metric] updated 3d17h ago
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
>I    2000::214/128 [115 pref/30 metric] updated 00:05:58 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:32:175::/64 [115 pref/20 metric] updated 2d15h ago
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
>I    2001:0:53:175::/64 [115 pref/30 metric] updated 00:05:58 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:66:175::/64 [115 pref/30 metric] updated 00:05:58 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:72:175::/64 [115 pref/30 metric] updated 00:05:58 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:84:175::/64 [115 pref/20 metric] updated 2d14h ago
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
>I    2001:0:120:175::/64 [115 pref/20 metric] updated 2d14h ago
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:120:214::/64 [115 pref/20 metric] updated 2d14h ago
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:120:217::/64 [115 pref/10 metric] updated 2d14h ago
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:128:175::/64 [115 pref/30 metric] updated 00:05:58 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:131:175::/64 [115 pref/30 metric] updated 00:05:58 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:156:175::/64 [115 pref/20 metric] updated 2d18h ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
>I    2001:0:175::/64 [115 pref/30 metric] updated 00:05:58 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:175:184::/64 [115 pref/30 metric] updated 00:05:58 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:175:214::/64 [115 pref/30 metric] updated 00:05:58 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:175:217::/64 [115 pref/20 metric] updated 2d15h ago
         via fe80::c214:b8ff:fe21:9790, Ethernet4
>I    2001:0:175:221::/64 [115 pref/30 metric] updated 00:05:58 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:214:216::/64 [115 pref/40 metric] updated 00:05:58 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2002::32/128 [115 pref/20 metric] updated 2d15h ago
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
>I    2002::53/128 [115 pref/30 metric] updated 00:05:58 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2002::120/128 [115 pref/10 metric] updated 2d14h ago
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2002::156/128 [115 pref/10 metric] updated 2d18h ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
>I    2002::175/128 [115 pref/20 metric] updated 00:05:58 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2002::216/128 [115 pref/40 metric] updated 00:05:58 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2002::217/128 [115 pref/10 metric] updated 2d15h ago
         via fe80::c214:b8ff:fe21:9790, Ethernet4
```

## show platform sand l3 summary

```text
Number of vrfs: 4

Ipv4:
  Routes:       176  backlog:  0  unprogrammed:  0
  Adjacencies:  261  backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       69   backlog:  0  unprogrammed:  0
  Adjacencies:  261  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       63  backlog:  0  unprogrammed:  0
  Adjacencies:  22  backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4204  ecmp fecs:  10  fec entries:  4245
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  17  ecmp fecs:  5  fec entries:  47
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   176  unprogrammed:   0   
  Routes6:  69   unprogrammed6:  0   
  Backlog:  0  

Jericho2 Lpm:
  TCAM entries used:   4   Percent free:  99  ADS2 entries used:   12  Percent free:  99
  Pivot buckets used:  6   Rows used:     2   Entries Per Bucket:  2   Percent free:  99
  Route buckets used:  41  Rows used:     6   Entries Per Bucket:  5   Percent free:  99

Lem:
  IPv4  Host in Lem:            disabled
  IPv4  Prefix-lengths in Lem:  None    
  IPv6  Host in Lem:            disabled
  IPv6  Prefix-lengths in Lem:  None    
  Number of downloads:        0
  Number of overflow events:  0

Egress Arp rewrite entries in use (in each fap):
  FixedSystem: 16
Egress Arp remote rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Ip tunnel rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Mpls (for outer 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Mpls (for inner 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 37
Egress Sflow rewrite entries in use (in each fap):
  FixedSystem: 0

Egress rewrite chains in backlog: resource-full 0, no-interface 0

Glem entries used per fap :
  FixedSystem: 4212

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  320  allocs:  2631  frees:  2494  shuffles:  0  cmds:  0
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
    Non-ecmp fecs:            82  ecmp fecs:            0  
    Non-ecmp (Percent free):  99  ecmp (Percent free):  100
  Level3  Fecs:
    Non-ecmp fecs:            304  ecmp fecs:            15
    Non-ecmp (Percent free):  99   ecmp (Percent free):  99

Lpm Detail:
  Requests:  5209  cleanses:  793  batches:  793  avg batch size:  6

Jericho Arp:
  ArpTable writes:      50160   queued      0   
  IngressTable writes:  120464  queued      0   
  Coprocessors:         1       in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  100  
  Number of uncountable MPLS tunnels:      100  
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
|0  |10.0.0.32/32      |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |  -  |319054|   -   
|0  |10.0.0.53/32      |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |24581|318812|   -   
|0  |10.0.0.53/32      |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24581|318813|   -   
|0  |10.0.0.53/32      |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24581|318814|   -   
|0  |10.0.0.53/32      |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24581|318815|   -   
|0  |10.0.0.53/32      |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24581|318816|   -   
|0  |10.0.0.53/32      |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24581|318817|   -   
|0  |10.0.0.53/32      |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24581|318818|   -   
|0  |10.0.0.53/32      |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24581|318819|   -   
|0  |10.0.0.53/32      |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24581|318820|   -   
|0  |10.0.0.53/32      |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24581|318821|   -   
|0  |10.0.0.53/32      |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24581|318822|   -   
|0  |10.0.0.53/32      |ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |24581|318823|   -   
|0  |10.0.0.53/32      |ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |24581|318824|   -   
|0  |10.0.0.53/32      |ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |24581|318825|   -   
|0  |10.0.0.53/32      |ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |24581|318826|   -   
|0  |10.0.0.53/32      |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |24581|318827|   -   
|0  |10.0.0.66/32      |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318838|   -   
|0  |10.0.0.72/32      |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |  -  |318860|   -   
|0  |10.0.0.84/32      |ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |  -  |318960|   -   
|0  |10.0.0.120/32     |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |  -  |318924|   -   
|0  |10.0.0.124/32     |ROUTE| Et18               |1013 |103450  | 64:6d:4e:32:e1:23 |24577|318856|   -   
|0  |10.0.0.124/32     |ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |24577|318857|   -   
|0  |10.0.0.124/32     |ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |24577|318858|   -   
|0  |10.0.0.124/32     |ROUTE| Et18               |1013 |103450  | 64:6d:4e:32:e1:23 |24577|318859|   -   
|0  |10.0.0.128/32     |ROUTE| Et20               |1025 |103475  | 60:53:75:13:ba:dd |24580|319014|   -   
|0  |10.0.0.128/32     |ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |24580|319015|   -   
|0  |10.0.0.128/32     |ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |24580|319016|   -   
|0  |10.0.0.128/32     |ROUTE| Et20               |1025 |103475  | 60:53:75:13:ba:dd |24580|319017|   -   
|0  |10.0.0.131/32     |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |  -  |318868|   -   
|0  |10.0.0.156/32     |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24582|318844|   -   
|0  |10.0.0.156/32     |ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |24582|318845|   -   
|0  |10.0.0.156/32     |ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |24582|318846|   -   
|0  |10.0.0.156/32     |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24582|318847|   -   
|0  |10.0.0.175/32     |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |24581|318812|   -   
|0  |10.0.0.175/32     |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24581|318813|   -   
|0  |10.0.0.175/32     |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24581|318814|   -   
|0  |10.0.0.175/32     |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24581|318815|   -   
|0  |10.0.0.175/32     |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24581|318816|   -   
|0  |10.0.0.175/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24581|318817|   -   
|0  |10.0.0.175/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24581|318818|   -   
|0  |10.0.0.175/32     |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24581|318819|   -   
|0  |10.0.0.175/32     |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24581|318820|   -   
|0  |10.0.0.175/32     |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24581|318821|   -   
|0  |10.0.0.175/32     |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24581|318822|   -   
|0  |10.0.0.175/32     |ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |24581|318823|   -   
|0  |10.0.0.175/32     |ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |24581|318824|   -   
|0  |10.0.0.175/32     |ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |24581|318825|   -   
|0  |10.0.0.175/32     |ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |24581|318826|   -   
|0  |10.0.0.175/32     |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |24581|318827|   -   
|0  |10.0.0.179/32     |ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |  -  |318910|   -   
|0  |10.0.0.214/32     |ROUTE| Et5                |1008 |103423  | 18:5b:00:61:ac:6f |  -  |318926|   -   
|0  |10.0.0.216/32     |ROUTE| Et5                |1008 |103423  | 18:5b:00:61:ac:6f |  -  |318926|   -   
|0  |10.0.0.217/32     |ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |  -  |319066|   -   
|0  |10.0.0.221/32     |ROUTE| Et15               |1006 |103424  | 30:c5:07:84:3e:79 |  -  |318950|   -   
|0  |10.0.1.179/32     |ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |  -  |318910|   -   
|0  |20.30.32.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.32.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.32.32/32    |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |  -  |318882|   -   
|0  |20.30.32.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.32.0/24     |TRAP | CoppSystemL3DstMiss|1018 |1018    | ArpTrap           |  -  |315689|   -   
|0  |20.30.66.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.66.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.66.66/32    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318992|   -   
|0  |20.30.66.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.66.0/24     |TRAP | CoppSystemL3DstMiss|1020 |1020    | ArpTrap           |  -  |315691|   -   
|0  |20.30.72.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.72.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.72.72/32    |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |  -  |318864|   -   
|0  |20.30.72.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.72.0/24     |TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |  -  |315680|   -   
|0  |20.30.84.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.84.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.84.84/32    |ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |  -  |318776|   -   
|0  |20.30.84.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.84.0/24     |TRAP | CoppSystemL3DstMiss|1014 |1014    | ArpTrap           |  -  |315685|   -   
|0  |20.30.120.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.120.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.120.120/32  |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |  -  |318800|   -   
|0  |20.30.120.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.120.0/24    |TRAP | CoppSystemL3DstMiss|1017 |1017    | ArpTrap           |  -  |315688|   -   
|0  |20.30.124.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.124.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.124.124/32  |ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |  -  |318936|   -   
|0  |20.30.124.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.124.0/24    |TRAP | CoppSystemL3DstMiss|1016 |1016    | ArpTrap           |  -  |315687|   -   
|0  |20.30.128.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.128.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.128.128/32  |ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |  -  |318842|   -   
|0  |20.30.128.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.128.0/24    |TRAP | CoppSystemL3DstMiss|1021 |1021    | ArpTrap           |  -  |315692|   -   
|0  |20.30.131.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.131.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.131.131/32  |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |  -  |318928|   -   
|0  |20.30.131.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.131.0/24    |TRAP | CoppSystemL3DstMiss|1012 |1012    | ArpTrap           |  -  |315683|   -   
|0  |20.30.156.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.156.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.156.156/32  |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |  -  |318770|   -   
|0  |20.30.156.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.156.0/24    |TRAP | CoppSystemL3DstMiss|1019 |1019    | ArpTrap           |  -  |315690|   -   
|0  |20.30.179.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.179.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.179.179/32  |ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |  -  |319072|   -   
|0  |20.30.179.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.179.0/24    |TRAP | CoppSystemL3DstMiss|1015 |1015    | ArpTrap           |  -  |315686|   -   
|0  |20.30.184.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.184.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.184.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.184.0/24    |TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |  -  |315681|   -   
|0  |20.30.214.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.214.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.214.214/32  |ROUTE| Et5                |1008 |103423  | 18:5b:00:61:ac:6f |  -  |319032|   -   
|0  |20.30.214.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.214.0/24    |TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |  -  |315679|   -   
|0  |20.30.217.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.217.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.217.217/32  |ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |  -  |318962|   -   
|0  |20.30.217.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.217.0/24    |TRAP | CoppSystemL3DstMiss|1007 |1007    | ArpTrap           |  -  |315678|   -   
|0  |20.30.221.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.221.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.221.221/32  |ROUTE| Et15               |1006 |103424  | 30:c5:07:84:3e:79 |  -  |318854|   -   
|0  |20.30.221.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.221.0/24    |TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |  -  |315677|   -   
|0  |20.32.175.0/24    |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |  -  |319054|   -   
|0  |20.53.175.0/24    |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |24581|318812|   -   
|0  |20.53.175.0/24    |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24581|318813|   -   
|0  |20.53.175.0/24    |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24581|318814|   -   
|0  |20.53.175.0/24    |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24581|318815|   -   
|0  |20.53.175.0/24    |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24581|318816|   -   
|0  |20.53.175.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24581|318817|   -   
|0  |20.53.175.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24581|318818|   -   
|0  |20.53.175.0/24    |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24581|318819|   -   
|0  |20.53.175.0/24    |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24581|318820|   -   
|0  |20.53.175.0/24    |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24581|318821|   -   
|0  |20.53.175.0/24    |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24581|318822|   -   
|0  |20.53.175.0/24    |ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |24581|318823|   -   
|0  |20.53.175.0/24    |ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |24581|318824|   -   
|0  |20.53.175.0/24    |ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |24581|318825|   -   
|0  |20.53.175.0/24    |ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |24581|318826|   -   
|0  |20.53.175.0/24    |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |24581|318827|   -   
|0  |20.66.175.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318838|   -   
|0  |20.72.175.0/24    |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |  -  |318860|   -   
|0  |20.84.175.0/24    |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |24581|318812|   -   
|0  |20.84.175.0/24    |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24581|318813|   -   
|0  |20.84.175.0/24    |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24581|318814|   -   
|0  |20.84.175.0/24    |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24581|318815|   -   
|0  |20.84.175.0/24    |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24581|318816|   -   
|0  |20.84.175.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24581|318817|   -   
|0  |20.84.175.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24581|318818|   -   
|0  |20.84.175.0/24    |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24581|318819|   -   
|0  |20.84.175.0/24    |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24581|318820|   -   
|0  |20.84.175.0/24    |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24581|318821|   -   
|0  |20.84.175.0/24    |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24581|318822|   -   
|0  |20.84.175.0/24    |ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |24581|318823|   -   
|0  |20.84.175.0/24    |ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |24581|318824|   -   
|0  |20.84.175.0/24    |ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |24581|318825|   -   
|0  |20.84.175.0/24    |ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |24581|318826|   -   
|0  |20.84.175.0/24    |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |24581|318827|   -   
|0  |20.120.175.0/24   |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |  -  |318924|   -   
|0  |20.120.214.0/24   |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |  -  |318924|   -   
|0  |20.120.217.0/24   |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |  -  |318924|   -   
|0  |20.124.175.0/24   |ROUTE| Et18               |1013 |103450  | 64:6d:4e:32:e1:23 |24577|318856|   -   
|0  |20.124.175.0/24   |ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |24577|318857|   -   
|0  |20.124.175.0/24   |ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |24577|318858|   -   
|0  |20.124.175.0/24   |ROUTE| Et18               |1013 |103450  | 64:6d:4e:32:e1:23 |24577|318859|   -   
|0  |20.128.175.0/24   |ROUTE| Et20               |1025 |103475  | 60:53:75:13:ba:dd |24580|319014|   -   
|0  |20.128.175.0/24   |ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |24580|319015|   -   
|0  |20.128.175.0/24   |ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |24580|319016|   -   
|0  |20.128.175.0/24   |ROUTE| Et20               |1025 |103475  | 60:53:75:13:ba:dd |24580|319017|   -   
|0  |20.131.175.0/24   |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |  -  |318868|   -   
|0  |20.156.175.0/24   |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24582|318844|   -   
|0  |20.156.175.0/24   |ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |24582|318845|   -   
|0  |20.156.175.0/24   |ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |24582|318846|   -   
|0  |20.156.175.0/24   |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24582|318847|   -   
|0  |20.175.179.0/24   |ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |  -  |318910|   -   
|0  |20.175.184.0/24   |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |24581|318812|   -   
|0  |20.175.184.0/24   |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24581|318813|   -   
|0  |20.175.184.0/24   |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24581|318814|   -   
|0  |20.175.184.0/24   |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24581|318815|   -   
|0  |20.175.184.0/24   |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24581|318816|   -   
|0  |20.175.184.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24581|318817|   -   
|0  |20.175.184.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24581|318818|   -   
|0  |20.175.184.0/24   |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24581|318819|   -   
|0  |20.175.184.0/24   |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24581|318820|   -   
|0  |20.175.184.0/24   |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24581|318821|   -   
|0  |20.175.184.0/24   |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24581|318822|   -   
|0  |20.175.184.0/24   |ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |24581|318823|   -   
|0  |20.175.184.0/24   |ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |24581|318824|   -   
|0  |20.175.184.0/24   |ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |24581|318825|   -   
|0  |20.175.184.0/24   |ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |24581|318826|   -   
|0  |20.175.184.0/24   |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |24581|318827|   -   
|0  |20.175.214.0/24   |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |24581|318812|   -   
|0  |20.175.214.0/24   |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24581|318813|   -   
|0  |20.175.214.0/24   |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24581|318814|   -   
|0  |20.175.214.0/24   |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24581|318815|   -   
|0  |20.175.214.0/24   |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24581|318816|   -   
|0  |20.175.214.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24581|318817|   -   
|0  |20.175.214.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24581|318818|   -   
|0  |20.175.214.0/24   |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24581|318819|   -   
|0  |20.175.214.0/24   |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24581|318820|   -   
|0  |20.175.214.0/24   |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24581|318821|   -   
|0  |20.175.214.0/24   |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24581|318822|   -   
|0  |20.175.214.0/24   |ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |24581|318823|   -   
|0  |20.175.214.0/24   |ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |24581|318824|   -   
|0  |20.175.214.0/24   |ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |24581|318825|   -   
|0  |20.175.214.0/24   |ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |24581|318826|   -   
|0  |20.175.214.0/24   |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |24581|318827|   -   
|0  |20.175.217.0/24   |ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |  -  |319066|   -   
|0  |20.175.221.0/24   |ROUTE| Et15               |1006 |103424  | 30:c5:07:84:3e:79 |  -  |318950|   -   
|0  |20.214.216.0/24   |ROUTE| Et5                |1008 |103423  | 18:5b:00:61:ac:6f |  -  |318926|   -   
|0  |21.30.124.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.124.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |21.30.124.124/32  |ROUTE| Et18               |1013 |103450  | 64:6d:4e:32:e1:23 |  -  |318938|   -   
|0  |21.30.124.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.124.0/24    |TRAP | CoppSystemL3DstMiss|1013 |1013    | ArpTrap           |  -  |315684|   -   
|0  |21.30.128.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.128.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |21.30.128.128/32  |ROUTE| Et20               |1025 |103475  | 60:53:75:13:ba:dd |  -  |319070|   -   
|0  |21.30.128.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.128.0/24    |TRAP | CoppSystemL3DstMiss|1025 |1025    | ArpTrap           |  -  |315696|   -   
|0  |21.30.156.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.156.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |21.30.156.156/32  |ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |  -  |318954|   -   
|0  |21.30.156.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.156.0/24    |TRAP | CoppSystemL3DstMiss|1027 |1027    | ArpTrap           |  -  |315698|   -   
|0  |21.30.217.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.217.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |21.30.217.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.217.0/24    |TRAP | CoppSystemL3DstMiss|1023 |1023    | ArpTrap           |  -  |315694|   -   
|0  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|0  |192.168.20.0/23   |ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |  -  |318924|   -   
|0  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|1  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318968|   -   
|1  |10.0.0.30/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|1  |50.10.32.0/24     |ROUTE| FEC 318794         |0    |2097128 | 00:00:00:00:00:00 |  -  |183506|M 378528
|1  |50.10.53.0/24     |ROUTE| FEC 24579          |0    |2097122 | 00:00:00:00:00:00 |  -  |183520|M 970000
|1  |50.10.66.0/24     |ROUTE| FEC 319034         |0    |2097146 | 00:00:00:00:00:00 |  -  |183556|M 62000
|1  |50.10.72.0/24     |ROUTE| FEC 319038         |0    |2097148 | 00:00:00:00:00:00 |  -  |183538|M 62000
|1  |50.10.84.0/24     |ROUTE| FEC 319030         |0    |2097139 | 00:00:00:00:00:00 |  -  |183518|M 20084 720898
|1  |50.10.120.0/24    |ROUTE| FEC 318840         |0    |2097151 | 00:00:00:00:00:00 |  -  |183542|M 1279
|1  |50.10.131.0/24    |ROUTE| FEC 318942         |0    |2097134 | 00:00:00:00:00:00 |  -  |183530|M 18
|1  |50.10.156.0/24    |ROUTE| FEC 24587          |0    |2097138 | 00:00:00:00:00:00 |  -  |183524|M 16
|1  |50.10.179.0/24    |ROUTE| FEC 318940         |0    |2097127 | 00:00:00:00:00:00 |  -  |183560|M 16
|1  |50.10.214.0/24    |ROUTE| FEC 318866         |0    |2097150 | 00:00:00:00:00:00 |  -  |183550|M 20214 500000
|1  |50.10.217.0/24    |ROUTE| FEC 319012         |0    |2097124 | 00:00:00:00:00:00 |  -  |183510|M 20217 524287
|1  |50.10.221.0/24    |ROUTE| FEC 318998         |0    |2097133 | 00:00:00:00:00:00 |  -  |183536|M 524292
|1  |50.129.66.0/24    |ROUTE| FEC 319034         |0    |2097146 | 00:00:00:00:00:00 |  -  |183556|M 62000
|1  |50.129.72.0/24    |ROUTE| FEC 319038         |0    |2097148 | 00:00:00:00:00:00 |  -  |183538|M 62000
|1  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|1  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|2  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318970|   -   
|2  |10.128.0.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|2  |50.128.32.0/24    |ROUTE| FEC 318808         |0    |2097117 | 00:00:00:00:00:00 |  -  |183540|M 378530
|2  |50.128.53.0/24    |ROUTE| FEC 318994         |0    |2097115 | 00:00:00:00:00:00 |  -  |183570|M 970002
|2  |50.128.120.0/24   |ROUTE| FEC 318798         |0    |2097143 | 00:00:00:00:00:00 |  -  |183580|M 1278
|2  |50.128.156.0/24   |ROUTE| FEC 24587          |0    |2097130 | 00:00:00:00:00:00 |  -  |183526|M 17
|2  |50.128.179.0/24   |ROUTE| FEC 318796         |0    |2097118 | 00:00:00:00:00:00 |  -  |183562|M 21
|2  |50.128.217.0/24   |ROUTE| FEC 319086         |0    |2097131 | 00:00:00:00:00:00 |  -  |183512|M 21345 524284
|2  |50.129.32.0/24    |ROUTE| FEC 319048         |0    |2097114 | 00:00:00:00:00:00 |  -  |183532|M 378530
|2  |50.129.53.0/24    |ROUTE| FEC 24588          |0    |2097121 | 00:00:00:00:00:00 |  -  |183574|M 970002
|2  |50.129.120.0/24   |ROUTE| FEC 24576          |0    |2097149 | 00:00:00:00:00:00 |  -  |183578|M 1277
|2  |50.129.156.0/24   |ROUTE| FEC 24587          |0    |2097130 | 00:00:00:00:00:00 |  -  |183528|M 17
|2  |50.129.179.0/24   |ROUTE| FEC 318964         |0    |2097112 | 00:00:00:00:00:00 |  -  |183564|M 21
|2  |50.129.217.0/24   |ROUTE| FEC 319012         |0    |2097116 | 00:00:00:00:00:00 |  -  |183514|M 21346 524284
|2  |50.129.221.0/24   |ROUTE| FEC 318948         |0    |2097129 | 00:00:00:00:00:00 |  -  |183548|M 524293
|2  |50.130.32.0/24    |ROUTE| FEC 318986         |0    |2097135 | 00:00:00:00:00:00 |  -  |183554|M 378530
|2  |50.130.53.0/24    |ROUTE| FEC 24579          |0    |2097126 | 00:00:00:00:00:00 |  -  |183572|M 970002
|2  |50.130.120.0/24   |ROUTE| FEC 318840         |0    |2097142 | 00:00:00:00:00:00 |  -  |183582|M 1276
|2  |50.130.156.0/24   |ROUTE| FEC 24587          |0    |2097130 | 00:00:00:00:00:00 |  -  |183522|M 17
|2  |50.130.179.0/24   |ROUTE| FEC 318940         |0    |2097145 | 00:00:00:00:00:00 |  -  |183544|M 21
|2  |50.130.217.0/24   |ROUTE| FEC 319010         |0    |2097119 | 00:00:00:00:00:00 |  -  |183516|M 21347 524284
|2  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|2  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|3  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318966|   -   
|3  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|3  |192.168.20.0/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|3  |192.168.20.30/32  |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|3  |192.168.21.255/32 |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|3  |192.168.20.0/23   |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|3  |0.0.0.0/0         |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   

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
|24576|319074|ROUTE| Et21               |1027 |103460  | d0:48:a1:ba:3c:63 |Mpush 21249
|24576|319075|ROUTE| Et11               |1019 |103463  | d0:48:a1:ba:3c:61 |Mpush 21249
|24576|319076|ROUTE| Et11               |1019 |103463  | d0:48:a1:ba:3c:61 |Mpush 21249
|24576|319077|ROUTE| Et2                |1018 |103466  | d4:af:f7:2f:13:96 |Mpush 21249
|24576|319078|ROUTE| Et2                |1018 |103466  | d4:af:f7:2f:13:96 |Mpush 21249
|24576|319079|ROUTE| Et40               |1015 |103467  | e8:24:a6:96:05:48 |Mpush 21249
|24576|319080|ROUTE| Et40               |1015 |103467  | e8:24:a6:96:05:48 |Mpush 21249
|24576|319081|ROUTE| Et4                |1007 |103469  | c0:14:b8:21:97:90 |Mpush 21249
|24576|319082|ROUTE| Et4                |1007 |103469  | c0:14:b8:21:97:90 |Mpush 21249
|24576|319083|ROUTE| Et15               |1006 |103471  | 30:c5:07:84:3e:79 |Mpush 721249
|24576|319084|ROUTE| Et15               |1006 |103471  | 30:c5:07:84:3e:79 |Mpush 721249
|24576|319085|ROUTE| Et21               |1027 |103460  | d0:48:a1:ba:3c:63 |Mpush 21249
|24577|318856|ROUTE| Et18               |1013 |103450  | 64:6d:4e:32:e1:23 |   -   
|24577|318857|ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |   -   
|24577|318858|ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |   -   
|24577|318859|ROUTE| Et18               |1013 |103450  | 64:6d:4e:32:e1:23 |   -   
|24578|318778|ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |   -   
|24578|318779|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24578|318780|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24578|318781|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|24578|318782|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|24578|318783|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|24578|318784|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|24578|318785|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|24578|318786|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|24578|318787|ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |   -   
|24579|318884|ROUTE| Et3                |1017 |103529  | bc:31:e2:e1:ec:2c |Mpush 20053
|24579|318885|ROUTE| Et35               |1012 |103530  | 40:a6:b7:94:34:cb |Mpush 20053
|24579|318886|ROUTE| Et35               |1012 |103530  | 40:a6:b7:94:34:cb |Mpush 20053
|24579|318887|ROUTE| Et31               |1020 |103531  | e4:6d:7f:e3:c8:0a |Mpush 20053
|24579|318888|ROUTE| Et31               |1020 |103531  | e4:6d:7f:e3:c8:0a |Mpush 20053
|24579|318889|ROUTE| Et2                |1018 |103532  | d4:af:f7:2f:13:96 |Mpush 20053
|24579|318890|ROUTE| Et2                |1018 |103532  | d4:af:f7:2f:13:96 |Mpush 20053
|24579|318891|ROUTE| Et9                |1009 |103533  | e0:9b:27:c4:c5:84 |Mpush 20053
|24579|318892|ROUTE| Et9                |1009 |103533  | e0:9b:27:c4:c5:84 |Mpush 20053
|24579|318893|ROUTE| Et11               |1019 |103534  | d0:48:a1:ba:3c:61 |Mpush 20053
|24579|318894|ROUTE| Et11               |1019 |103534  | d0:48:a1:ba:3c:61 |Mpush 20053
|24579|318895|ROUTE| Et3                |1017 |103529  | bc:31:e2:e1:ec:2c |Mpush 20053
|24580|319014|ROUTE| Et20               |1025 |103475  | 60:53:75:13:ba:dd |   -   
|24580|319015|ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |   -   
|24580|319016|ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |   -   
|24580|319017|ROUTE| Et20               |1025 |103475  | 60:53:75:13:ba:dd |   -   
|24581|318812|ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |   -   
|24581|318813|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24581|318814|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24581|318815|ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |   -   
|24581|318816|ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |   -   
|24581|318817|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   
|24581|318818|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   
|24581|318819|ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |   -   
|24581|318820|ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |   -   
|24581|318821|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|24581|318822|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|24581|318823|ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |   -   
|24581|318824|ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |   -   
|24581|318825|ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |   -   
|24581|318826|ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |   -   
|24581|318827|ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |   -   
|24582|318844|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24582|318845|ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |   -   
|24582|318846|ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |   -   
|24582|318847|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24583|318802|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24583|318803|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|24583|318804|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|24583|318805|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24584|318972|ROUTE| Et2                |1018 |103445  | d4:af:f7:2f:13:96 |Mswap 20175
|24584|318973|ROUTE| Et11               |1019 |103432  | d0:48:a1:ba:3c:61 |Mswap 20175
|24584|318974|ROUTE| Et11               |1019 |103432  | d0:48:a1:ba:3c:61 |Mswap 20175
|24584|318975|ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |Mswap 20175
|24584|318976|ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |Mswap 20175
|24584|318977|ROUTE| Et31               |1020 |103439  | e4:6d:7f:e3:c8:0a |Mswap 20175
|24584|318978|ROUTE| Et31               |1020 |103439  | e4:6d:7f:e3:c8:0a |Mswap 20175
|24584|318979|ROUTE| Et9                |1009 |103441  | e0:9b:27:c4:c5:84 |Mswap 20175
|24584|318980|ROUTE| Et9                |1009 |103441  | e0:9b:27:c4:c5:84 |Mswap 20175
|24584|318981|ROUTE| Et35               |1012 |103462  | 40:a6:b7:94:34:cb |Mswap 20175
|24584|318982|ROUTE| Et35               |1012 |103462  | 40:a6:b7:94:34:cb |Mswap 20175
|24584|318983|ROUTE| Et2                |1018 |103445  | d4:af:f7:2f:13:96 |Mswap 20175
|24585|319088|ROUTE| Et11               |1019 |103485  | d0:48:a1:ba:3c:61 |Mswap 21249
|24585|319089|ROUTE| Et40               |1015 |103486  | e8:24:a6:96:05:48 |Mswap 21249
|24585|319090|ROUTE| Et40               |1015 |103486  | e8:24:a6:96:05:48 |Mswap 21249
|24585|319091|ROUTE| Et4                |1007 |103487  | c0:14:b8:21:97:90 |Mswap 21249
|24585|319092|ROUTE| Et4                |1007 |103487  | c0:14:b8:21:97:90 |Mswap 21249
|24585|319093|ROUTE| Et15               |1006 |103489  | 30:c5:07:84:3e:79 |Mswap 721249
|24585|319094|ROUTE| Et15               |1006 |103489  | 30:c5:07:84:3e:79 |Mswap 721249
|24585|319095|ROUTE| Et2                |1018 |103490  | d4:af:f7:2f:13:96 |Mswap 21249
|24585|319096|ROUTE| Et2                |1018 |103490  | d4:af:f7:2f:13:96 |Mswap 21249
|24585|319097|ROUTE| Et21               |1027 |103491  | d0:48:a1:ba:3c:63 |Mswap 21249
|24585|319098|ROUTE| Et21               |1027 |103491  | d0:48:a1:ba:3c:63 |Mswap 21249
|24585|319099|ROUTE| Et11               |1019 |103485  | d0:48:a1:ba:3c:61 |Mswap 21249
|24586|318870|ROUTE| Et2                |1018 |103493  | d4:af:f7:2f:13:96 |Mswap 21304
|24586|318871|ROUTE| Et40               |1015 |103494  | e8:24:a6:96:05:48 |Mswap 21304
|24586|318872|ROUTE| Et40               |1015 |103494  | e8:24:a6:96:05:48 |Mswap 21304
|24586|318873|ROUTE| Et4                |1007 |103496  | c0:14:b8:21:97:90 |Mswap 21304
|24586|318874|ROUTE| Et4                |1007 |103496  | c0:14:b8:21:97:90 |Mswap 21304
|24586|318875|ROUTE| Et11               |1019 |103497  | d0:48:a1:ba:3c:61 |Mswap 21304
|24586|318876|ROUTE| Et11               |1019 |103497  | d0:48:a1:ba:3c:61 |Mswap 21304
|24586|318877|ROUTE| Et21               |1027 |103498  | d0:48:a1:ba:3c:63 |Mswap 21304
|24586|318878|ROUTE| Et21               |1027 |103498  | d0:48:a1:ba:3c:63 |Mswap 21304
|24586|318879|ROUTE| Et15               |1006 |103500  | 30:c5:07:84:3e:79 |Mswap 721304
|24586|318880|ROUTE| Et15               |1006 |103500  | 30:c5:07:84:3e:79 |Mswap 721304
|24586|318881|ROUTE| Et2                |1018 |103493  | d4:af:f7:2f:13:96 |Mswap 21304
|24587|319004|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24587|319005|ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |   -   
|24587|319006|ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |   -   
|24587|319007|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24588|318896|ROUTE| Et11               |1019 |103535  | d0:48:a1:ba:3c:61 |Mpush 21182
|24588|318897|ROUTE| Et21               |1027 |103536  | d0:48:a1:ba:3c:63 |Mpush 21182
|24588|318898|ROUTE| Et21               |1027 |103536  | d0:48:a1:ba:3c:63 |Mpush 21182
|24588|318899|ROUTE| Et2                |1018 |103495  | d4:af:f7:2f:13:96 |Mpush 21182
|24588|318900|ROUTE| Et2                |1018 |103495  | d4:af:f7:2f:13:96 |Mpush 21182
|24588|318901|ROUTE| Et40               |1015 |103537  | e8:24:a6:96:05:48 |Mpush 21182
|24588|318902|ROUTE| Et40               |1015 |103537  | e8:24:a6:96:05:48 |Mpush 21182
|24588|318903|ROUTE| Et4                |1007 |103538  | c0:14:b8:21:97:90 |Mpush 21182
|24588|318904|ROUTE| Et4                |1007 |103538  | c0:14:b8:21:97:90 |Mpush 21182
|24588|318905|ROUTE| Et15               |1006 |103539  | 30:c5:07:84:3e:79 |Mpush 721182
|24588|318906|ROUTE| Et15               |1006 |103539  | 30:c5:07:84:3e:79 |Mpush 721182
|24588|318907|ROUTE| Et11               |1019 |103535  | d0:48:a1:ba:3c:61 |Mpush 21182
|24589|319102|ROUTE| Et3                |1017 |103516  | bc:31:e2:e1:ec:2c |Mswap 20053
|24589|319103|ROUTE| Et35               |1012 |103517  | 40:a6:b7:94:34:cb |Mswap 20053
|24589|319104|ROUTE| Et35               |1012 |103517  | 40:a6:b7:94:34:cb |Mswap 20053
|24589|319105|ROUTE| Et31               |1020 |103518  | e4:6d:7f:e3:c8:0a |Mswap 20053
|24589|319106|ROUTE| Et31               |1020 |103518  | e4:6d:7f:e3:c8:0a |Mswap 20053
|24589|319107|ROUTE| Et2                |1018 |103519  | d4:af:f7:2f:13:96 |Mswap 20053
|24589|319108|ROUTE| Et2                |1018 |103519  | d4:af:f7:2f:13:96 |Mswap 20053
|24589|319109|ROUTE| Et11               |1019 |103520  | d0:48:a1:ba:3c:61 |Mswap 20053
|24589|319110|ROUTE| Et11               |1019 |103520  | d0:48:a1:ba:3c:61 |Mswap 20053
|24589|319111|ROUTE| Et9                |1009 |103521  | e0:9b:27:c4:c5:84 |Mswap 20053
|24589|319112|ROUTE| Et9                |1009 |103521  | e0:9b:27:c4:c5:84 |Mswap 20053
|24589|319113|ROUTE| Et3                |1017 |103516  | bc:31:e2:e1:ec:2c |Mswap 20053
|24590|319114|ROUTE| Et4                |1007 |103522  | c0:14:b8:21:97:90 |Mswap 21182
|24590|319115|ROUTE| Et15               |1006 |103523  | 30:c5:07:84:3e:79 |Mswap 721182
|24590|319116|ROUTE| Et15               |1006 |103523  | 30:c5:07:84:3e:79 |Mswap 721182
|24590|319117|ROUTE| Et2                |1018 |103524  | d4:af:f7:2f:13:96 |Mswap 21182
|24590|319118|ROUTE| Et2                |1018 |103524  | d4:af:f7:2f:13:96 |Mswap 21182
|24590|319119|ROUTE| Et40               |1015 |103525  | e8:24:a6:96:05:48 |Mswap 21182
|24590|319120|ROUTE| Et40               |1015 |103525  | e8:24:a6:96:05:48 |Mswap 21182
|24590|319121|ROUTE| Et11               |1019 |103526  | d0:48:a1:ba:3c:61 |Mswap 21182
|24590|319122|ROUTE| Et11               |1019 |103526  | d0:48:a1:ba:3c:61 |Mswap 21182
|24590|319123|ROUTE| Et21               |1027 |103527  | d0:48:a1:ba:3c:63 |Mswap 21182
|24590|319124|ROUTE| Et21               |1027 |103527  | d0:48:a1:ba:3c:63 |Mswap 21182
|24590|319125|ROUTE| Et4                |1007 |103522  | c0:14:b8:21:97:90 |Mswap 21182
|  -  |183502|ROUTE| FEC 319052         |   - |  -     |                   |   -   
|  -  |183504|ROUTE| FEC 319012         |   - |2097124 |                 - |Mpush 20217 524287
|  -  |183506|ROUTE| FEC 318794         |   - |2097128 |                 - |Mpush 378528
|  -  |183508|ROUTE| FEC 318942         |   - |2097134 |                 - |Mpush 18
|  -  |183510|ROUTE| FEC 319012         |   - |2097124 |                 - |Mpush 20217 524287
|  -  |183512|ROUTE| FEC 319086         |   - |2097131 |                 - |Mpush 21345 524284
|  -  |183514|ROUTE| FEC 319012         |   - |2097116 |                 - |Mpush 21346 524284
|  -  |183516|ROUTE| FEC 319010         |   - |2097119 |                 - |Mpush 21347 524284
|  -  |183518|ROUTE| FEC 319030         |   - |2097139 |                 - |Mpush 20084 720898
|  -  |183520|ROUTE| FEC 24579          |   - |2097122 |                 - |Mpush 970000
|  -  |183522|ROUTE| FEC 24587          |   - |2097130 |                 - |Mpush 17
|  -  |183524|ROUTE| FEC 24587          |   - |2097138 |                 - |Mpush 16
|  -  |183526|ROUTE| FEC 24587          |   - |2097130 |                 - |Mpush 17
|  -  |183528|ROUTE| FEC 24587          |   - |2097130 |                 - |Mpush 17
|  -  |183530|ROUTE| FEC 318942         |   - |2097134 |                 - |Mpush 18
|  -  |183532|ROUTE| FEC 319048         |   - |2097114 |                 - |Mpush 378530
|  -  |183534|ROUTE| FEC 319030         |   - |2097137 |                 - |Mpush 20084 720899
|  -  |183536|ROUTE| FEC 318998         |   - |2097133 |                 - |Mpush 524292
|  -  |183538|ROUTE| FEC 319038         |   - |2097148 |                 - |Mpush 62000
|  -  |183540|ROUTE| FEC 318808         |   - |2097117 |                 - |Mpush 378530
|  -  |183542|ROUTE| FEC 318840         |   - |2097151 |                 - |Mpush 1279
|  -  |183544|ROUTE| FEC 318940         |   - |2097145 |                 - |Mpush 21
|  -  |183546|ROUTE| FEC 24587          |   - |2097138 |                 - |Mpush 16
|  -  |183548|ROUTE| FEC 318948         |   - |2097129 |                 - |Mpush 524293
|  -  |183550|ROUTE| FEC 318866         |   - |2097150 |                 - |Mpush 20214 500000
|  -  |183552|ROUTE| FEC 318866         |   - |2097150 |                 - |Mpush 20214 500000
|  -  |183554|ROUTE| FEC 318986         |   - |2097135 |                 - |Mpush 378530
|  -  |183556|ROUTE| FEC 319034         |   - |2097146 |                 - |Mpush 62000
|  -  |183558|ROUTE| FEC 318994         |   - |  -     |                   |   -   
|  -  |183560|ROUTE| FEC 318940         |   - |2097127 |                 - |Mpush 16
|  -  |183562|ROUTE| FEC 318796         |   - |2097118 |                 - |Mpush 21
|  -  |183564|ROUTE| FEC 318964         |   - |2097112 |                 - |Mpush 21
|  -  |183566|ROUTE| FEC 318940         |   - |2097127 |                 - |Mpush 16
|  -  |183568|ROUTE| FEC 318798         |   - |  -     |                   |   -   
|  -  |183570|ROUTE| FEC 318994         |   - |2097115 |                 - |Mpush 970002
|  -  |183572|ROUTE| FEC 24579          |   - |2097126 |                 - |Mpush 970002
|  -  |183574|ROUTE| FEC 24588          |   - |2097121 |                 - |Mpush 970002
|  -  |183576|ROUTE| FEC 318794         |   - |2097125 |                 - |Mpush 378529
|  -  |183578|ROUTE| FEC 24576          |   - |2097149 |                 - |Mpush 1277
|  -  |183580|ROUTE| FEC 318798         |   - |2097143 |                 - |Mpush 1278
|  -  |183582|ROUTE| FEC 318840         |   - |2097142 |                 - |Mpush 1276
|  -  |314666|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |314667|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |314669|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |314671|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |315677|TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |   -   
|  -  |315678|TRAP | CoppSystemL3DstMiss|1007 |1007    | ArpTrap           |   -   
|  -  |315679|TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |   -   
|  -  |315680|TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |   -   
|  -  |315681|TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |   -   
|  -  |315683|TRAP | CoppSystemL3DstMiss|1012 |1012    | ArpTrap           |   -   
|  -  |315684|TRAP | CoppSystemL3DstMiss|1013 |1013    | ArpTrap           |   -   
|  -  |315685|TRAP | CoppSystemL3DstMiss|1014 |1014    | ArpTrap           |   -   
|  -  |315686|TRAP | CoppSystemL3DstMiss|1015 |1015    | ArpTrap           |   -   
|  -  |315687|TRAP | CoppSystemL3DstMiss|1016 |1016    | ArpTrap           |   -   
|  -  |315688|TRAP | CoppSystemL3DstMiss|1017 |1017    | ArpTrap           |   -   
|  -  |315689|TRAP | CoppSystemL3DstMiss|1018 |1018    | ArpTrap           |   -   
|  -  |315690|TRAP | CoppSystemL3DstMiss|1019 |1019    | ArpTrap           |   -   
|  -  |315691|TRAP | CoppSystemL3DstMiss|1020 |1020    | ArpTrap           |   -   
|  -  |315692|TRAP | CoppSystemL3DstMiss|1021 |1021    | ArpTrap           |   -   
|  -  |315694|TRAP | CoppSystemL3DstMiss|1023 |1023    | ArpTrap           |   -   
|  -  |315696|TRAP | CoppSystemL3DstMiss|1025 |1025    | ArpTrap           |   -   
|  -  |315698|TRAP | CoppSystemL3DstMiss|1027 |1027    | ArpTrap           |   -   
|  -  |318768|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|  -  |318769|ROUTE| Et2                |1018 |103438  | d4:af:f7:2f:13:96 |Mpush 20575 20556
|  -  |318770|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|  -  |318772|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318774|ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |   -   
|  -  |318776|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|  -  |318794|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |318795|ROUTE| Et40               |1015 |103451  | e8:24:a6:96:05:48 |Mpush 20032
|  -  |318796|ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |   -   
|  -  |318797|ROUTE| Et15               |1006 |103504  | 30:c5:07:84:3e:79 |Mpush 721303 21307
|  -  |318798|ROUTE| Et15               |1006 |103482  | 30:c5:07:84:3e:79 |Mpush 721248
|  -  |318799|ROUTE| Et4                |1007 |103484  | c0:14:b8:21:97:90 |Mpush 524283 21248
|  -  |318800|ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |   -   
|  -  |318806|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |318808|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |318809|ROUTE| Et15               |1006 |103506  | 30:c5:07:84:3e:79 |Mpush 721303 20161
|  -  |318810|ROUTE| Et5                |1008 |103423  | 18:5b:00:61:ac:6f |   -   
|  -  |318836|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|  -  |318838|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   
|  -  |318840|ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |   -   
|  -  |318842|ROUTE| Et19               |1021 |103428  | 60:53:75:13:ba:d8 |   -   
|  -  |318848|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|  -  |318850|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|  -  |318852|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   
|  -  |318854|ROUTE| Et15               |1006 |103424  | 30:c5:07:84:3e:79 |   -   
|  -  |318860|ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |   -   
|  -  |318862|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|  -  |318864|ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |   -   
|  -  |318866|ROUTE| Et5                |1008 |103423  | 18:5b:00:61:ac:6f |   -   
|  -  |318867|ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |   -   
|  -  |318868|ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |   -   
|  -  |318882|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |318910|ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |   -   
|  -  |318922|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318924|ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |   -   
|  -  |318926|ROUTE| Et5                |1008 |103423  | 18:5b:00:61:ac:6f |   -   
|  -  |318928|ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |   -   
|  -  |318930|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |318936|ROUTE| Et17               |1016 |103443  | 64:6d:4e:32:e1:22 |   -   
|  -  |318938|ROUTE| Et18               |1013 |103450  | 64:6d:4e:32:e1:23 |   -   
|  -  |318940|ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |   -   
|  -  |318942|ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |   -   
|  -  |318943|ROUTE| Et40               |1015 |103442  | e8:24:a6:96:05:48 |Mpush 20131
|  -  |318948|ROUTE| Et15               |1006 |103424  | 30:c5:07:84:3e:79 |   -   
|  -  |318949|ROUTE| Et4                |1007 |103456  | c0:14:b8:21:97:90 |Mpush 21350
|  -  |318950|ROUTE| Et15               |1006 |103424  | 30:c5:07:84:3e:79 |   -   
|  -  |318952|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |318954|ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |   -   
|  -  |318956|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318958|ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |   -   
|  -  |318960|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|  -  |318962|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |318964|ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |   -   
|  -  |318965|ROUTE| Et21               |1027 |103575  | d0:48:a1:ba:3c:63 |Mpush 21308
|  -  |318966|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318968|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318970|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318986|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |318988|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|  -  |318989|ROUTE| Et2                |1018 |103458  | d4:af:f7:2f:13:96 |Mpush 21703 21684
|  -  |318990|ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |   -   
|  -  |318992|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   
|  -  |318994|ROUTE| Et15               |1006 |103542  | 30:c5:07:84:3e:79 |Mpush 721181
|  -  |318995|ROUTE| Et4                |1007 |103543  | c0:14:b8:21:97:90 |Mpush 524283 21181
|  -  |318996|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |318998|ROUTE| Et15               |1006 |103424  | 30:c5:07:84:3e:79 |   -   
|  -  |318999|ROUTE| Et40               |1015 |103435  | e8:24:a6:96:05:48 |Mpush 20221
|  -  |319000|ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |   -   
|  -  |319008|ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |   -   
|  -  |319010|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |319012|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |319013|ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |   -   
|  -  |319018|ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |   -   
|  -  |319020|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |319022|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|  -  |319023|ROUTE| Et2                |1018 |103449  | d4:af:f7:2f:13:96 |Mpush 21685
|  -  |319026|ROUTE| Et15               |1006 |103424  | 30:c5:07:84:3e:79 |   -   
|  -  |319028|ROUTE| Et3                |1017 |103478  | bc:31:e2:e1:ec:2c |   -   
|  -  |319030|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|  -  |319031|ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |   -   
|  -  |319032|ROUTE| Et5                |1008 |103423  | 18:5b:00:61:ac:6f |   -   
|  -  |319034|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   
|  -  |319035|ROUTE| Et40               |1015 |103444  | e8:24:a6:96:05:48 |Mpush 20066
|  -  |319036|ROUTE| Et15               |1006 |103424  | 30:c5:07:84:3e:79 |   -   
|  -  |319037|ROUTE| Et17               |1016 |103461  | 64:6d:4e:32:e1:22 |Mpush 404 21349
|  -  |319038|ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |   -   
|  -  |319039|ROUTE| Et40               |1015 |103452  | e8:24:a6:96:05:48 |Mpush 20072
|  -  |319042|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |319044|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|  -  |319046|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|  -  |319048|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |319049|ROUTE| Et4                |1007 |103473  | c0:14:b8:21:97:90 |Mpush 20162
|  -  |319050|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|  -  |319052|ROUTE| Et15               |1006 |103440  | 30:c5:07:84:3e:79 |Mpush 721303
|  -  |319053|ROUTE| Et4                |1007 |103544  | c0:14:b8:21:97:90 |Mpush 524283
|  -  |319054|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |319066|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |319070|ROUTE| Et20               |1025 |103475  | 60:53:75:13:ba:dd |   -   
|  -  |319072|ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |   -   
|  -  |319086|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |319087|ROUTE| Et15               |1006 |103446  | 30:c5:07:84:3e:79 |Mpush 721303
|  -  |319100|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   

```

