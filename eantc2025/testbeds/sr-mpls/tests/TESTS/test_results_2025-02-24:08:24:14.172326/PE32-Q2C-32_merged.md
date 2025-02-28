# Test results for PE32-Q2C-32

## show version

```text
Arista DCS-7280SR3K-48YC8-F
Hardware version: 10.05
Serial number: JAS20300015
Hardware MAC address: d4af.f72f.1396
System MAC address: d4af.f72f.1396

Software image version: 4.33.1.1F
Architecture: x86_64
Internal build version: 4.33.1.1F-40155285.43311F
Internal build ID: 2170da2c-90c5-421e-adc1-86266708cffc
Image format version: 3.0
Image optimization: Default

Uptime: 1 week, 0 days, 1 hour and 31 minutes
Total memory: 65734472 kB
Free memory: 61726800 kB

```

## show interfaces counters rates | nz

```text
Port      Name                 Intvl  In Mbps      %  In Kpps Out Mbps      %

Port      Out Kpps
```

## show ip interface brief | exclude una

```text
                                                                        Address
Interface        IP Address          Status        Protocol       MTU   Owner  
---------------- ------------------- ------------- ----------- -------- -------
Ethernet1        20.30.32.32/24      up            up            1500          
Ethernet2        21.30.32.32/24      admin down    down          1500          
Ethernet5        20.32.175.32/24     up            up            1500          
Ethernet40.4     50.10.32.1/24       up            up            1500          
Ethernet40.128   50.128.32.1/24      up            up            1500          
Ethernet40.129   50.129.32.1/24      up            up            1500          
Ethernet40.130   50.130.32.1/24      up            up            1500          
Loopback0        10.0.0.32/32        up            up           65535          
Management1      192.168.20.32/23    up            up            1500          

```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
IGP       default  Arista-Spine3-Q2A-30 L2   Ethernet1          P2P               UP    21          79                  
IGP       default  Juniper-175-ACX7100-48L L2   Ethernet5          P2P               UP    26          01                  
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
      IS Neighbor (MT-IPv6): H3C_M1A_120.00      Metric: 10
        IPv6 Neighbor Address: 2001:0:30:120::120
        Global IPv6 Interface Address: 2001:0:30:120::30
        Adj-sid: 378598 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Ericsson_84_R6678.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:84::175
        Global IPv6 Interface Address: 2001:0:30:84::30
        Adj-sid: 378587 flags: [L V F] weight: 0x0
    Arista-PE32-Q2C-32.00-00       780  32665   851    592 L2  0000.0000.0032.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 551 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
      Hostname: 221
    221.00-02                  9068  40768   846    483 L2  0221.0221.0221.00-02  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
    Arista-Spine3-Q2A-30.00-01       909   7244   978   1086 L2  0000.0000.0030.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 551 s
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
    Ericsson_84_R6678.00-00       828  16588  1049    324 L2  0000.0000.0084.00-00  <>
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
    H3C_M1A_120.00-00          4124  14887   843   1436 L2  0000.0000.0120.00-00  <>
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
            Administrative group (Color): JUNIPER(1)
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
    H3C_M1A_120.00-01           370  31719   841    357 L2  0000.0000.0120.00-01  <>
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
    Juniper-156-PTX10002-36QDD.00-00       612  53877  1131   1014 L2  0000.0000.0156.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
    Juniper-175-ACX7100-48L.00-00       972  38906   960   1178 L2  0000.0000.0175.00-00  <>
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      Reachability (MT-IPv6): 2001:0:131:175::/64 Metric: 10 Type: 1 Up
    Juniper-179-ACX7024.00-00       720  31209   830    543 L2  0000.0000.0179.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
            Administrative group (Color): JUNIPER(1)
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
    Nokia-SR1-217.00-00        1105  16143   929    594 L2  0100.0000.0217.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
            Administrative group (Color): JUNIPER(1)
            TE default metric: 10
            Maximum link BW: 10.00 Gbps
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): JUNIPER(1)
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
    221.00-00                   720  65427   681     85 L2  0221.0221.0221.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
    221.00-01                   652  49185   845     32 L2  0221.0221.0221.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      Hostname: 221
    221.00-02                  9068  40768   845    483 L2  0221.0221.0221.00-02  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
        Administrative group (Color): JUNIPER(1)
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
            Administrative group (Color): JUNIPER(1)
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
  Destination                      Algorithm         Next Hop         Interface
------------------------------- ----------------- ------------------- ---------
  221                              MIN-LATENCY       20.30.32.30      Ethernet1
                                                                               
  221                              MIN-TE            20.32.175.175    Ethernet5
                                                                               
  Arista-PE32-Q2C-32               MIN-LATENCY                                 
                                                                               
  Arista-PE32-Q2C-32               MIN-TE                                      
                                                                               
  Arista-PE32-Q2C-32               ADMIN                                       
                                                                               
  Arista-Spine3-Q2A-30             MIN-LATENCY       20.30.32.30      Ethernet1
                                                                               
  Arista-Spine3-Q2A-30             MIN-TE            20.32.175.175    Ethernet5
                                                                               
  Arista-Spine3-Q2A-30             ADMIN             20.30.32.30      Ethernet1
                                                                               
  Arrcus-53                        MIN-LATENCY       20.30.32.30      Ethernet1
                                                                               
  Arrcus-53                        MIN-TE            20.32.175.175    Ethernet5
                                                                               
  Arrcus-53                        ADMIN                                       
                                                                               
  Ciena-5134-72                    MIN-TE                                      
                                                                               
  Ciena-8140-66                    MIN-TE                                      
                                                                               
  H3C_M1A_120                      MIN-LATENCY       20.30.32.30      Ethernet1
                                                                               
  H3C_M1A_120                      MIN-TE            20.32.175.175    Ethernet5
                                                                               
  H3C_M1A_120                      ADMIN                                       
                                                                               
  Juniper-156-PTX10002-36QDD       MIN-LATENCY       20.30.32.30      Ethernet1
                                                                               
  Juniper-156-PTX10002-36QDD       MIN-TE            20.32.175.175    Ethernet5
                                                                               
  Juniper-156-PTX10002-36QDD       ADMIN             20.30.32.30      Ethernet1
                                                                               
  Juniper-175-ACX7100-48L          MIN-LATENCY       20.30.32.30      Ethernet1
                                                                               
  Juniper-175-ACX7100-48L          MIN-TE            20.32.175.175    Ethernet5
                                                                               
  Juniper-175-ACX7100-48L          ADMIN             20.30.32.30      Ethernet1
                                                                               
  Juniper-179-ACX7024              MIN-LATENCY       20.30.32.30      Ethernet1
                                                                               
  Juniper-179-ACX7024              MIN-TE            20.32.175.175    Ethernet5
                                                                               
  Juniper-179-ACX7024              ADMIN             20.30.32.30      Ethernet1
                                                                               
  Nokia-SR1-217                    MIN-LATENCY       20.30.32.30      Ethernet1
                                                                               
  Nokia-SR1-217                    MIN-TE            20.32.175.175    Ethernet5
                                                                               
  Nokia-SR1-217                    ADMIN             20.30.32.30      Ethernet1
                                                                               

Flex algo paths for IPv6 address family
Topology ID: Level-2
Destination                  Algorithm     Next Hop                   Interface
--------------------------- ------------- --------------------------- ---------
Arista-Spine3-Q2A-30         MIN-LATENCY   fe80::c6ca:2bff:fe45:a215  Ethernet1
                                                                               
Arista-Spine3-Q2A-30         MIN-TE        fe80::c6ca:2bff:fe45:a215  Ethernet1
                                                                               
Arista-Spine3-Q2A-30         ADMIN         fe80::c6ca:2bff:fe45:a215  Ethernet1
                                                                               
Arrcus-53                    MIN-LATENCY   fe80::3e08:cdff:fe8d:badc  Ethernet5
                                                                               
Arrcus-53                    MIN-TE        fe80::3e08:cdff:fe8d:badc  Ethernet5
                                                                               
Arrcus-53                    ADMIN                                             
                                                                               
H3C_M1A_120                  MIN-LATENCY                                       
                                                                               
H3C_M1A_120                  MIN-TE                                            
                                                                               
H3C_M1A_120                  ADMIN                                             
                                                                               
Juniper-156-PTX10002-36QDD   MIN-LATENCY   fe80::c6ca:2bff:fe45:a215  Ethernet1
                                                                               
Juniper-156-PTX10002-36QDD   MIN-TE        fe80::3e08:cdff:fe8d:badc  Ethernet5
                                                                               
Juniper-156-PTX10002-36QDD   ADMIN         fe80::c6ca:2bff:fe45:a215  Ethernet1
                                                                               
Juniper-175-ACX7100-48L      MIN-LATENCY   fe80::3e08:cdff:fe8d:badc  Ethernet5
                                                                               
Juniper-175-ACX7100-48L      MIN-TE        fe80::3e08:cdff:fe8d:badc  Ethernet5
                                                                               
Juniper-175-ACX7100-48L      ADMIN         fe80::c6ca:2bff:fe45:a215  Ethernet1
                                                                               

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
Metric: 20000
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: 221
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2
Last updated: 2 days, 15:05:36 ago
Metric: 20
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Arista-PE32-Q2C-32
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 23:15:55 ago
Next Hop Interface
-------- ---------

Destination: Arista-PE32-Q2C-32
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 23:15:55 ago
Next Hop Interface
-------- ---------

Destination: Arista-PE32-Q2C-32
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 23:15:55 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
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
20.30.32.30 Ethernet1

Destination: Arista-Spine3-Q2A-30
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 3
Last updated: 2 days, 15:05:36 ago
Metric: 30
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Arista-Spine3-Q2A-30
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 12
Last updated: 2 days, 15:40:12 ago
Metric: 10
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: Arrcus-53
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 26
Last updated: 0:05:56 ago
Metric: 120010
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: Arrcus-53
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 17:53:55 ago
Metric: 20
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Arrcus-53
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 27
Last updated: 0:05:56 ago
Next Hop Interface
-------- ---------

Destination: Ciena-5134-72
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2
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
Metric: 120010
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: H3C_M1A_120
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 14:19:03 ago
Metric: 20
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: H3C_M1A_120
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
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
Number of times path updated: 14
Last updated: 2 days, 15:40:12 ago
Metric: 20000
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: Juniper-156-PTX10002-36QDD
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 17:53:55 ago
Metric: 20
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Juniper-156-PTX10002-36QDD
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 12
Last updated: 2 days, 15:40:12 ago
Metric: 11
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: Juniper-175-ACX7100-48L
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 18
Last updated: 2 days, 15:05:36 ago
Metric: 20010
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: Juniper-175-ACX7100-48L
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 17:53:55 ago
Metric: 10
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Juniper-175-ACX7100-48L
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 12
Last updated: 2 days, 15:40:12 ago
Metric: 21
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: Juniper-179-ACX7024
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 14
Last updated: 2 days, 15:40:12 ago
Metric: 20000
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: Juniper-179-ACX7024
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 17:53:55 ago
Metric: 20
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Juniper-179-ACX7024
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 12
Last updated: 2 days, 15:40:12 ago
Metric: 11
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: Nokia-SR1-217
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 24
Last updated: 2 days, 15:40:12 ago
Metric: 20000
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: Nokia-SR1-217
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 17:53:55 ago
Metric: 20
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Nokia-SR1-217
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 22
Last updated: 2 days, 15:40:12 ago
Metric: 11
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Flex algo paths for IPv6 address family
Topology ID: Level-2
Destination: Arista-Spine3-Q2A-30
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 12
Last updated: 2 days, 15:40:12 ago
Metric: 10000
Next Hop                  Interface
------------------------- ---------
fe80::c6ca:2bff:fe45:a215 Ethernet1

Destination: Arista-Spine3-Q2A-30
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 12
Last updated: 2 days, 15:40:12 ago
Metric: 100
Next Hop                  Interface
------------------------- ---------
fe80::c6ca:2bff:fe45:a215 Ethernet1

Destination: Arista-Spine3-Q2A-30
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 10
Last updated: 2 days, 15:40:12 ago
Metric: 10
Next Hop                  Interface
------------------------- ---------
fe80::c6ca:2bff:fe45:a215 Ethernet1

Destination: Arrcus-53
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 25
Last updated: 0:05:56 ago
Metric: 200000
Next Hop                  Interface
------------------------- ---------
fe80::3e08:cdff:fe8d:badc Ethernet5

Destination: Arrcus-53
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 17:53:55 ago
Metric: 20
Next Hop                  Interface
------------------------- ---------
fe80::3e08:cdff:fe8d:badc Ethernet5

Destination: Arrcus-53
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 23
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
Last updated: 2 days, 14:19:04 ago
Next Hop Interface
-------- ---------

Destination: H3C_M1A_120
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 14:19:04 ago
Next Hop Interface
-------- ---------

Destination: H3C_M1A_120
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 14:19:04 ago
Next Hop Interface
-------- ---------

Destination: Juniper-156-PTX10002-36QDD
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 14
Last updated: 2 days, 15:40:12 ago
Metric: 20000
Next Hop                  Interface
------------------------- ---------
fe80::c6ca:2bff:fe45:a215 Ethernet1

Destination: Juniper-156-PTX10002-36QDD
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 17:53:55 ago
Metric: 20
Next Hop                  Interface
------------------------- ---------
fe80::3e08:cdff:fe8d:badc Ethernet5

Destination: Juniper-156-PTX10002-36QDD
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 12
Last updated: 2 days, 15:40:12 ago
Metric: 20
Next Hop                  Interface
------------------------- ---------
fe80::c6ca:2bff:fe45:a215 Ethernet1

Destination: Juniper-175-ACX7100-48L
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 25
Last updated: 0:05:56 ago
Metric: 100000
Next Hop                  Interface
------------------------- ---------
fe80::3e08:cdff:fe8d:badc Ethernet5

Destination: Juniper-175-ACX7100-48L
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2 days, 17:53:55 ago
Metric: 10
Next Hop                  Interface
------------------------- ---------
fe80::3e08:cdff:fe8d:badc Ethernet5

Destination: Juniper-175-ACX7100-48L
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 26
Last updated: 2 days, 15:40:12 ago
Metric: 30
Next Hop                  Interface
------------------------- ---------
fe80::c6ca:2bff:fe45:a215 Ethernet1

```

## show isis segment-routing tunnel

```text
 Index    Endpoint          Next Hop/Tunnel Index         Interface   Labels   
-------- ---------------- ----------------------------- ------------- ---------
 1        10.0.0.175/32     TI-LFA (16)                   -           [ 3 ]    
 2        10.0.0.84/32      TI-LFA (0)                    -           [ 20084 ]
 5        10.0.0.30/32      TI-LFA (1)                    -           [ 3 ]    
 6        10.0.0.53/32      TI-LFA (6)                    -           [ 20053 ]
 7        10.0.0.179/32     TI-LFA (0)                    -           [ 20179 ]
 8        10.0.0.120/32     TI-LFA (0)                    -           [ 20120 ]
 9        10.0.0.72/32      TI-LFA (0)                    -           [ 20072 ]
 10       10.0.0.214/32     TI-LFA (0)                    -           [ 20214 ]
 12       10.0.0.131/32     TI-LFA (0)                    -           [ 20131 ]
 13       10.0.0.221/32     TI-LFA (0)                    -           [ 20221 ]
 16       10.0.0.217/32     TI-LFA (0)                    -           [ 20217 ]
 17       10.0.0.66/32      TI-LFA (0)                    -           [ 20066 ]
 18       10.0.0.156/32     TI-LFA (0)                    -           [ 20156 ]
 20       2002::30/128      fe80::c6ca:2bff:fe45:a215     Ethernet1   [ 3 ]    
 21       2002::53/128      fe80::3e08:cdff:fe8d:badc     Ethernet5   [ 20453 ]
 22       2002::175/128     fe80::3e08:cdff:fe8d:badc     Ethernet5   [ 3 ]    
 25       2002::156/128     fe80::3e08:cdff:fe8d:badc     Ethernet5   [ 20556 ]
                            fe80::c6ca:2bff:fe45:a215     Ethernet1   [ 20556 ]
 27       2002::120/128     fe80::3e08:cdff:fe8d:badc     Ethernet5   [ 20520 ]
                            fe80::c6ca:2bff:fe45:a215     Ethernet1   [ 20520 ]

```

## show isis segment-routing prefix-segments

```text

System ID: Arista-PE32-Q2C-32			Instance: 'IGP'
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.32

Node: 62     Proxy-Node: 0      Prefix: 0       Total Segments: 62

Flag Descriptions: R: Re-advertised, N: Node Segment, P: no-PHP
                   E: Explicit-NULL, V: Value, L: Local
Segment status codes: * - Self originated Prefix, L1 - level 1, L2 - level 2, ! - SR-unreachable,
                      # - Some IS-IS next-hops are SR-unreachable
   Prefix                      SID   Label Type       Flags                        System ID       Level Protection  Algorithm   
   ------------------------- ----- ------- ---------- ---------------------------- --------------- ----- ----------- -------------
   10.0.0.30/32                 30   20030 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node with SRLG strict SPF         
   10.0.0.30/32                158   20158 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node with SRLG strict MIN-LATENCY 
   10.0.0.30/32                159   20159 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node with SRLG strict MIN-TE      
   10.0.0.30/32                160   20160 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node with SRLG strict ADMIN       
*  10.0.0.32/32                 32   20032 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected SPF         
*  10.0.0.32/32                161   20161 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected MIN-LATENCY 
*  10.0.0.32/32                162   20162 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected MIN-TE      
*  10.0.0.32/32                163   20163 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected ADMIN       
   10.0.0.53/32                 53   20053 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    node with SRLG strict SPF         
   10.0.0.53/32               1181   21181 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node with SRLG strict MIN-LATENCY 
   10.0.0.53/32               1182   21182 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node with SRLG strict MIN-TE      
   10.0.0.53/32               1183   21183 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    unprotected ADMIN       
   10.0.0.66/32                 66   20066 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-8140-66   L2    node with SRLG strict SPF         
   10.0.0.66/32               1195   21195 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-8140-66   L2    unprotected MIN-TE      
   10.0.0.72/32                 72   20072 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    node with SRLG strict SPF         
   10.0.0.72/32               1201   21201 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    unprotected MIN-TE      
   10.0.0.84/32                 84   20084 Node       R:0 N:1 P:1 E:0 V:0 L:0      Ericsson_84_R6678 L2    node with SRLG strict SPF         
   10.0.0.120/32               120   20120 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node with SRLG strict SPF         
   10.0.0.120/32              1248   21248 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node with SRLG strict MIN-LATENCY 
   10.0.0.120/32              1249   21249 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node with SRLG strict MIN-TE      
   10.0.0.120/32              1250   21250 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected ADMIN       
   10.0.0.131/32               131   20131 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-131-JCNR L2    node with SRLG strict SPF         
   10.0.0.156/32               156   20156 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node with SRLG strict SPF         
   10.0.0.156/32              1284   21284 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node with SRLG strict MIN-LATENCY 
   10.0.0.156/32              1285   21285 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node with SRLG strict MIN-TE      
   10.0.0.156/32              1286   21286 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node with SRLG strict ADMIN       
   10.0.0.175/32               175   20175 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node with SRLG strict SPF         
   10.0.0.175/32              1303   21303 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node with SRLG strict MIN-LATENCY 
   10.0.0.175/32              1304   21304 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node with SRLG strict MIN-TE      
   10.0.0.175/32              1305   21305 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node with SRLG strict ADMIN       
   10.0.0.179/32               179   20179 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node with SRLG strict SPF         
   10.0.0.179/32              1307   21307 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node with SRLG strict MIN-LATENCY 
   10.0.0.179/32              1308   21308 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node with SRLG strict MIN-TE      
   10.0.0.179/32              1309   21309 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node with SRLG strict ADMIN       
   10.0.0.214/32               214   20214 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node with SRLG strict SPF         
   10.0.0.217/32               217   20217 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node with SRLG strict SPF         
   10.0.0.217/32              1345   21345 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node with SRLG strict MIN-LATENCY 
   10.0.0.217/32              1346   21346 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node with SRLG strict MIN-TE      
   10.0.0.217/32              1347   21347 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node with SRLG strict ADMIN       
   10.0.0.221/32               221  720221 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node with SRLG strict SPF         
   10.0.0.221/32              1349  721349 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node with SRLG strict MIN-LATENCY 
   10.0.0.221/32              1350  721350 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node with SRLG strict MIN-TE      
   2002::30/128                430   20430 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node        SPF         
   2002::30/128                558   20558 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node        MIN-LATENCY 
   2002::30/128                559   20559 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node        MIN-TE      
   2002::30/128                560   20560 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node        ADMIN       
   2002::53/128                453   20453 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    node        SPF         
   2002::53/128               1581   21581 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        MIN-LATENCY 
   2002::53/128               1582   21582 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        MIN-TE      
   2002::53/128               1583   21583 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    unprotected ADMIN       
   2002::120/128               520   20520 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected SPF         
   2002::120/128              1648   21648 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected MIN-LATENCY 
   2002::120/128              1649   21649 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected MIN-TE      
   2002::120/128              1650   21650 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected ADMIN       
   2002::156/128               556   20556 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    unprotected SPF         
   2002::156/128              1684   21684 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        MIN-LATENCY 
   2002::156/128              1685   21685 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        MIN-TE      
   2002::156/128              1686   21686 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        ADMIN       
   2002::175/128               575   20575 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        SPF         
   2002::175/128              1703   21703 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        MIN-LATENCY 
   2002::175/128              1704   21704 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        MIN-TE      
   2002::175/128              1705   21705 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        ADMIN       
```

## show ip ospf segment-routing

```text
! OSPF (Instance Id: 1) Segment Routing has been administratively shutdown
```

## show ip ospf segment-routing global-blocks

```text
! OSPF (Instance Id: 1) Segment Routing has been administratively shutdown
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

 I L2     10.0.0.30/32 [115/10]
           via 20.30.32.30, Ethernet1
 C        10.0.0.32/32
           directly connected, Loopback0
 I L2     10.0.0.53/32 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.66/32 [115/21]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.72/32 [115/21]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.84/32 [115/21]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.120/32 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.124/32 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.128/32 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.131/32 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.156/32 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.175/32 [115/10]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.179/32 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.214/32 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.216/32 [115/21]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.217/32 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.221/32 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     10.0.1.179/32 [115/11]
           via 20.30.32.30, Ethernet1
 C        20.30.32.0/24
           directly connected, Ethernet1
 I L2     20.30.66.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     20.30.72.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     20.30.84.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     20.30.120.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     20.30.124.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     20.30.128.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     20.30.131.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     20.30.156.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     20.30.179.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     20.30.184.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     20.30.214.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     20.30.217.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     20.30.221.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 C        20.32.175.0/24
           directly connected, Ethernet5
 I L2     20.53.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.66.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.72.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.84.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.120.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.120.214.0/24 [115/21]
           via 20.30.32.30, Ethernet1
 I L2     20.120.217.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     20.124.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.128.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.131.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.156.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.175.179.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.175.184.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.175.214.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.175.217.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.175.221.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.214.216.0/24 [115/21]
           via 20.30.32.30, Ethernet1
 I L2     21.30.124.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     21.30.128.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     21.30.156.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     21.30.217.0/24 [115/11]
           via 20.30.32.30, Ethernet1
 I L2     192.168.20.0/23 [115/11]
           via 20.30.32.30, Ethernet1


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

 C        50.128.32.0/24
           directly connected, Ethernet40.128
 B I      50.128.53.0/24 [200/0]
           via 10.0.0.53/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 6, label 970002
              via TI-LFA tunnel index 0, label 21181
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.128.120.0/24 [200/0]
           via 10.0.0.120/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 44, label 1278
              via TI-LFA tunnel index 0, label 21248
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.128.156.0/24 [200/0]
           via 10.0.0.156/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 27, label 17
              via TI-LFA tunnel index 0, label 21284
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.128.179.0/24 [200/0]
           via 10.0.0.179/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 40, label 21
              via TI-LFA tunnel index 0, label 21307
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.128.217.0/24 [200/0]
           via 10.0.0.217/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 10, label 524284
              via TI-LFA tunnel index 0, label 21345
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 C        50.129.32.0/24
           directly connected, Ethernet40.129
 B I      50.129.53.0/24 [200/0]
           via 10.0.0.53/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 12, label 970002
              via TI-LFA tunnel index 3, label 21182
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label 21308
 B I      50.129.120.0/24 [200/0]
           via 10.0.0.120/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 45, label 1277
              via 20.32.175.175, Ethernet5, label 21249
 B I      50.129.156.0/24 [200/0]
           via 10.0.0.156/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 26, label 17
              via TI-LFA tunnel index 4, label 21285
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label imp-null(3)
 B I      50.129.179.0/24 [200/0]
           via 10.0.0.179/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 38, label 21
              via TI-LFA tunnel index 4, label 21308
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label imp-null(3)
 B I      50.129.217.0/24 [200/0]
           via 10.0.0.217/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 14, label 524284
              via TI-LFA tunnel index 4, label 21346
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label imp-null(3)
 B I      50.129.221.0/24 [200/0]
           via 10.0.0.221/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 15, label 524293
              via TI-LFA tunnel index 4, label 21350
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label imp-null(3)
 C        50.130.32.0/24
           directly connected, Ethernet40.130
 B I      50.130.53.0/24 [200/0]
           via 10.0.0.53/32, IS-IS SR tunnel index 6, label 970002
              via TI-LFA tunnel index 6, label 20053
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label 20156
 B I      50.130.120.0/24 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 8, label 1276
              via TI-LFA tunnel index 0, label 20120
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.130.156.0/24 [200/0]
           via 10.0.0.156/32, algorithm ADMIN, IS-IS FlexAlgo tunnel index 28, label 17
              via 20.30.32.30, Ethernet1, label 21286
 B I      50.130.179.0/24 [200/0]
           via 10.0.0.179/32, algorithm ADMIN, IS-IS FlexAlgo tunnel index 39, label 21
              via 20.30.32.30, Ethernet1, label 21309
 B I      50.130.217.0/24 [200/0]
           via 10.0.0.217/32, algorithm ADMIN, IS-IS FlexAlgo tunnel index 3, label 524284
              via 20.30.32.30, Ethernet1, label 21347


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

 C        50.10.32.0/24
           directly connected, Ethernet40.4
 B I      50.10.53.0/24 [200/0]
           via 10.0.0.53/32, IS-IS SR tunnel index 6, label 970000
              via TI-LFA tunnel index 6, label 20053
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label 20156
 B I      50.10.66.0/24 [200/0]
           via 10.0.0.66/32, IS-IS SR tunnel index 17, label 62000
              via TI-LFA tunnel index 0, label 20066
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.10.72.0/24 [200/0]
           via 10.0.0.72/32, IS-IS SR tunnel index 9, label 62000
              via TI-LFA tunnel index 0, label 20072
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.10.84.0/24 [200/0]
           via 10.0.0.84/32, IS-IS SR tunnel index 2, label 720898
              via TI-LFA tunnel index 0, label 20084
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.10.120.0/24 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 8, label 1279
              via TI-LFA tunnel index 0, label 20120
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.10.131.0/24 [200/0]
           via 10.0.0.131/32, IS-IS SR tunnel index 12, label 18
              via TI-LFA tunnel index 0, label 20131
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.10.156.0/24 [200/0]
           via 10.0.0.156/32, IS-IS SR tunnel index 18, label 16
              via TI-LFA tunnel index 0, label 20156
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.10.179.0/24 [200/0]
           via 10.0.0.179/32, IS-IS SR tunnel index 7, label 16
              via TI-LFA tunnel index 0, label 20179
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.10.214.0/24 [200/0]
           via 10.0.0.214/32, IS-IS SR tunnel index 10, label 500000
              via TI-LFA tunnel index 0, label 20214
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.10.217.0/24 [200/0]
           via 10.0.0.217/32, IS-IS SR tunnel index 16, label 524287
              via TI-LFA tunnel index 0, label 20217
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.10.221.0/24 [200/0]
           via 10.0.0.221/32, IS-IS SR tunnel index 13, label 524292
              via TI-LFA tunnel index 0, label 20221
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.129.66.0/24 [200/0]
           via 10.0.0.66/32, IS-IS SR tunnel index 17, label 62000
              via TI-LFA tunnel index 0, label 20066
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.129.72.0/24 [200/0]
           via 10.0.0.72/32, IS-IS SR tunnel index 9, label 62000
              via TI-LFA tunnel index 0, label 20072
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)


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
Displaying 40 of 45 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 I L2     2000::214/128 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 C        2001:0:30:32::/64 [0/0]
           via Ethernet1, directly connected
 I L2     2001:0:30:66::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:72::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:84::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:120::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:124::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:128::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:131::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:156::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:179::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:184::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:214::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:217::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:221::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 C        2001:0:32:175::/64 [0/0]
           via Ethernet5, directly connected
 I L2     2001:0:53:175::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:66:175::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:72:175::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:84:175::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:120:175::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:120:214::/64 [115/30]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:120:217::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:128:175::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:131:175::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:156:175::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:175::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:175:184::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:175:214::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:175:217::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:175:221::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:214:216::/64 [115/30]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2002::30/128 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 C        2002::32/128 [0/0]
           via Loopback0, directly connected
 I L2     2002::53/128 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2002::120/128 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2002::156/128 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2002::175/128 [115/10]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2002::216/128 [115/30]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2002::217/128 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
           via fe80::3e08:cdff:fe8d:badc, Ethernet5

```

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 57 routes 
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
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20030
 20053   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 6
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20156
 20066   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20072   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20084   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20120   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20131   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20156   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20158   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 10
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20158
 20159   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 11
                    via 20.32.175.175, Ethernet5, label 20159
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 20160   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.32.30 Ethernet1
 20175   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 16
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20217 20175
 20179   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20214   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20217   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20221   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20430   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::c6ca:2bff:fe45:a215 Ethernet1
 20453   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::3e08:cdff:fe8d:badc Ethernet5
 20520   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::c6ca:2bff:fe45:a215 Ethernet1
                    fe80::3e08:cdff:fe8d:badc Ethernet5
 20556   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::c6ca:2bff:fe45:a215 Ethernet1
                    fe80::3e08:cdff:fe8d:badc Ethernet5
 20558   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 12
                    via fe80::c6ca:2bff:fe45:a215, Ethernet1, label imp-null(3)
                    backup via fe80::3e08:cdff:fe8d:badc, Ethernet5, label 21684 20558
 20559   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 14
                    via fe80::c6ca:2bff:fe45:a215, Ethernet1, label imp-null(3)
                    backup via fe80::3e08:cdff:fe8d:badc, Ethernet5, label 21685 20559
 20560   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::c6ca:2bff:fe45:a215 Ethernet1
 20575   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::3e08:cdff:fe8d:badc Ethernet5
 21181   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21182   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 3
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 21308
 21248   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21249   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 21284   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21285   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 4
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 21286   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.32.30 Ethernet1
 21303   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 9
                    via 20.30.32.30, Ethernet1, label 21303
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21304   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 2
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 21308 21304
 21305   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.32.30 Ethernet1
 21307   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21308   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 4
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 21309   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.32.30 Ethernet1
 21345   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21346   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 4
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 21347   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.32.30 Ethernet1
 21349   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21350   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 4
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 21581   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 15
                    via fe80::3e08:cdff:fe8d:badc, Ethernet5, label imp-null(3)
                    backup via fe80::c6ca:2bff:fe45:a215, Ethernet1, label 21684
 21582   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 8
                    via fe80::3e08:cdff:fe8d:badc, Ethernet5, label imp-null(3)
                    backup via fe80::c6ca:2bff:fe45:a215, Ethernet1, label 21685
 21684   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 13
                    via fe80::c6ca:2bff:fe45:a215, Ethernet1, label imp-null(3)
                    backup via fe80::3e08:cdff:fe8d:badc, Ethernet5, label imp-null(3)
 21685   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 7
                    via fe80::3e08:cdff:fe8d:badc, Ethernet5, label imp-null(3)
                    backup via fe80::c6ca:2bff:fe45:a215, Ethernet1, label imp-null(3)
 21686   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::c6ca:2bff:fe45:a215 Ethernet1
 21703   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 19
                    via fe80::3e08:cdff:fe8d:badc, Ethernet5, label imp-null(3)
                    backup via fe80::c6ca:2bff:fe45:a215, Ethernet1, label 21684 21703
 21704   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 23
                    via fe80::3e08:cdff:fe8d:badc, Ethernet5, label imp-null(3)
                    backup via fe80::c6ca:2bff:fe45:a215, Ethernet1, label 21685 21704
 21705   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::c6ca:2bff:fe45:a215 Ethernet1
 362168  A[1]
                via M, 20.30.32.30, pop
                    EgressACL: apply
                    directly connected, Ethernet1
                    c4:ca:2b:45:a2:15, vlan 1006
 362169  A[1]
                via M, fe80::c6ca:2bff:fe45:a215, pop
                    EgressACL: apply
                    directly connected, Ethernet1
                    c4:ca:2b:45:a2:15, vlan 1006
 362170  A[1]
                via M, 20.32.175.175, pop
                    EgressACL: apply
                    directly connected, Ethernet5
                    3c:08:cd:8d:ba:dc, vlan 1010
 362171  A[1]
                via M, fe80::3e08:cdff:fe8d:badc, pop
                    EgressACL: apply
                    directly connected, Ethernet5
                    3c:08:cd:8d:ba:dc, vlan 1010
 378528   [0]
                via I, ipv4, vrf RED
 378529   [0]
                via I, ipv6, vrf RED
 378530   [0]
                via I, ipv4, vrf FLEXALGO
```

## show mpls lfib route

```text
MPLS forwarding table (Label [metric] Vias) - 57 routes 
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
                via TI-LFA tunnel index 1, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20030
 IP    20053    [1], 10.0.0.53/32
                via TI-LFA tunnel index 6, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20156
 IP    20066    [1], 10.0.0.66/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20072    [1], 10.0.0.72/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20084    [1], 10.0.0.84/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20120    [1], 10.0.0.120/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20131    [1], 10.0.0.131/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20156    [1], 10.0.0.156/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20158    [1], 10.0.0.30/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 10, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20158
 IP    20159    [1], 10.0.0.30/32, algorithm MIN-TE
                via TI-LFA tunnel index 11, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label 20159
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    20160    [1], 10.0.0.30/32, algorithm ADMIN
                via M, 20.30.32.30, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    20175    [1], 10.0.0.175/32
                via TI-LFA tunnel index 16, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20217 20175
 IP    20179    [1], 10.0.0.179/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20214    [1], 10.0.0.214/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20217    [1], 10.0.0.217/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20221    [1], 10.0.0.221/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20430    [1], 2002::30/128
                via M, fe80::c6ca:2bff:fe45:a215, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    20453    [1], 2002::53/128
                via M, fe80::3e08:cdff:fe8d:badc, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    20520    [1], 2002::120/128
                via M, fe80::3e08:cdff:fe8d:badc, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
                via M, fe80::c6ca:2bff:fe45:a215, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    20556    [1], 2002::156/128
                via M, fe80::3e08:cdff:fe8d:badc, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
                via M, fe80::c6ca:2bff:fe45:a215, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    20558    [1], 2002::30/128, algorithm MIN-LATENCY
                via TI-LFA tunnel index 12, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::c6ca:2bff:fe45:a215, Ethernet1, label imp-null(3)
                    backup via fe80::3e08:cdff:fe8d:badc, Ethernet5, label 21684 20558
 IP    20559    [1], 2002::30/128, algorithm MIN-TE
                via TI-LFA tunnel index 14, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::c6ca:2bff:fe45:a215, Ethernet1, label imp-null(3)
                    backup via fe80::3e08:cdff:fe8d:badc, Ethernet5, label 21685 20559
 IP    20560    [1], 2002::30/128, algorithm ADMIN
                via M, fe80::c6ca:2bff:fe45:a215, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    20575    [1], 2002::175/128
                via M, fe80::3e08:cdff:fe8d:badc, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21181    [1], 10.0.0.53/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21182    [1], 10.0.0.53/32, algorithm MIN-TE
                via TI-LFA tunnel index 3, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 21308
 IP    21248    [1], 10.0.0.120/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21249    [1], 10.0.0.120/32, algorithm MIN-TE
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21284    [1], 10.0.0.156/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21285    [1], 10.0.0.156/32, algorithm MIN-TE
                via TI-LFA tunnel index 4, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    21286    [1], 10.0.0.156/32, algorithm ADMIN
                via M, 20.30.32.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    21303    [1], 10.0.0.175/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 9, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label 21303
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21304    [1], 10.0.0.175/32, algorithm MIN-TE
                via TI-LFA tunnel index 2, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 21308 21304
 IP    21305    [1], 10.0.0.175/32, algorithm ADMIN
                via M, 20.30.32.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    21307    [1], 10.0.0.179/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21308    [1], 10.0.0.179/32, algorithm MIN-TE
                via TI-LFA tunnel index 4, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    21309    [1], 10.0.0.179/32, algorithm ADMIN
                via M, 20.30.32.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    21345    [1], 10.0.0.217/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21346    [1], 10.0.0.217/32, algorithm MIN-TE
                via TI-LFA tunnel index 4, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    21347    [1], 10.0.0.217/32, algorithm ADMIN
                via M, 20.30.32.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    21349    [1], 10.0.0.221/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21350    [1], 10.0.0.221/32, algorithm MIN-TE
                via TI-LFA tunnel index 4, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    21581    [1], 2002::53/128, algorithm MIN-LATENCY
                via TI-LFA tunnel index 15, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::3e08:cdff:fe8d:badc, Ethernet5, label imp-null(3)
                    backup via fe80::c6ca:2bff:fe45:a215, Ethernet1, label 21684
 IP    21582    [1], 2002::53/128, algorithm MIN-TE
                via TI-LFA tunnel index 8, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::3e08:cdff:fe8d:badc, Ethernet5, label imp-null(3)
                    backup via fe80::c6ca:2bff:fe45:a215, Ethernet1, label 21685
 IP    21684    [1], 2002::156/128, algorithm MIN-LATENCY
                via TI-LFA tunnel index 13, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::c6ca:2bff:fe45:a215, Ethernet1, label imp-null(3)
                    backup via fe80::3e08:cdff:fe8d:badc, Ethernet5, label imp-null(3)
 IP    21685    [1], 2002::156/128, algorithm MIN-TE
                via TI-LFA tunnel index 7, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::3e08:cdff:fe8d:badc, Ethernet5, label imp-null(3)
                    backup via fe80::c6ca:2bff:fe45:a215, Ethernet1, label imp-null(3)
 IP    21686    [1], 2002::156/128, algorithm ADMIN
                via M, fe80::c6ca:2bff:fe45:a215, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    21703    [1], 2002::175/128, algorithm MIN-LATENCY
                via TI-LFA tunnel index 19, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::3e08:cdff:fe8d:badc, Ethernet5, label imp-null(3)
                    backup via fe80::c6ca:2bff:fe45:a215, Ethernet1, label 21684 21703
 IP    21704    [1], 2002::175/128, algorithm MIN-TE
                via TI-LFA tunnel index 23, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::3e08:cdff:fe8d:badc, Ethernet5, label imp-null(3)
                    backup via fe80::c6ca:2bff:fe45:a215, Ethernet1, label 21685 21704
 IP    21705    [1], 2002::175/128, algorithm ADMIN
                via M, fe80::c6ca:2bff:fe45:a215, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IA    362168   [1]
                via M, 20.30.32.30, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
 IA    362169   [1]
                via M, fe80::c6ca:2bff:fe45:a215, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
 IA    362170   [1]
                via M, 20.32.175.175, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet5
 IA    362171   [1]
                via M, fe80::3e08:cdff:fe8d:badc, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet5
 B3    378528   [0]
                via I, ipv4, vrf RED
 B3    378529   [0]
                via I, ipv6, vrf RED
 B3    378530   [0]
                via I, ipv4, vrf FLEXALGO
```

## show bgp evpn

```text
BGP routing table information for VRF default
Router identifier 10.0.0.32, local AS number 64512
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
```

## show bgp vpn-ipv4

```text
BGP routing table information for VRF default
Router identifier 10.0.0.32, local AS number 64512
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 10.0.0.32:5001 IPv4 prefix 50.10.32.0/24
                                 -                     -       -       0       i
 * >Ec    RD: 53:5001 IPv4 prefix 50.10.53.0/24
                                 10.0.0.53             -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.30 
 *  ec    RD: 53:5001 IPv4 prefix 50.10.53.0/24
                                 10.0.0.53             -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.175 
 * >Ec    RD: 66:5001 IPv4 prefix 50.10.66.0/24
                                 10.0.0.66             -       100     0       ? Or-ID: 10.0.0.66 C-LST: 10.0.0.30 
 *  ec    RD: 66:5001 IPv4 prefix 50.10.66.0/24
                                 10.0.0.66             -       100     0       ? Or-ID: 10.0.0.66 C-LST: 10.0.0.175 
 * >Ec    RD: 72:5001 IPv4 prefix 50.10.72.0/24
                                 10.0.0.72             -       100     0       ? Or-ID: 10.0.0.72 C-LST: 10.0.0.30 
 *  ec    RD: 72:5001 IPv4 prefix 50.10.72.0/24
                                 10.0.0.72             -       100     0       ? Or-ID: 10.0.0.72 C-LST: 10.0.0.175 
 * >Ec    RD: 84:5001 IPv4 prefix 50.10.84.0/24
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.30 
 *  ec    RD: 84:5001 IPv4 prefix 50.10.84.0/24
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.175 
 * >Ec    RD: 120:5001 IPv4 prefix 50.10.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.30 
 *  ec    RD: 120:5001 IPv4 prefix 50.10.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.175 
          RD: 124:5001 IPv4 prefix 50.10.124.0/24
                                 10.0.0.124            0       100     0       ? Or-ID: 10.0.0.124 C-LST: 10.0.0.175 
          RD: 128:5001 IPv4 prefix 50.10.128.0/24
                                 10.0.0.128            0       100     0       ? Or-ID: 10.0.0.128 C-LST: 10.0.0.175 
 * >Ec    RD: 131:5001 IPv4 prefix 50.10.131.0/24
                                 10.0.0.131            -       100     0       i Or-ID: 10.0.0.131 C-LST: 10.0.0.30 
 *  ec    RD: 131:5001 IPv4 prefix 50.10.131.0/24
                                 10.0.0.131            -       100     0       i Or-ID: 10.0.0.131 C-LST: 10.0.0.175 
 * >Ec    RD: 156:5001 IPv4 prefix 50.10.156.0/24
                                 10.0.0.156            -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.30 
 *  ec    RD: 156:5001 IPv4 prefix 50.10.156.0/24
                                 10.0.0.156            -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.175 
 * >Ec    RD: 179:5001 IPv4 prefix 50.10.179.0/24
                                 10.0.0.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.30 
 *  ec    RD: 179:5001 IPv4 prefix 50.10.179.0/24
                                 10.0.0.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.175 
 * >Ec    RD: 214:5001 IPv4 prefix 50.10.214.0/24
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.30 
 *  ec    RD: 214:5001 IPv4 prefix 50.10.214.0/24
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.175 
 * >Ec    RD: 217:5001 IPv4 prefix 50.10.217.0/24
                                 10.0.0.217            -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.30 
 *  ec    RD: 217:5001 IPv4 prefix 50.10.217.0/24
                                 10.0.0.217            -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.175 
 * >Ec    RD: 221:5001 IPv4 prefix 50.10.221.0/24
                                 10.0.0.221            -       100     0       i Or-ID: 10.0.0.221 C-LST: 10.0.0.30 
 *  ec    RD: 221:5001 IPv4 prefix 50.10.221.0/24
                                 10.0.0.221            -       100     0       i Or-ID: 10.0.0.221 C-LST: 10.0.0.175 
 * >      RD: 10.0.0.30:5128 IPv4 prefix 50.128.32.0/24
                                 -                     -       -       0       i
 * >Ec    RD: 53:5128 IPv4 prefix 50.128.53.0/24
                                 10.0.0.53             -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.30 
 *  ec    RD: 53:5128 IPv4 prefix 50.128.53.0/24
                                 10.0.0.53             -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.175 
 * >Ec    RD: 120:5128 IPv4 prefix 50.128.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.30 
 *  ec    RD: 120:5128 IPv4 prefix 50.128.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.175 
          RD: 124:5128 IPv4 prefix 50.128.124.0/24
                                 10.0.0.124            0       100     0       ? Or-ID: 10.0.0.124 C-LST: 10.0.0.175 
          RD: 128:5128 IPv4 prefix 50.128.128.0/24
                                 10.0.0.128            0       100     0       ? Or-ID: 10.0.0.128 C-LST: 10.0.0.175 
 * >Ec    RD: 5128:5128 IPv4 prefix 50.128.156.0/24
                                 10.0.0.156            -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.30 
 *  ec    RD: 5128:5128 IPv4 prefix 50.128.156.0/24
                                 10.0.0.156            -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.175 
 * >Ec    RD: 5128:5128 IPv4 prefix 50.128.179.0/24
                                 10.0.0.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.30 
 *  ec    RD: 5128:5128 IPv4 prefix 50.128.179.0/24
                                 10.0.0.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.175 
 * >Ec    RD: 217:5128 IPv4 prefix 50.128.217.0/24
                                 10.0.0.217            -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.30 
 *  ec    RD: 217:5128 IPv4 prefix 50.128.217.0/24
                                 10.0.0.217            -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.175 
 * >      RD: 10.0.0.30:5128 IPv4 prefix 50.129.32.0/24
                                 -                     -       -       0       i
 * >Ec    RD: 53:5128 IPv4 prefix 50.129.53.0/24
                                 10.0.0.53             -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.30 
 *  ec    RD: 53:5128 IPv4 prefix 50.129.53.0/24
                                 10.0.0.53             -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.175 
 * >Ec    RD: 66:5001 IPv4 prefix 50.129.66.0/24
                                 10.0.0.66             -       100     0       ? Or-ID: 10.0.0.66 C-LST: 10.0.0.30 
 *  ec    RD: 66:5001 IPv4 prefix 50.129.66.0/24
                                 10.0.0.66             -       100     0       ? Or-ID: 10.0.0.66 C-LST: 10.0.0.175 
 * >Ec    RD: 72:5001 IPv4 prefix 50.129.72.0/24
                                 10.0.0.72             -       100     0       ? Or-ID: 10.0.0.72 C-LST: 10.0.0.30 
 *  ec    RD: 72:5001 IPv4 prefix 50.129.72.0/24
                                 10.0.0.72             -       100     0       ? Or-ID: 10.0.0.72 C-LST: 10.0.0.175 
 * >Ec    RD: 120:5129 IPv4 prefix 50.129.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.30 
 *  ec    RD: 120:5129 IPv4 prefix 50.129.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.175 
 * >Ec    RD: 5128:5128 IPv4 prefix 50.129.156.0/24
                                 10.0.0.156            -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.30 
 *  ec    RD: 5128:5128 IPv4 prefix 50.129.156.0/24
                                 10.0.0.156            -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.175 
 * >Ec    RD: 5128:5128 IPv4 prefix 50.129.179.0/24
                                 10.0.0.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.30 
 *  ec    RD: 5128:5128 IPv4 prefix 50.129.179.0/24
                                 10.0.0.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.175 
 * >Ec    RD: 217:5128 IPv4 prefix 50.129.217.0/24
                                 10.0.0.217            -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.30 
 *  ec    RD: 217:5128 IPv4 prefix 50.129.217.0/24
                                 10.0.0.217            -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.175 
 * >Ec    RD: 221:5128 IPv4 prefix 50.129.221.0/24
                                 10.0.0.221            -       100     0       i Or-ID: 10.0.0.221 C-LST: 10.0.0.30 
 *  ec    RD: 221:5128 IPv4 prefix 50.129.221.0/24
                                 10.0.0.221            -       100     0       i Or-ID: 10.0.0.221 C-LST: 10.0.0.175 
 * >      RD: 10.0.0.30:5128 IPv4 prefix 50.130.32.0/24
                                 -                     -       -       0       i
 * >Ec    RD: 53:5128 IPv4 prefix 50.130.53.0/24
                                 10.0.0.53             -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.30 
 *  ec    RD: 53:5128 IPv4 prefix 50.130.53.0/24
                                 10.0.0.53             -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.175 
 * >Ec    RD: 120:5130 IPv4 prefix 50.130.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.30 
 *  ec    RD: 120:5130 IPv4 prefix 50.130.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.175 
 * >Ec    RD: 5128:5128 IPv4 prefix 50.130.156.0/24
                                 10.0.0.156            -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.30 
 *  ec    RD: 5128:5128 IPv4 prefix 50.130.156.0/24
                                 10.0.0.156            -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.175 
 * >Ec    RD: 5128:5128 IPv4 prefix 50.130.179.0/24
                                 10.0.0.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.30 
 *  ec    RD: 5128:5128 IPv4 prefix 50.130.179.0/24
                                 10.0.0.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.175 
 * >Ec    RD: 217:5128 IPv4 prefix 50.130.217.0/24
                                 10.0.0.217            -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.30 
 *  ec    RD: 217:5128 IPv4 prefix 50.130.217.0/24
                                 10.0.0.217            -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.175 
```

## show bgp vpn-ipv6

```text
BGP routing table information for VRF default
Router identifier 10.0.0.32, local AS number 64512
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 10.0.0.32:5001 IPv6 prefix 2600:50:10:32::/64
                                 -                     -       -       0       i
 * >Ec    RD: 84:5001 IPv6 prefix 2600:50:10:84::/64
                                 ::ffff:10.0.0.84      0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.30 
 *  ec    RD: 84:5001 IPv6 prefix 2600:50:10:84::/64
                                 ::ffff:10.0.0.84      0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.175 
 * >Ec    RD: 131:5001 IPv6 prefix 2600:50:10:131::/64
                                 ::ffff:10.0.0.131     -       100     0       i Or-ID: 10.0.0.131 C-LST: 10.0.0.30 
 *  ec    RD: 131:5001 IPv6 prefix 2600:50:10:131::/64
                                 ::ffff:10.0.0.131     -       100     0       i Or-ID: 10.0.0.131 C-LST: 10.0.0.175 
 * >Ec    RD: 156:5001 IPv6 prefix 2600:50:10:156::/64
                                 ::ffff:10.0.0.156     -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.30 
 *  ec    RD: 156:5001 IPv6 prefix 2600:50:10:156::/64
                                 ::ffff:10.0.0.156     -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.175 
 * >Ec    RD: 179:5001 IPv6 prefix 2600:50:10:179::/64
                                 ::ffff:10.0.0.179     -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.30 
 *  ec    RD: 179:5001 IPv6 prefix 2600:50:10:179::/64
                                 ::ffff:10.0.0.179     -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.175 
 * >Ec    RD: 214:5001 IPv6 prefix 2600:50:10:214::/64
                                 ::ffff:10.0.0.214     -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.30 
 *  ec    RD: 214:5001 IPv6 prefix 2600:50:10:214::/64
                                 ::ffff:10.0.0.214     -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.175 
 * >Ec    RD: 217:5001 IPv6 prefix 2600:50:10:217::/64
                                 ::ffff:10.0.0.217     -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.30 
 *  ec    RD: 217:5001 IPv6 prefix 2600:50:10:217::/64
                                 ::ffff:10.0.0.217     -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.175 
```

## show bgp ipv4 labeled-unicast

```text
BGP routing table information for VRF default
Router identifier 10.0.0.32, local AS number 64512
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
```

## show bgp neighbors

```text
BGP neighbor is 10.0.0.30, remote AS 64512, internal link
 Description: Arista-Spine30
  BGP version 4, remote router ID 10.0.0.30, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:57, last write 00:00:34
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:03
  Keepalive timer is active, time left: 00:00:16
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 3d15h
  Number of transitions to established: 5
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Hold Timer Expired Error/None, Last time 3d17h, First time 5d23h, Repeats 3
  Last sent socket-error:Connect (Connection refused), Last time 3d15h, First time 3d15h, Repeats 7
  Types of communities advertised: standard extended large
  Enhanced route refresh stale path removal disabled
  Outbound enhanced route refresh enabled
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
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: yes
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 3d15h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 22
    VPN-IPv6 End-of-RIB received: Yes
      Received 3d15h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 4
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
    Opens:                           5         5
    Notifications:                   4         0
    Updates:                        70      1352
    Keepalives:                  11207     11026
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:              11286     12383
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         4        29             29                  29
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         1         6              6                   6
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
  Outbound route map for VPN-IPv6 is SET_COLOR_101
Local AS is 64512, local router ID 10.0.0.32
TTL is 255
Local TCP address is 10.0.0.32, local port is 179
Remote TCP address is 10.0.0.30, remote port is 39975
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.32
  VPN-IPv6: ::ffff:10.0.0.32
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
    TCP Throughput: 461.51 Mbps
    Recv Round-trip Time (rcv_rtt): 31.0ms
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.175, remote AS 64512, internal link
 Description: Juniper_175
  BGP version 4, remote router ID 10.0.0.175, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:16, last write 00:00:22
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:14
  Keepalive timer is active, time left: 00:00:03
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 3d15h
  Number of transitions to established: 138
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Open Message Error/unsupported capability, Last time 3d15h, First time 3d15h, Repeats 3
    Sent data: 0x010400010080010400020080
  Last rcvd notification:Update Message Error/error with optional attribute, Last time 3d18h, First time 3d18h, Repeats 123
  Last sent socket-error:Connect (Network is unreachable), Last time 3d15h, First time 4d22h, Repeats 64
  Last rcvd socket-error:Connection reset by peer, Last time 4d22h
  Types of communities advertised: standard extended large
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
      Received 3d15h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 12
    VPN-IPv6 End-of-RIB received: Yes
      Received 3d15h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 3
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
    Opens:                142       142
    Notifications:         15       125
    Updates:              968      1851
    Keepalives:         22612     20323
    Route Refresh:          0         0
    Total messages:     23737     22441
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         4        33             29                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         1         6              6                   0
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
  Outbound route map for VPN-IPv6 is SET_COLOR_101
Local AS is 64512, local router ID 10.0.0.32
TTL is 255
Local TCP address is 10.0.0.32, local port is 43733
Remote TCP address is 10.0.0.175, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.32
  VPN-IPv6: ::ffff:10.0.0.32
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1448
  Total Number of TCP retransmissions: 3
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
    Congestion Window (cwnd): 2
    Slow-start Threshold (ssthresh): 7
    TCP Throughput: 52.30 Mbps
    Recv Round-trip Time (rcv_rtt): 177600.0ms
    Advertised Recv Window (rcv_space): 64341

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
10.0.0.30/32    IS-IS SR IPv4   5           10                  115            
10.0.0.53/32    IS-IS SR IPv4   6           10                  115            
10.0.0.66/32    IS-IS SR IPv4   17          10                  115            
10.0.0.72/32    IS-IS SR IPv4   9           10                  115            
10.0.0.84/32    IS-IS SR IPv4   2           10                  115            
10.0.0.120/32   IS-IS SR IPv4   8           10                  115            
10.0.0.131/32   IS-IS SR IPv4   12          10                  115            
10.0.0.156/32   IS-IS SR IPv4   18          10                  115            
10.0.0.175/32   IS-IS SR IPv4   1           10                  115            
10.0.0.179/32   IS-IS SR IPv4   7           10                  115            
10.0.0.214/32   IS-IS SR IPv4   10          10                  115            
10.0.0.217/32   IS-IS SR IPv4   16          10                  115            
10.0.0.221/32   IS-IS SR IPv4   13          10                  115            
2002::120/128   IS-IS SR IPv6   27          10                  115            
2002::175/128   IS-IS SR IPv6   22          10                  115            
2002::30/128    IS-IS SR IPv6   20          10                  115            
2002::53/128    IS-IS SR IPv6   21          10                  115            
2002::156/128   IS-IS SR IPv6   25          10                  115            

   IGP Metric    Metric Type
---------------- -----------
   10            metric     
   20            metric     
   21            metric     
   21            metric     
   21            metric     
   11            metric     
   11            metric     
   11            metric     
   10            metric     
   11            metric     
   11            metric     
   11            metric     
   11            metric     
   20            metric     
   10            metric     
   20            metric     
   20            metric     
   20            metric     

```

## show tunnel rib colored brief

```text
Tunnel RIB: system-colored-tunnel-rib
 Endpoint        Color   Tunnel Type       Index(es)    Tunnel Preference    IGP Preference    IGP Metric   Metric Type
--------------- ------- ----------------- ------------ -------------------- ----------------- ------------- -----------
 10.0.0.30/32    128     IS-IS FlexAlgo    7            65                   115               10000        metric     
 10.0.0.30/32    129     IS-IS FlexAlgo    11           65                   115               30           metric     
 10.0.0.30/32    130     IS-IS FlexAlgo    2            65                   115               10           metric     
 10.0.0.53/32    128     IS-IS FlexAlgo    6            65                   115               120010       metric     
 10.0.0.53/32    129     IS-IS FlexAlgo    12           65                   115               20           metric     
 10.0.0.120/32   128     IS-IS FlexAlgo    44           65                   115               120010       metric     
 10.0.0.120/32   129     IS-IS FlexAlgo    45           65                   115               20           metric     
 10.0.0.156/32   128     IS-IS FlexAlgo    27           65                   115               20000        metric     
 10.0.0.156/32   129     IS-IS FlexAlgo    26           65                   115               20           metric     
 10.0.0.156/32   130     IS-IS FlexAlgo    28           65                   115               11           metric     
 10.0.0.175/32   128     IS-IS FlexAlgo    30           65                   115               20010        metric     
 10.0.0.175/32   129     IS-IS FlexAlgo    29           65                   115               10           metric     
 10.0.0.175/32   130     IS-IS FlexAlgo    31           65                   115               21           metric     
 10.0.0.179/32   128     IS-IS FlexAlgo    40           65                   115               20000        metric     
 10.0.0.179/32   129     IS-IS FlexAlgo    38           65                   115               20           metric     
 10.0.0.179/32   130     IS-IS FlexAlgo    39           65                   115               11           metric     
 10.0.0.217/32   128     IS-IS FlexAlgo    10           65                   115               20000        metric     
 10.0.0.217/32   129     IS-IS FlexAlgo    14           65                   115               20           metric     
 10.0.0.217/32   130     IS-IS FlexAlgo    3            65                   115               11           metric     
 10.0.0.221/32   128     IS-IS FlexAlgo    5            65                   115               20000        metric     
 10.0.0.221/32   129     IS-IS FlexAlgo    15           65                   115               20           metric     
 2002::30/128    128     IS-IS FlexAlgo    47           65                   115               10000        metric     
 2002::30/128    129     IS-IS FlexAlgo    48           65                   115               100          metric     
 2002::30/128    130     IS-IS FlexAlgo    64           65                   115               10           metric     
 2002::156/128   128     IS-IS FlexAlgo    61           65                   115               20000        metric     
 2002::156/128   129     IS-IS FlexAlgo    62           65                   115               20           metric     
 2002::156/128   130     IS-IS FlexAlgo    63           65                   115               20           metric     
 2002::53/128    128     IS-IS FlexAlgo    50           65                   115               200000       metric     
 2002::53/128    129     IS-IS FlexAlgo    49           65                   115               20           metric     
 2002::175/128   128     IS-IS FlexAlgo    54           65                   115               100000       metric     
 2002::175/128   129     IS-IS FlexAlgo    51           65                   115               10           metric     
 2002::175/128   130     IS-IS FlexAlgo    53           65                   115               30           metric     

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
>C    10.0.0.32/32 [0 pref/0 metric] updated 6d19h ago
         via Loopback0, directly connected
>C    20.30.32.0/24 [0 pref/0 metric] updated 2d15h ago
         via Ethernet1, directly connected
>C    20.32.175.0/24 [0 pref/0 metric] updated 2d17h ago
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
>P    0.0.0.0/8 [1 pref/0 metric] updated 7d01h ago
         via Null0, directly connected [NF]
>P    127.0.0.0/8 [1 pref/0 metric] updated 7d01h ago
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
>I    10.0.0.30/32 [115 pref/10 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.53/32 [115 pref/20 metric] updated 00:05:59 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.66/32 [115 pref/21 metric] updated 2d14h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.72/32 [115 pref/21 metric] updated 2d14h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.84/32 [115 pref/21 metric] updated 2d14h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.120/32 [115 pref/11 metric] updated 2d14h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.124/32 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.128/32 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.131/32 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.156/32 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.175/32 [115 pref/10 metric] updated 2d17h ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.179/32 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.214/32 [115 pref/11 metric] updated 1d18h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.216/32 [115 pref/21 metric] updated 1d18h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.217/32 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.221/32 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    10.0.1.179/32 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    20.30.66.0/24 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    20.30.72.0/24 [115 pref/11 metric] updated 2d14h ago
         via 20.30.32.30, Ethernet1
>I    20.30.84.0/24 [115 pref/11 metric] updated 2d14h ago
         via 20.30.32.30, Ethernet1
>I    20.30.120.0/24 [115 pref/11 metric] updated 2d14h ago
         via 20.30.32.30, Ethernet1
>I    20.30.124.0/24 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    20.30.128.0/24 [115 pref/11 metric] updated 22:08:51 ago
         via 20.30.32.30, Ethernet1
>I    20.30.131.0/24 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    20.30.156.0/24 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    20.30.179.0/24 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    20.30.184.0/24 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    20.30.214.0/24 [115 pref/11 metric] updated 1d18h ago
         via 20.30.32.30, Ethernet1
>I    20.30.217.0/24 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    20.30.221.0/24 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    20.53.175.0/24 [115 pref/20 metric] updated 2d17h ago
         via 20.32.175.175, Ethernet5
>I    20.66.175.0/24 [115 pref/20 metric] updated 2d17h ago
         via 20.32.175.175, Ethernet5
>I    20.72.175.0/24 [115 pref/20 metric] updated 2d17h ago
         via 20.32.175.175, Ethernet5
>I    20.84.175.0/24 [115 pref/20 metric] updated 2d17h ago
         via 20.32.175.175, Ethernet5
>I    20.120.175.0/24 [115 pref/20 metric] updated 2d14h ago
         via 20.32.175.175, Ethernet5
>I    20.120.214.0/24 [115 pref/21 metric] updated 2d14h ago
         via 20.30.32.30, Ethernet1
>I    20.120.217.0/24 [115 pref/11 metric] updated 2d14h ago
         via 20.30.32.30, Ethernet1
>I    20.124.175.0/24 [115 pref/20 metric] updated 2d15h ago
         via 20.32.175.175, Ethernet5
>I    20.128.175.0/24 [115 pref/20 metric] updated 2d17h ago
         via 20.32.175.175, Ethernet5
>I    20.131.175.0/24 [115 pref/20 metric] updated 2d17h ago
         via 20.32.175.175, Ethernet5
>I    20.156.175.0/24 [115 pref/20 metric] updated 2d17h ago
         via 20.32.175.175, Ethernet5
>I    20.175.179.0/24 [115 pref/20 metric] updated 2d17h ago
         via 20.32.175.175, Ethernet5
>I    20.175.184.0/24 [115 pref/20 metric] updated 2d17h ago
         via 20.32.175.175, Ethernet5
>I    20.175.214.0/24 [115 pref/20 metric] updated 2d17h ago
         via 20.32.175.175, Ethernet5
>I    20.175.217.0/24 [115 pref/20 metric] updated 2d17h ago
         via 20.32.175.175, Ethernet5
>I    20.175.221.0/24 [115 pref/20 metric] updated 2d15h ago
         via 20.32.175.175, Ethernet5
>I    20.214.216.0/24 [115 pref/21 metric] updated 1d18h ago
         via 20.30.32.30, Ethernet1
>I    21.30.124.0/24 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    21.30.128.0/24 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    21.30.156.0/24 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    21.30.217.0/24 [115 pref/11 metric] updated 2d15h ago
         via 20.30.32.30, Ethernet1
>I    192.168.20.0/23 [115 pref/11 metric] updated 2d14h ago
         via 20.30.32.30, Ethernet1
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
         via Ethernet1, directly connected
>C    2001:0:32:175::/64 [0 pref/0 metric] updated 2d17h ago
         via Ethernet5, directly connected
>C    2002::32/128 [0 pref/0 metric] updated 3d18h ago
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
>P    ::/96 [1 pref/0 metric] updated 5d22h ago
         via Null0, directly connected [NF]
>P    ::ffff:127.0.0.0/104 [1 pref/0 metric] updated 5d22h ago
         via :: [1 pref/1 metric] type ipv6
            via , directly connected
>P    fe80::/10 [1 pref/0 metric] updated 5d22h ago
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
>I    2000::214/128 [115 pref/20 metric] updated 2d17h ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:30:66::/64 [115 pref/20 metric] updated 2d15h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:72::/64 [115 pref/20 metric] updated 2d14h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:84::/64 [115 pref/20 metric] updated 2d14h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:120::/64 [115 pref/20 metric] updated 2d14h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:124::/64 [115 pref/20 metric] updated 2d15h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:128::/64 [115 pref/20 metric] updated 22:08:51 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:131::/64 [115 pref/20 metric] updated 2d15h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:156::/64 [115 pref/20 metric] updated 2d15h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:179::/64 [115 pref/20 metric] updated 2d15h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:184::/64 [115 pref/20 metric] updated 2d15h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:214::/64 [115 pref/20 metric] updated 1d18h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:217::/64 [115 pref/20 metric] updated 2d15h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:221::/64 [115 pref/20 metric] updated 2d15h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:53:175::/64 [115 pref/20 metric] updated 2d17h ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:66:175::/64 [115 pref/20 metric] updated 2d17h ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:72:175::/64 [115 pref/20 metric] updated 2d17h ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:84:175::/64 [115 pref/20 metric] updated 2d17h ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:120:175::/64 [115 pref/20 metric] updated 2d14h ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:120:214::/64 [115 pref/30 metric] updated 2d14h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:120:217::/64 [115 pref/20 metric] updated 2d14h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:128:175::/64 [115 pref/20 metric] updated 2d17h ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:131:175::/64 [115 pref/20 metric] updated 2d17h ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:156:175::/64 [115 pref/20 metric] updated 2d17h ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:175::/64 [115 pref/20 metric] updated 2d17h ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:175:184::/64 [115 pref/20 metric] updated 2d17h ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:175:214::/64 [115 pref/20 metric] updated 2d17h ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:175:217::/64 [115 pref/20 metric] updated 2d17h ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:175:221::/64 [115 pref/20 metric] updated 2d15h ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:214:216::/64 [115 pref/30 metric] updated 2d17h ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2002::30/128 [115 pref/20 metric] updated 2d15h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2002::53/128 [115 pref/20 metric] updated 00:05:59 ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2002::120/128 [115 pref/20 metric] updated 2d14h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2002::156/128 [115 pref/20 metric] updated 2d15h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2002::175/128 [115 pref/10 metric] updated 2d17h ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2002::216/128 [115 pref/30 metric] updated 2d17h ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2002::217/128 [115 pref/20 metric] updated 2d15h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
```

## show platform sand l3 summary

```text
Number of vrfs: 4

Ipv4:
  Routes:       127  backlog:  0  unprogrammed:  0
  Adjacencies:  137  backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       58   backlog:  0  unprogrammed:  0
  Adjacencies:  137  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       54  backlog:  0  unprogrammed:  0
  Adjacencies:  4   backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4189  ecmp fecs:  1  fec entries:  4191
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  4  ecmp fecs:  0  fec entries:  4
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   127  unprogrammed:   0   
  Routes6:  58   unprogrammed6:  0   
  Backlog:  0  

Jericho2 Lpm:
  TCAM entries used:   4   Percent free:  99  ADS2 entries used:   9  Percent free:  99
  Pivot buckets used:  6   Rows used:     2   Entries Per Bucket:  1  Percent free:  99
  Route buckets used:  34  Rows used:     4   Entries Per Bucket:  5  Percent free:  99

Lem:
  IPv4  Host in Lem:            disabled
  IPv4  Prefix-lengths in Lem:  None    
  IPv6  Host in Lem:            disabled
  IPv6  Prefix-lengths in Lem:  None    
  Number of downloads:        0
  Number of overflow events:  0

Egress Arp rewrite entries in use (in each fap):
  FixedSystem: 5
Egress Arp remote rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Ip tunnel rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Mpls (for outer 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Mpls (for inner 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 64
Egress Sflow rewrite entries in use (in each fap):
  FixedSystem: 0

Egress rewrite chains in backlog: resource-full 0, no-interface 0

Glem entries used per fap :
  FixedSystem: 4207

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  2  allocs:  1280  frees:  1185  shuffles:  0  cmds:  0
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
    Non-ecmp fecs:            66  ecmp fecs:            0  
    Non-ecmp (Percent free):  99  ecmp (Percent free):  100
  Level3  Fecs:
    Non-ecmp fecs:            126  ecmp fecs:            1 
    Non-ecmp (Percent free):  99   ecmp (Percent free):  99

Lpm Detail:
  Requests:  3192  cleanses:  680  batches:  680  avg batch size:  4

Jericho Arp:
  ArpTable writes:      48019  queued      0   
  IngressTable writes:  93550  queued      0   
  Coprocessors:         1      in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  106  
  Number of uncountable MPLS tunnels:      24   
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
|0  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |528526|   -   
|0  |10.0.0.30/32      |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |10.0.0.32/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |10.0.0.53/32      |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528600|   -   
|0  |10.0.0.66/32      |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |10.0.0.72/32      |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |10.0.0.84/32      |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |10.0.0.120/32     |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |10.0.0.124/32     |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |10.0.0.128/32     |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |10.0.0.131/32     |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |10.0.0.156/32     |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |10.0.0.175/32     |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528600|   -   
|0  |10.0.0.179/32     |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |10.0.0.214/32     |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |10.0.0.216/32     |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |10.0.0.217/32     |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |10.0.0.221/32     |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |10.0.1.179/32     |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |20.30.32.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.30.32.30/32    |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528532|   -   
|0  |20.30.32.32/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |20.30.32.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.30.32.0/24     |TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |  -  |525301|   -   
|0  |20.30.66.0/24     |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |20.30.72.0/24     |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |20.30.84.0/24     |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |20.30.120.0/24    |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |20.30.124.0/24    |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |20.30.128.0/24    |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |20.30.131.0/24    |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |20.30.156.0/24    |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |20.30.179.0/24    |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |20.30.184.0/24    |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |20.30.214.0/24    |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |20.30.217.0/24    |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |20.30.221.0/24    |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |20.32.175.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.32.175.32/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |20.32.175.175/32  |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528596|   -   
|0  |20.32.175.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.32.175.0/24    |TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |  -  |525305|   -   
|0  |20.53.175.0/24    |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528600|   -   
|0  |20.66.175.0/24    |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528600|   -   
|0  |20.72.175.0/24    |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528600|   -   
|0  |20.84.175.0/24    |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528600|   -   
|0  |20.120.175.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528600|   -   
|0  |20.120.214.0/24   |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |20.120.217.0/24   |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |20.124.175.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528600|   -   
|0  |20.128.175.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528600|   -   
|0  |20.131.175.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528600|   -   
|0  |20.156.175.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528600|   -   
|0  |20.175.179.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528600|   -   
|0  |20.175.184.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528600|   -   
|0  |20.175.214.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528600|   -   
|0  |20.175.217.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528600|   -   
|0  |20.175.221.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528600|   -   
|0  |20.214.216.0/24   |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |21.30.124.0/24    |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |21.30.128.0/24    |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |21.30.156.0/24    |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |21.30.217.0/24    |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|0  |192.168.20.0/23   |ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |  -  |528534|   -   
|0  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |524293|   -   
|1  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |528542|   -   
|1  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|1  |192.168.20.0/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|1  |192.168.20.32/32  |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|1  |192.168.21.255/32 |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|1  |192.168.20.0/23   |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|1  |0.0.0.0/0         |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|2  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |528538|   -   
|2  |50.10.32.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|2  |50.10.32.1/32     |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|2  |50.10.32.2/32     |ROUTE| Et40               |1008 |107521  | 00:28:01:00:00:01 |  -  |528584|   -   
|2  |50.10.32.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|2  |50.10.32.0/24     |TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |  -  |525303|   -   
|2  |50.10.53.0/24     |ROUTE| FEC 528572         |0    |2097135 | 00:00:00:00:00:00 |  -  |288386|M 970000
|2  |50.10.66.0/24     |ROUTE| FEC 528570         |0    |2097147 | 00:00:00:00:00:00 |  -  |288378|M 62000
|2  |50.10.72.0/24     |ROUTE| FEC 528488         |0    |2097145 | 00:00:00:00:00:00 |  -  |288380|M 62000
|2  |50.10.84.0/24     |ROUTE| FEC 528524         |0    |2097140 | 00:00:00:00:00:00 |  -  |288422|M 720898
|2  |50.10.120.0/24    |ROUTE| FEC 528514         |0    |2097150 | 00:00:00:00:00:00 |  -  |288394|M 1279
|2  |50.10.131.0/24    |ROUTE| FEC 528506         |0    |2097094 | 00:00:00:00:00:00 |  -  |288428|M 18
|2  |50.10.156.0/24    |ROUTE| FEC 528500         |0    |2097099 | 00:00:00:00:00:00 |  -  |288426|M 16
|2  |50.10.179.0/24    |ROUTE| FEC 528498         |0    |2097103 | 00:00:00:00:00:00 |  -  |288424|M 16
|2  |50.10.214.0/24    |ROUTE| FEC 528484         |0    |2097139 | 00:00:00:00:00:00 |  -  |288420|M 500000
|2  |50.10.217.0/24    |ROUTE| FEC 528502         |0    |2097098 | 00:00:00:00:00:00 |  -  |288430|M 524287
|2  |50.10.221.0/24    |ROUTE| FEC 528554         |0    |2097148 | 00:00:00:00:00:00 |  -  |288372|M 524292
|2  |50.129.66.0/24    |ROUTE| FEC 528570         |0    |2097147 | 00:00:00:00:00:00 |  -  |288378|M 62000
|2  |50.129.72.0/24    |ROUTE| FEC 528488         |0    |2097145 | 00:00:00:00:00:00 |  -  |288380|M 62000
|2  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|2  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |524293|   -   
|3  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |528544|   -   
|3  |50.128.32.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|3  |50.128.32.1/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|3  |50.128.32.2/32    |ROUTE| Et40               |1012 |107518  | 00:28:01:00:00:02 |  -  |528582|   -   
|3  |50.128.32.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|3  |50.128.32.0/24    |TRAP | CoppSystemL3DstMiss|1012 |1012    | ArpTrap           |  -  |525307|   -   
|3  |50.128.53.0/24    |ROUTE| FEC 528560         |0    |2097078 | 00:00:00:00:00:00 |  -  |288364|M 970002
|3  |50.128.120.0/24   |ROUTE| FEC 528562         |0    |2097149 | 00:00:00:00:00:00 |  -  |288396|M 1278
|3  |50.128.156.0/24   |ROUTE| FEC 528564         |0    |2097080 | 00:00:00:00:00:00 |  -  |288368|M 17
|3  |50.128.179.0/24   |ROUTE| FEC 528566         |0    |2097077 | 00:00:00:00:00:00 |  -  |288370|M 21
|3  |50.128.217.0/24   |ROUTE| FEC 528558         |0    |2097079 | 00:00:00:00:00:00 |  -  |288366|M 524284
|3  |50.129.32.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|3  |50.129.32.1/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|3  |50.129.32.2/32    |ROUTE| Et40               |1013 |107517  | 00:28:01:00:00:03 |  -  |528578|   -   
|3  |50.129.32.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|3  |50.129.32.0/24    |TRAP | CoppSystemL3DstMiss|1013 |1013    | ArpTrap           |  -  |525308|   -   
|3  |50.129.53.0/24    |ROUTE| FEC 528552         |0    |2097084 | 00:00:00:00:00:00 |  -  |288360|M 970002
|3  |50.129.120.0/24   |ROUTE| FEC 528546         |0    |2097151 | 00:00:00:00:00:00 |  -  |288384|M 21249 1277
|3  |50.129.156.0/24   |ROUTE| FEC 528550         |0    |2097085 | 00:00:00:00:00:00 |  -  |288382|M 17
|3  |50.129.179.0/24   |ROUTE| FEC 528548         |0    |2097086 | 00:00:00:00:00:00 |  -  |288362|M 21
|3  |50.129.217.0/24   |ROUTE| FEC 528556         |0    |2097082 | 00:00:00:00:00:00 |  -  |288374|M 524284
|3  |50.129.221.0/24   |ROUTE| FEC 528516         |0    |2097146 | 00:00:00:00:00:00 |  -  |288376|M 524293
|3  |50.130.32.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|3  |50.130.32.1/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|3  |50.130.32.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|3  |50.130.32.0/24    |TRAP | CoppSystemL3DstMiss|1014 |1014    | ArpTrap           |  -  |525309|   -   
|3  |50.130.53.0/24    |ROUTE| FEC 528572         |0    |2097134 | 00:00:00:00:00:00 |  -  |288432|M 970002
|3  |50.130.120.0/24   |ROUTE| FEC 528514         |0    |2097144 | 00:00:00:00:00:00 |  -  |288398|M 1276
|3  |50.130.156.0/24   |ROUTE| FEC 528614         |0    |2097074 | 00:00:00:00:00:00 |  -  |288408|M 21286 17
|3  |50.130.179.0/24   |ROUTE| FEC 528614         |0    |2097073 | 00:00:00:00:00:00 |  -  |288392|M 21309 21
|3  |50.130.217.0/24   |ROUTE| FEC 528614         |0    |2097076 | 00:00:00:00:00:00 |  -  |288406|M 21347 524284
|3  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|3  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |524293|   -   

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
|24576|528604|ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |   -   
|24576|528605|ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |   -   
|24576|528606|ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |   -   
|24576|528607|ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288360|ROUTE| FEC 528552         |   - |2097084 |                 - |Mpush 970002
|  -  |288362|ROUTE| FEC 528548         |   - |2097086 |                 - |Mpush 21
|  -  |288364|ROUTE| FEC 528560         |   - |2097078 |                 - |Mpush 970002
|  -  |288366|ROUTE| FEC 528558         |   - |2097079 |                 - |Mpush 524284
|  -  |288368|ROUTE| FEC 528564         |   - |2097080 |                 - |Mpush 17
|  -  |288370|ROUTE| FEC 528566         |   - |2097077 |                 - |Mpush 21
|  -  |288372|ROUTE| FEC 528554         |   - |2097148 |                 - |Mpush 524292
|  -  |288374|ROUTE| FEC 528556         |   - |2097082 |                 - |Mpush 524284
|  -  |288376|ROUTE| FEC 528516         |   - |2097146 |                 - |Mpush 524293
|  -  |288378|ROUTE| FEC 528570         |   - |2097147 |                 - |Mpush 62000
|  -  |288380|ROUTE| FEC 528488         |   - |2097145 |                 - |Mpush 62000
|  -  |288382|ROUTE| FEC 528550         |   - |2097085 |                 - |Mpush 17
|  -  |288384|ROUTE| FEC 528546         |   - |2097151 |                 - |Mpush 21249 1277
|  -  |288386|ROUTE| FEC 528572         |   - |2097135 |                 - |Mpush 970000
|  -  |288388|ROUTE| FEC 528524         |   - |2097141 |                 - |Mpush 720899
|  -  |288390|ROUTE| FEC 528498         |   - |2097103 |                 - |Mpush 16
|  -  |288392|ROUTE| FEC 528614         |   - |2097073 |                 - |Mpush 21309 21
|  -  |288394|ROUTE| FEC 528514         |   - |2097150 |                 - |Mpush 1279
|  -  |288396|ROUTE| FEC 528562         |   - |2097149 |                 - |Mpush 1278
|  -  |288398|ROUTE| FEC 528514         |   - |2097144 |                 - |Mpush 1276
|  -  |288400|ROUTE| FEC 528484         |   - |2097139 |                 - |Mpush 500000
|  -  |288402|ROUTE| FEC 528506         |   - |2097094 |                 - |Mpush 18
|  -  |288404|ROUTE| FEC 528502         |   - |2097098 |                 - |Mpush 524287
|  -  |288406|ROUTE| FEC 528614         |   - |2097076 |                 - |Mpush 21347 524284
|  -  |288408|ROUTE| FEC 528614         |   - |2097074 |                 - |Mpush 21286 17
|  -  |288410|ROUTE| FEC 528500         |   - |2097099 |                 - |Mpush 16
|  -  |288420|ROUTE| FEC 528484         |   - |2097139 |                 - |Mpush 500000
|  -  |288422|ROUTE| FEC 528524         |   - |2097140 |                 - |Mpush 720898
|  -  |288424|ROUTE| FEC 528498         |   - |2097103 |                 - |Mpush 16
|  -  |288426|ROUTE| FEC 528500         |   - |2097099 |                 - |Mpush 16
|  -  |288428|ROUTE| FEC 528506         |   - |2097094 |                 - |Mpush 18
|  -  |288430|ROUTE| FEC 528502         |   - |2097098 |                 - |Mpush 524287
|  -  |288432|ROUTE| FEC 528572         |   - |2097134 |                 - |Mpush 970002
|  -  |524290|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |524291|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |524293|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |524295|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |525301|TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |   -   
|  -  |525303|TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |   -   
|  -  |525304|TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |   -   
|  -  |525305|TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |   -   
|  -  |525307|TRAP | CoppSystemL3DstMiss|1012 |1012    | ArpTrap           |   -   
|  -  |525308|TRAP | CoppSystemL3DstMiss|1013 |1013    | ArpTrap           |   -   
|  -  |525309|TRAP | CoppSystemL3DstMiss|1014 |1014    | ArpTrap           |   -   
|  -  |528482|ROUTE| Et1                |1006 |107522  | c4:ca:2b:45:a2:15 |   -   
|  -  |528483|ROUTE| Et5                |1010 |107523  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528484|ROUTE| Et1                |1006 |107525  | c4:ca:2b:45:a2:15 |Mpush 20214
|  -  |528485|ROUTE| Et5                |1010 |107526  | 3c:08:cd:8d:ba:dc |Mpush 20214
|  -  |528486|ROUTE| Et5                |1010 |107579  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528487|ROUTE| Et1                |1006 |107580  | c4:ca:2b:45:a2:15 |Mpush 21684 21703
|  -  |528488|ROUTE| Et1                |1006 |107542  | c4:ca:2b:45:a2:15 |Mpush 20072
|  -  |528489|ROUTE| Et5                |1010 |107543  | 3c:08:cd:8d:ba:dc |Mpush 20072
|  -  |528490|ROUTE| Et5                |1010 |107530  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528491|ROUTE| Et1                |1006 |107531  | c4:ca:2b:45:a2:15 |   -   
|  -  |528492|ROUTE| Et5                |1010 |107532  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528493|ROUTE| Et1                |1006 |107533  | c4:ca:2b:45:a2:15 |Mpush 21308 21304
|  -  |528494|ROUTE| Et5                |1010 |107524  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528495|ROUTE| Et1                |1006 |107529  | c4:ca:2b:45:a2:15 |Mpush 21308
|  -  |528496|ROUTE| Et5                |1010 |107536  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528497|ROUTE| Et1                |1006 |107537  | c4:ca:2b:45:a2:15 |   -   
|  -  |528498|ROUTE| Et1                |1006 |107540  | c4:ca:2b:45:a2:15 |Mpush 20179
|  -  |528499|ROUTE| Et5                |1010 |107541  | 3c:08:cd:8d:ba:dc |Mpush 20179
|  -  |528500|ROUTE| Et1                |1006 |107562  | c4:ca:2b:45:a2:15 |Mpush 20156
|  -  |528501|ROUTE| Et5                |1010 |107563  | 3c:08:cd:8d:ba:dc |Mpush 20156
|  -  |528502|ROUTE| Et1                |1006 |107564  | c4:ca:2b:45:a2:15 |Mpush 20217
|  -  |528503|ROUTE| Et5                |1010 |107565  | 3c:08:cd:8d:ba:dc |Mpush 20217
|  -  |528504|ROUTE| Et1                |1006 |107527  | c4:ca:2b:45:a2:15 |   -   
|  -  |528505|ROUTE| Et5                |1010 |107528  | 3c:08:cd:8d:ba:dc |Mpush 20030
|  -  |528506|ROUTE| Et1                |1006 |107568  | c4:ca:2b:45:a2:15 |Mpush 20131
|  -  |528507|ROUTE| Et5                |1010 |107569  | 3c:08:cd:8d:ba:dc |Mpush 20131
|  -  |528508|ROUTE| Et1                |1006 |107577  | c4:ca:2b:45:a2:15 |   -   
|  -  |528509|ROUTE| Et5                |1010 |107578  | 3c:08:cd:8d:ba:dc |Mpush 21684 20558
|  -  |528510|ROUTE| Et5                |1010 |107581  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528511|ROUTE| Et1                |1006 |107582  | c4:ca:2b:45:a2:15 |Mpush 21684
|  -  |528512|ROUTE| Et5                |1010 |107575  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528513|ROUTE| Et1                |1006 |107576  | c4:ca:2b:45:a2:15 |Mpush 21685 21704
|  -  |528514|ROUTE| Et1                |1006 |107534  | c4:ca:2b:45:a2:15 |Mpush 20120
|  -  |528515|ROUTE| Et5                |1010 |107535  | 3c:08:cd:8d:ba:dc |Mpush 20120
|  -  |528516|ROUTE| Et5                |1010 |107550  | 3c:08:cd:8d:ba:dc |Mpush 21350
|  -  |528517|ROUTE| Et1                |1006 |107551  | c4:ca:2b:45:a2:15 |Mpush 21350
|  -  |528518|ROUTE| Et5                |1010 |107557  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528519|ROUTE| Et1                |1006 |107558  | c4:ca:2b:45:a2:15 |Mpush 20156
|  -  |528520|ROUTE| Et5                |1010 |107554  | 3c:08:cd:8d:ba:dc |Mpush 20159
|  -  |528521|ROUTE| Et1                |1006 |107555  | c4:ca:2b:45:a2:15 |   -   
|  -  |528522|ROUTE| Et1                |1006 |107628  | c4:ca:2b:45:a2:15 |   -   
|  -  |528523|ROUTE| Et5                |1010 |107629  | 3c:08:cd:8d:ba:dc |Mpush 20158
|  -  |528524|ROUTE| Et1                |1006 |107549  | c4:ca:2b:45:a2:15 |Mpush 20084
|  -  |528525|ROUTE| Et5                |1010 |107556  | 3c:08:cd:8d:ba:dc |Mpush 20084
|  -  |528526|DROP | DROP               |0    |  -     |                   |   -   
|  -  |528528|ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528530|ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528532|ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |   -   
|  -  |528534|ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |   -   
|  -  |528536|DROP | DROP               |0    |  -     |                   |   -   
|  -  |528538|DROP | DROP               |0    |  -     |                   |   -   
|  -  |528540|DROP | DROP               |0    |  -     |                   |   -   
|  -  |528542|DROP | DROP               |0    |  -     |                   |   -   
|  -  |528544|DROP | DROP               |0    |  -     |                   |   -   
|  -  |528546|ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528548|ROUTE| Et5                |1010 |107598  | 3c:08:cd:8d:ba:dc |Mpush 21308
|  -  |528549|ROUTE| Et1                |1006 |107599  | c4:ca:2b:45:a2:15 |Mpush 21308
|  -  |528550|ROUTE| Et5                |1010 |107610  | 3c:08:cd:8d:ba:dc |Mpush 21285
|  -  |528551|ROUTE| Et1                |1006 |107611  | c4:ca:2b:45:a2:15 |Mpush 21285
|  -  |528552|ROUTE| Et5                |1010 |107612  | 3c:08:cd:8d:ba:dc |Mpush 21182
|  -  |528553|ROUTE| Et1                |1006 |107548  | c4:ca:2b:45:a2:15 |Mpush 21308 21182
|  -  |528554|ROUTE| Et1                |1006 |107546  | c4:ca:2b:45:a2:15 |Mpush 20221
|  -  |528555|ROUTE| Et5                |1010 |107547  | 3c:08:cd:8d:ba:dc |Mpush 20221
|  -  |528556|ROUTE| Et5                |1010 |107616  | 3c:08:cd:8d:ba:dc |Mpush 21346
|  -  |528557|ROUTE| Et1                |1006 |107617  | c4:ca:2b:45:a2:15 |Mpush 21346
|  -  |528558|ROUTE| Et1                |1006 |107622  | c4:ca:2b:45:a2:15 |Mpush 21345
|  -  |528559|ROUTE| Et5                |1010 |107623  | 3c:08:cd:8d:ba:dc |Mpush 21345
|  -  |528560|ROUTE| Et1                |1006 |107624  | c4:ca:2b:45:a2:15 |Mpush 21181
|  -  |528561|ROUTE| Et5                |1010 |107625  | 3c:08:cd:8d:ba:dc |Mpush 21181
|  -  |528562|ROUTE| Et1                |1006 |107538  | c4:ca:2b:45:a2:15 |Mpush 21248
|  -  |528563|ROUTE| Et5                |1010 |107539  | 3c:08:cd:8d:ba:dc |Mpush 21248
|  -  |528564|ROUTE| Et1                |1006 |107620  | c4:ca:2b:45:a2:15 |Mpush 21284
|  -  |528565|ROUTE| Et5                |1010 |107621  | 3c:08:cd:8d:ba:dc |Mpush 21284
|  -  |528566|ROUTE| Et1                |1006 |107626  | c4:ca:2b:45:a2:15 |Mpush 21307
|  -  |528567|ROUTE| Et5                |1010 |107627  | 3c:08:cd:8d:ba:dc |Mpush 21307
|  -  |528568|ROUTE| Et1                |1006 |107630  | c4:ca:2b:45:a2:15 |Mpush 21303
|  -  |528569|ROUTE| Et5                |1010 |107631  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528570|ROUTE| Et1                |1006 |107544  | c4:ca:2b:45:a2:15 |Mpush 20066
|  -  |528571|ROUTE| Et5                |1010 |107545  | 3c:08:cd:8d:ba:dc |Mpush 20066
|  -  |528572|ROUTE| Et5                |1010 |107570  | 3c:08:cd:8d:ba:dc |Mpush 20053
|  -  |528573|ROUTE| Et1                |1006 |107572  | c4:ca:2b:45:a2:15 |Mpush 20156 20053
|  -  |528574|ROUTE| Et1                |1006 |107636  | c4:ca:2b:45:a2:15 |   -   
|  -  |528575|ROUTE| Et5                |1010 |107637  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528576|ROUTE| Et1                |1006 |107638  | c4:ca:2b:45:a2:15 |   -   
|  -  |528577|ROUTE| Et5                |1010 |107639  | 3c:08:cd:8d:ba:dc |Mpush 21685 20559
|  -  |528578|ROUTE| Et40               |1013 |107517  | 00:28:01:00:00:03 |   -   
|  -  |528580|ROUTE| Et5                |1010 |107552  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528581|ROUTE| Et1                |1006 |107553  | c4:ca:2b:45:a2:15 |Mpush 20217 20175
|  -  |528582|ROUTE| Et40               |1012 |107518  | 00:28:01:00:00:02 |   -   
|  -  |528584|ROUTE| Et40               |1008 |107521  | 00:28:01:00:00:01 |   -   
|  -  |528596|ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528598|ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528600|ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528602|ROUTE| Et5                |1010 |107573  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528603|ROUTE| Et1                |1006 |107574  | c4:ca:2b:45:a2:15 |Mpush 21685
|  -  |528608|ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |   -   
|  -  |528610|ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |   -   
|  -  |528612|ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |   -   
|  -  |528614|ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |   -   
|  -  |528616|ROUTE| Et1                |1006 |107520  | c4:ca:2b:45:a2:15 |   -   

```

